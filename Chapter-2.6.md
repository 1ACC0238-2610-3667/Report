## 2.6. Tactical-Level Domain-Driven Design

## 2.6. Bounded Contexts

### 2.6.1. Bounded Context: Identity and Access Management (IAM)

Este contexto delimitado es de alcance global y de naturaleza técnica. Su responsabilidad es gestionar la identidad de los usuarios registrados en Splitly y proporcionar los mecanismos de autenticación y autorización mediante tokens, abstrayéndose completamente de la lógica de negocio de la distribución de gastos.

#### 2.6.1.1. Domain Layer 

**Aggregates**
* **`User` (Aggregate Root):** Representa la identidad central del usuario en el sistema. Administra los datos de acceso, credenciales y su estado de actividad.
* **`Role` (Entity):** Define los niveles de acceso a nivel de plataforma (sistema) que pueden ser asignados a un `User`.

**Value Objects**
* **`Roles` (Enum):** Enumerador que encapsula y restringe los valores permitidos para los roles del sistema, garantizando type-safety en la capa de dominio.

**Commands (CQRS)**
* **`SeedRolesCommand`**: Comando empleado al inicio de la aplicación para poblar la base de datos con los roles fundamentales del sistema si estos no existen.

**Queries (CQRS)**
* **`GetAllRolesQuery`**: Solicitud para obtener la lista completa de roles disponibles.
* **`GetRoleByNameQuery`**: Solicitud para buscar un rol específico mediante su nombre.
* **`GetUserByIdQuery`**: Solicitud para obtener los detalles de un usuario a partir de su identificador único.
* **`GetUserByUsernameQuery`**: Solicitud para recuperar el perfil de un usuario utilizando su nombre de usuario (útil para validaciones de login o registro).

**Events**
* Actualmente, el modelo está preparado para soportar eventos de dominio (Domain Events) que permitirán reaccionar a cambios de estado (por ejemplo, notificar a otros Bounded Contexts cuando un nuevo `User` se registre exitosamente).

**Repositories (Interfaces de Persistencia)**
* **`IUserRepository`**: Define el contrato para las operaciones de acceso a datos relacionadas con la entidad `User`.
* **`IRoleRepository`**: Define el contrato para la persistencia y consulta de la entidad `Role`.

**Services**
* **`IUserCommandService` / `IUserQueryService`**: Segregan las responsabilidades de mutación (escritura) y lectura de la identidad del usuario, respetando el principio CQRS.
* **`IRoleCommandService` / `IRoleQueryService`**: Abstracciones para la administración y consulta de los roles del sistema.
* **`IHashingService`**: Servicio de dominio encargado de aplicar algoritmos de derivación unidireccional (hashing) a las contraseñas para su almacenamiento seguro.
* **`ITokenService`**: Servicio responsable de la generación, firma y validación de los tokens (JWT) requeridos para el acceso desde la aplicación móvil multiplataforma.
  
#### 2.6.1.2. Interface Layer

Esta capa actúa como el punto de entrada a los servicios de IAM para la aplicación móvil de **Splitly** y su Landing Page. Su responsabilidad fundamental es exponer los endpoints RESTful, gestionar las solicitudes HTTP, traducir los datos de entrada (Payload) a comandos entendibles por la capa de aplicación y formatear las respuestas de salida, manteniendo la integridad del sistema frente a clientes externos.

##### REST (Controllers)

* **`AuthenticationController`**: Es el controlador crítico para la seguridad. Expone los endpoints públicos para el registro de nuevas cuentas (`sign-up`) y la validación de credenciales para el inicio de sesión (`sign-in`), gestionando el retorno de tokens de acceso para la persistencia de sesión en el dispositivo móvil.
* **`RolesController`**: Proporciona endpoints para la lectura de los roles de sistema disponibles, permitiendo que la aplicación móvil configure los permisos básicos del usuario tras el registro.
* **`UsersController`**: Gestiona las solicitudes relacionadas con la consulta de perfiles, permitiendo recuperar la información pública de los usuarios registrados mediante su identificador único.

##### REST / Resources (DTOs)

* **`AuthenticatedUserResource`**: Estructura de datos enviada al cliente tras una autenticación exitosa. Contiene los datos básicos del usuario junto con el token JWT (Json Web Token) requerido para autorizar peticiones posteriores.
* **`RoleResource`**: Representación simplificada de la entidad `Role` (ID y nombre) para su consumo en la interfaz de usuario.
* **`SignInResource`**: Objeto de transferencia de datos que captura las credenciales (email y password) enviadas desde el formulario de inicio de sesión de la aplicación.
* **`SignUpResource`**: Estructura utilizada para recibir la información necesaria para la creación de una nueva cuenta global en la plataforma.
* **`UserResource`**: Representación pública de los datos de identidad del usuario, asegurando que información sensible como los hashes de contraseñas no se expongan fuera del backend.

##### REST / Transform (Assemblers)

* **`AuthenticatedUserResourceFromEntityAssembler`**: Mapeador encargado de construir el objeto `AuthenticatedUserResource` a partir de la entidad `User` y el token generado por la infraestructura.
* **`RoleResourceFromEntityAssembler`**: Transforma la entidad de dominio `Role` en un `RoleResource` listo para ser serializado a JSON.
* **`SignInCommandFromResourceAssembler`**: Traduce los datos del `SignInResource` a un comando de autenticación para ser procesado por la Application Layer.
* **`SignUpCommandFromResourceAssembler`**: Convierte el recurso de registro (`SignUpResource`) en el comando correspondiente para iniciar la creación del nuevo usuario.
* **`UserResourceFromEntityAssembler`**: Realiza la conversión de la entidad agregada `User` hacia un `UserResource`, filtrando cualquier dato que no deba ser enviado a la capa de presentación.

#### 2.6.1.3. Application Layer

Esta capa actúa como el motor de orquestación de **Splitly**, encargándose de implementar la lógica de los servicios definidos en la capa de dominio. Coordina las tareas de la aplicación y delega el trabajo a los objetos de dominio, asegurando que se respeten las reglas de negocio en cada transacción y manteniendo la separación de responsabilidades mediante el patrón CQRS.

**Internal**

* **CommandHandlers**: Contiene las implementaciones de los servicios de comando (escritura). Estas clases procesan los comandos que resultan en un cambio de estado en el sistema.
    * `RoleCommandServiceImpl`: Implementa la lógica para la gestión de roles, incluyendo la inicialización de los roles base (`SeedRolesCommand`) requeridos para la operación inicial del sistema.
    * `UserCommandServiceImpl`: Orquesta el proceso de registro de nuevos usuarios y la actualización de perfiles, coordinando la validación de identidad y el almacenamiento seguro.

* **QueryHandlers**: Contiene las implementaciones de los servicios de consulta (lectura). Se encargan de recuperar información sin alterar el estado de la base de datos.
    * `RoleQueryServiceImpl`: Gestiona la recuperación de roles existentes, permitiendo listar todos los roles o filtrar por criterios específicos.
    * `UserQueryServiceImpl`: Procesa las consultas para obtener la información de los usuarios mediante su identificador único o su nombre de usuario.

**OutboundServices**

Define las interfaces y servicios necesarios para interactuar con componentes técnicos externos o con otros contextos delimitados de la aplicación, manteniendo el núcleo del negocio aislado de implementaciones de infraestructura.

* **Hashing**: 
    * `IHashingService`: Define el contrato para los servicios de criptografía, encargándose de transformar las contraseñas en hashes seguros y validar las credenciales durante el inicio de sesión.
* **Tokens**:
    * `ITokenService`: Define el contrato para la gestión de la seguridad basada en tokens. Es responsable de la generación, firma y validación de los JSON Web Tokens (JWT) utilizados para autorizar las solicitudes desde la aplicación móvil.
* **ACL (Anti-Corruption Layer)**:
    * `IExternalProfileService` / `ExternalProfileService`: Actúa como una capa de anticorrupción que facilita la comunicación con otros Bounded Contexts. Su función es traducir y transferir información de identidad hacia módulos externos (como la gestión de perfiles o el registro en hogares) sin acoplar los modelos de dominio entre sí.

#### 2.6.1.4. Infrastructure Layer

Esta capa proporciona las implementaciones técnicas reales para los contratos definidos en las capas de dominio y aplicación. Es la encargada de gestionar el acceso a la base de datos, la seguridad criptográfica, la generación de tokens y la intercepción de peticiones en el pipeline, asegurando que los detalles de implementación permanezcan aislados de la lógica de negocio.

**Hashing**
* **`HashingService`**: Implementación concreta de la interfaz `IHashingService`. Utiliza internamente el algoritmo BCrypt para transformar las contraseñas de los usuarios en hashes seguros antes de su persistencia, garantizando la protección de las credenciales.

**Persistence / EFC (Entity Framework Core)**
* **`IAMContext`**: Contexto de base de datos específico para este Bounded Context. Configura las entidades `User` y `Role` mediante Fluent API, definiendo la estructura de las tablas, claves primarias y restricciones en el motor de base de datos.
* **`UserRepository`**: Implementación del repositorio (hereda de la configuración base) encargada de las operaciones de acceso a datos, consultas y mutaciones específicas para la entidad `User`.
* **`RoleRepository`**: Implementación del repositorio que maneja las operaciones CRUD reales sobre la tabla de roles en la base de datos.

**Pipeline / Middleware / Components**
* **`RequestAuthorizationMiddleware`**: Componente crítico en el pipeline de peticiones HTTP. Actúa como un middleware que intercepta las solicitudes entrantes para validar la presencia y autenticidad del token JWT. Si el token es válido, extrae los claims (como el ID del usuario) y los inyecta en el contexto de la petición (`HttpContext`), autorizando el acceso a los endpoints protegidos de la API.

**Tokens**
* **`TokenService`**: Implementación técnica de `ITokenService`. Es responsable de la creación, firma criptográfica y validación de los JSON Web Tokens (JWT) que permiten a los usuarios de la aplicación móvil y web mantener sus sesiones de forma segura.
* **`TokenSettings`**: Clase ubicada en la carpeta de configuración de tokens. Se encarga de mapear y tipar fuertemente los parámetros de seguridad definidos en el archivo `appsettings.json` (como el `Secret`, `Issuer`, `Audience` y el tiempo de expiración en días).

#### 2.6.1.5. Bounded Context Software Architecture Component Level Diagrams

El siguiente diagrama de componentes ilustra la estructura interna y el flujo de interacción dentro del Bounded Context de Identity and Access Management (IAM). Esta representación visual materializa la arquitectura en capas descrita en los apartados anteriores, evidenciando cómo se aplica el patrón Clean Architecture y CQRS en el proyecto. 

En el diagrama se detalla cómo las solicitudes de los clientes (como el inicio de sesión o el registro) son interceptadas por la **Interface Layer** (Controllers), las cuales delegan la orquestación a la **Application Layer** (Command y Query Handlers). Asimismo, se observa cómo estos servicios orquestadores interactúan con las entidades de la **Domain Layer** para validar las reglas de negocio, y finalmente se apoyan en la **Infrastructure Layer** (Repositories, TokenService, y IAMContext) para la persistencia de datos y la generación de credenciales seguras.

![Diagrama de componentes IAM](images/IAM%20-%20diagraman%20-%20componentes.png)

### 2.6.1.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.1.6.1 Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio representa el modelo conceptual de negocio para el contexto de **Identity and Access Management (IAM)**. En este esquema se visualizan las entidades fundamentales, como `User` (Aggregate Root) y `Role`, junto con sus atributos esenciales y las relaciones que definen el comportamiento del sistema de identidades. 

Este modelo se mantiene estrictamente agnóstico a factores externos, como la persistencia en base de datos o los protocolos de comunicación, centrándose únicamente en las reglas de dominio que rigen la creación y validación de usuarios y sus niveles de acceso dentro de la plataforma **Splitly**.

![Diagrama de Clases del Dominio](images/diagram-class-IAM.png)

#### 2.6.1.6.2 Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos (Entity-Relationship) estructurado específicamente para el contexto de **Identity and Access Management (IAM)**. 

En este esquema se visualiza la estructura relacional de las tablas empleadas para la persistencia de identidades y accesos, aislando las tablas `users`, `roles` y la tabla de resolución `user_roles`. Se especifican los atributos, las claves primarias (PK) y las claves foráneas (FK) que garantizan la integridad referencial y modelan correctamente la asignación de permisos a los usuarios registrados en la plataforma **Splitly**.

![Diagrama de Base de Datos](images/diagram-BD-IAM.png)

### 2.6.2. Bounded Context: Contributions Distribution

El Bounded Context de **Contributions Distribution** representa el núcleo matemático y de registro de cuentas de la plataforma **Splitly**. Su propósito principal es gestionar el ciclo de vida de los gastos compartidos, garantizando precisión en la división y trazabilidad en los compromisos de cada usuario.

A nivel arquitectónico, este límite transaccional consolida de manera cohesiva tres sub-dominios lógicos fundamentales:
* **Bills:** Encargado del registro, emisión y categorización de los gastos o facturas centrales generados dentro del hogar.
* **Contributions:** Actúa como el motor de reglas de negocio que aplica diferentes métodos de asignación matemática para fragmentar un gasto (Bill) y determinar la obligación financiera exacta que le corresponde a cada miembro.
* **Members Contribution:** Responsable del seguimiento interno y registro del estado de las cuotas de los usuarios (marcando y conciliando quién ya cumplió con su parte de la deuda), operando de forma independiente a la pasarela de pagos.

Al unificar estas responsabilidades en un único Bounded Context, el sistema asegura que la generación de un gasto y el cálculo automático de sus respectivas deudas se mantengan siempre consistentes, altamente cohesivos y sincronizados.

#### 2.6.2.1. Domain Layer

La capa de dominio (Domain Layer) del Bounded Context de **Contributions Distribution** encapsula la lógica central del negocio para el registro de gastos y la conciliación de deudas. Al ser el núcleo del sistema, esta capa es completamente independiente de frameworks, bases de datos o interfaces de usuario, modelando fielmente las reglas matemáticas y financieras de la plataforma.

A partir de la consolidación de los submódulos, el modelo de dominio se estructura mediante los siguientes elementos tácticos:

**Aggregates y Entities:**
* **`Expense` (Aggregate Root):** Es la entidad raíz que representa una factura o gasto general del hogar. Controla la consistencia de los datos del cobro (monto total, fecha de emisión `issueDate`, fecha de vencimiento `dueDate`) y actúa como punto de entrada para agregar detalles o marcar el gasto como liquidado (`markSettled()`).
* **`ExpenseLine` (Entity):** Representa cada uno de los ítems o líneas de detalle que componen un gasto mayor, especificando su propia categoría (`category`), monto (`amount`) y notas adicionales.
* **`DocumentAttachment` (Entity):** Gestiona los comprobantes físicos o digitales (recibos, facturas en PDF/imagen) asociados a un gasto para garantizar la transparencia, almacenando la clave del archivo (`fileKey`).
* **`Contribution` (Aggregate Root / Entity):** Representa el cálculo general de división de un gasto (`expenseId`). Contiene la lógica para recomputar (`recompute()`) las obligaciones financieras basándose en una política o método de asignación.
* **`ContributionItem` (Entity):** Representa la obligación financiera individual y exacta de un miembro del hogar (`memberId`). Define el porcentaje de la deuda, el monto a pagar y cuánto ha sido pagado hasta el momento (`paidTotal`).
* **`Payment` (Entity):** Registra la transacción individual que realiza un miembro para cubrir su cuota (`contributionItemId`). Encapsula el monto abonado, la fecha (`paidAt`), la referencia de la operación y los métodos para confirmar o conciliar el pago (`confirm()`, `reconcile()`).

**Value Objects y Enumeradores:**
* **Enumeradores de Estado:** `ExpenseStatus` y `PaymentStatus` para manejar el ciclo de vida de las deudas (ej. Pendiente, Saldado, Confirmado).
* **Enumeradores de Categoría y Método:** `ExpenseCategory` (ej. Comida, Servicios) y `PaymentMethod` (ej. Efectivo, Transferencia).
* **`AllocationMethod`:** Define la estrategia matemática para dividir el gasto (Partes iguales, Porcentual, etc.).

**Repositories (Interfaces):**
Para garantizar la persistencia de estos agregados sin acoplar el dominio a la base de datos, se exponen los siguientes contratos:
* **`IExpenseRepository`:** Contrato para persistir y recuperar los gastos generales y sus líneas de detalle.
* **`IContributionRepository`:** Contrato para gestionar el almacenamiento de los cálculos de división y las cuotas individuales.
* **`IPaymentRepository`:** Contrato para registrar el historial de transacciones y abonos de los miembros.

#### 2.6.2.2. Interface Layer

La capa de interfaz (Interface Layer) para el Bounded Context de **Contributions Distribution** actúa como la frontera externa del módulo. Su responsabilidad es recibir las solicitudes HTTP desde las aplicaciones cliente (móviles o web), transformar las cargas útiles (payloads) mediante DTOs, y enrutar las peticiones hacia la capa de aplicación correspondiente, protegiendo así el modelo de dominio subyacente.

Alineado con los agregados definidos en el modelo, esta capa expone los siguientes controladores RESTful y componentes:

**REST Controllers:**
* **`ExpensesController`:** Punto de entrada para la gestión de las facturas del hogar. Expone rutas para registrar un nuevo gasto, añadir líneas de detalle (`ExpenseLine`), subir comprobantes (`DocumentAttachment`) y actualizar el estado general del cobro.
* **`ContributionsController`:** Expone los endpoints para consultar y gestionar la división de los gastos. Permite solicitar la recomputación de las cuotas (`recompute()`) basándose en una política específica y obtener el listado de las obligaciones (`ContributionItem`) de cada miembro.
* **`PaymentsController`:** Maneja las peticiones relacionadas con la liquidación de las deudas. Expone rutas para que un usuario registre el pago de su cuota, y para que el representante del hogar pueda confirmar (`confirm()`) y conciliar (`reconcile()`) dichos abonos.

**Data Transfer Objects (DTOs / Resources):**
Para evitar exponer las entidades de dominio directamente, se implementan contratos de datos de entrada y salida, tales como:
* **Request Resources:** Clases como `CreateExpenseResource`, `AddExpenseLineResource`, o `RegisterPaymentResource`, que encapsulan los datos crudos enviados por el cliente y validan su formato antes de procesarlos.
* **Response Resources:** Clases como `ExpenseResponse`, `ContributionItemResponse`, o `PaymentResponse`, diseñadas para devolver al cliente únicamente la información relevante y segura, ocultando detalles de implementación interna y estructurando los datos de forma óptima para la interfaz de usuario.

#### 2.6.2.3. Application Layer

La capa de aplicación (Application Layer) en el Bounded Context de **Contributions Distribution** actúa como el orquestador central de los casos de uso financieros del sistema. Su responsabilidad principal es recibir las solicitudes desde la capa de interfaz, interactuar con los repositorios para recuperar las entidades, invocar la lógica de negocio pertinente en la capa de dominio, y finalmente guardar los cambios de estado. 

Para mantener el código escalable y organizado, esta capa implementa el patrón CQRS, separando las operaciones de lectura (Queries) de las de escritura (Commands):

**Commands (Operaciones de Escritura) y Command Handlers:**
Encapsulan la intención de mutar el estado de los gastos y deudas en el sistema. Los *Handlers* correspondientes orquestan el flujo transaccional de estas operaciones:
* **`ExpenseCommandService` / Handlers:** Orquesta casos de uso como `CreateExpenseCommand` (para instanciar un nuevo gasto central), `AddExpenseLineCommand` (invocando el método `addLine` del agregado) y `MarkExpenseAsSettledCommand` (ejecutando `markSettled()`).
* **`ContributionCommandService` / Handlers:** Gestiona comandos como `ComputeContributionsCommand`. Este handler es vital porque recupera el gasto, obtiene la política de asignación (`AllocationMethod`) y delega al agregado `Contribution` la ejecución de su método `recompute()`.
* **`PaymentCommandService` / Handlers:** Controla el ciclo de vida de los abonos mediante comandos como `RegisterPaymentCommand` (creando una nueva entidad `Payment`), y orquesta los cambios de estado ejecutando `confirm()` y `reconcile()` tras validaciones exitosas.

**Queries (Operaciones de Lectura) y Query Handlers:**
Encapsulan las solicitudes de información sin alterar el estado del sistema, optimizadas para devolver datos de forma rápida hacia los recursos de respuesta (Response DTOs):
* **`ExpenseQueryService` / Handlers:** Gestiona consultas como `GetExpenseByIdQuery` para ver los detalles de una factura y sus comprobantes (`DocumentAttachment`), o `GetExpensesByHouseholdQuery`.
* **`ContributionQueryService` / Handlers:** Atiende solicitudes como `GetContributionItemsByMemberQuery`, la cual es fundamental para que el cliente móvil pueda renderizar en pantalla cuánto dinero debe exactamente un usuario en un momento dado.

De esta manera, la capa de aplicación coordina eficientemente las matemáticas puras del modelo de dominio sin acoplarse a los detalles de la base de datos (Entity Framework) ni a los controladores de la API.

#### 2.6.2.4. Infrastructure Layer

La capa de infraestructura (Infrastructure Layer) para el Bounded Context de **Contributions Distribution** es la responsable de materializar los contratos definidos en el dominio, gestionando la persistencia de los datos financieros y la integración con servicios técnicos externos. Esta capa aísla los detalles tecnológicos (como el ORM y el almacenamiento en la nube) para que el núcleo de la aplicación se mantenga limpio e independiente.

Para este contexto delimitado, la infraestructura se compone de los siguientes elementos clave:

**Persistencia de Datos y ORM:**
Se utiliza Entity Framework Core (EF Core) como herramienta de mapeo objeto-relacional, gestionando el ciclo de vida de los datos a través de un contexto de base de datos específico (ej. `ContributionsDbContext` o un esquema dedicado dentro del contexto principal).
* **Mapeo de Entidades (Fluent API):** Se configuran las reglas de persistencia para garantizar la integridad referencial. Se mapean las relaciones de uno a muchos (1..*) observables en el modelo de dominio, como la relación entre `Expense` y sus `ExpenseLines` o `DocumentAttachments`, y la jerarquía entre `Contribution`, `ContributionItem` y `Payment`.
* **Precisión Financiera:** Se configuran las restricciones de tipo de dato para garantizar que los atributos monetarios (`amount`, `total`, `paidTotal` de tipo Decimal) se almacenen con la precisión exacta requerida para aplicaciones financieras, evitando errores de redondeo.
* **Mapeo de Enumeradores:** Los Value Objects y estados (`ExpenseStatus`, `PaymentStatus`, `AllocationMethod`) se configuran para ser persistidos como cadenas de texto (Strings) o enteros (Ints) en la base de datos, facilitando su lectura y mantenimiento.

**Implementación de Repositorios:**
Se proveen las implementaciones concretas de las interfaces del dominio, interactuando directamente con el `DbContext`:
* **`ExpenseRepository`:** Implementa la lógica SQL/LINQ para guardar facturas, incluyendo la inserción en cascada de sus líneas de detalle.
* **`ContributionRepository`:** Gestiona el guardado y la recuperación de las obligaciones financieras recomputadas.
* **`PaymentRepository`:** Inserta los registros de pagos y actualiza el estado de las transacciones conciliadas.

**Servicios Externos (Integraciones):**
* **Storage Services:** Para respaldar la entidad `DocumentAttachment`, se implementa un servicio de infraestructura (ej. `S3StorageService` o `BlobStorageService`) que gestiona la subida física de los comprobantes (imágenes o PDFs) a la nube, devolviendo el `fileKey` que finalmente se guarda en la base de datos relacional.

### 2.6.2.5. Bounded Context Software Architecture Component Level Diagrams

El siguiente diagrama de componentes ilustra la arquitectura de software interna del Bounded Context de **Contributions Distribution**. Esta representación visual detalla cómo los sub-dominios lógicos (Bills, Contributions y Members Contribution) están estructurados utilizando los principios de Clean Architecture y el Modelo C4.

El diagrama describe el flujo de dependencias a través de las cuatro capas principales:

* **Interface Layer:** Expone los endpoints de la API REST (`ExpensesController`, `ContributionsController`, `PaymentsController`) para manejar las peticiones HTTP entrantes desde las aplicaciones cliente.
* **Application Layer:** Orquesta los casos de uso del sistema a través de servicios de tipo Command y Query, delegando tareas sin contener ninguna lógica de negocio central.
* **Domain Layer:** El corazón del Bounded Context, donde se encapsulan las reglas puras de negocio, los métodos matemáticos de asignación o reparto y los Agregados principales (`Expense`, `Contribution`, `Payment`).
* **Infrastructure Layer:** Implementa las interfaces de persistencia, mapeando las entidades del dominio a la **Base de Datos Relacional** mediante Entity Framework Core, e interactuando con servicios externos de almacenamiento en la nube (**Cloud Storage Services**) para gestionar los `DocumentAttachments` (como los recibos o comprobantes de gastos).

Al imponer estos límites, la arquitectura garantiza que la lógica financiera central permanezca completamente aislada de las tecnologías de base de datos y de los frameworks de interfaz de usuario.

![Diagrama de Componentes Contributions Distribution](images/component-diagram-Contributions%20Distribution.png)


### 2.6.2.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.2.6.1 Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio ilustra el modelo conceptual de negocio estructurado específicamente para el Bounded Context de **Contributions Distribution**. 

En este esquema se visualizan las entidades centrales que conforman este límite transaccional, destacando los Aggregate Roots (`Expense` y `Contribution`) y sus entidades relacionadas (`ExpenseLine`, `Payment`, `ContributionItem`). Se detallan sus atributos esenciales, métodos de comportamiento (como `recompute()` y `registerPayment()`) y las multiplicidades que rigen las reglas de división de gastos y liquidación de deudas.

Al omitir intencionalmente detalles de infraestructura y dependencias externas, este modelo demuestra una alta cohesión interna y se mantiene estrictamente agnóstico a frameworks de persistencia o interfaces de usuario, cumpliendo fielmente con los principios tácticos de Domain-Driven Design (DDD).

![Diagrama de contexto Contributions Distribution](images/diagrama%20-%20context%20domain%20-%20distribution%20contribution.png)


#### 2.6.2.6.2 Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos (Entity-Relationship) estructurado específicamente para dar soporte a la persistencia del Bounded Context de **Contributions Distribution**. 

En este esquema se aíslan las tablas responsables de almacenar la información financiera y transaccional del módulo. Se observan las tablas `bills` (que materializa el agregado de gastos), `contributions` (que almacena las cuotas proporcionales calculadas mediante las políticas de reparto) y `member_contributions` (que registra el estado de los pagos y liquidaciones de cada usuario).

El diagrama detalla los atributos físicos, los tipos de datos implícitos, las claves primarias (PK) y las relaciones de clave foránea (FK) que garantizan la integridad referencial de las reglas de negocio finacieras de **Splitly**, manteniendo este esquema lógicamente separado de otros dominios como la gestión de identidades o el ciclo de vida de los hogares.

![Diagrama de base de datos Contributions Distribution](images/diagrama%20-%20base%20de%20datos%20-%20contribution%20distributions.png)

### 2.6.3. Bounded Context: Household Management

El Bounded Context de **Household Management** constituye la base estructural y organizativa de la plataforma. Su propósito fundamental es administrar el ciclo de vida de los grupos o "hogares", actuando como el contenedor lógico principal donde interactúan los usuarios y sobre el cual se asociarán posteriormente los gastos y deudas.

A nivel de diseño guiado por el dominio (DDD), este límite transaccional consolida de manera natural tres sub-dominios que comparten un alto grado de cohesión y operan en conjunto:
* **Households:** Encargado de la creación, configuración y administración del hogar en sí (entidad raíz), definiendo sus metadatos (como nombre o moneda base) y su estado de actividad.
* **HouseholdMembers:** Responsable de establecer el vínculo entre los usuarios del sistema y un hogar específico. Gestiona los roles locales dentro del grupo, la fecha de ingreso y el estado de la membresía.
* **Invitations:** Maneja la lógica de integración de nuevos participantes, controlando la generación, envío, validación, aceptación o expiración de los enlaces o códigos de invitación para unirse a un grupo.

La unificación de estas responsabilidades en un solo Bounded Context garantiza que las reglas de negocio sobre quién pertenece a un hogar y cómo ingresa a él se procesen de forma atómica. Esto asegura la integridad de los datos organizativos y proporciona una fuente de la verdad confiable para que módulos externos (como el de distribución de aportes) puedan operar sin preocuparse por la gestión de los usuarios.

#### 2.6.3.1. Domain Layer 

La capa de dominio (Domain Layer) para el Bounded Context de **Household Management** encapsula las reglas de negocio centrales encargadas de la estructuración y organización de los grupos de usuarios. Esta capa se mantiene completamente aislada de bases de datos, frameworks externos o detalles de la interfaz, enfocándose en la lógica pura de la creación de hogares, la administración de sus integrantes y la seguridad de los accesos mediante invitaciones.

A continuación, se detallan los elementos tácticos que estructuran esta capa, reflejando la integración de los submódulos de *Households*, *HouseholdMembers* e *Invitations*:

**Aggregates y Entities:**
* **`Household` (Aggregate Root):** Es la entidad principal que representa un grupo, vivienda o departamento compartido. Concentra la información base (nombre, descripción, moneda principal para las transacciones internas) y actúa como el límite de consistencia transaccional del módulo.
* **`HouseholdMember` (Entity):** Representa el vínculo específico entre un usuario del sistema y un hogar. Define el estado de la membresía, la fecha en la que el usuario se unió (`joinedAt`) y el nivel de permisos locales que posee dentro de ese grupo específico.
* **`Invitation` (Entity):** Gestiona el ciclo de vida de las solicitudes o códigos de acceso para integrar nuevos miembros a un hogar. Encapsula la lógica para verificar la validez del token, comprobar las fechas de expiración (`expiresAt`) y actualizar su estado una vez que un usuario acepta la invitación.

**Value Objects y Enumeradores:**
* **`InvitationStatus`:** Enumerador que define las transiciones de estado de una invitación (por ejemplo: *Pending*, *Accepted*, *Expired*, *Revoked*).
* **`HouseholdRole`:** Enumerador que define la jerarquía o nivel de permisos de un integrante dentro del hogar (por ejemplo: *Owner/Admin*, *Regular Member*).

**Repositories (Interfaces):**
Para garantizar la persistencia de estas entidades asegurando el principio de Inversión de Dependencias (Dependency Inversion), el dominio expone los siguientes contratos:
* **`IHouseholdRepository`:** Contrato para la creación, actualización y recuperación de los metadatos de los hogares.
* **`IHouseholdMemberRepository`:** Contrato para gestionar el listado de participantes de un hogar y para consultar a cuántos grupos pertenece un usuario en particular.
* **`IInvitationRepository`:** Contrato encargado de almacenar, consultar y actualizar los tokens de acceso temporales.

#### 2.6.3.2. Interface Layer

La capa de interfaz (Interface Layer) para el Bounded Context de **Household Management** funciona como el punto de entrada y la frontera de comunicación externa del módulo. Su responsabilidad principal es recibir las solicitudes HTTP enviadas desde las aplicaciones cliente (Web o Móvil), transformar las cargas útiles (payloads) utilizando objetos de transferencia de datos (DTOs), y delegar la ejecución hacia la capa de aplicación, protegiendo así la lógica de negocio subyacente.

Basándose en los agregados y entidades definidos en el modelo de dominio, esta capa expone los siguientes controladores RESTful y componentes:

**REST Controllers:**
* **`HouseholdsController`:** Constituye el punto de entrada para la gestión principal de los grupos. Expone endpoints para crear un nuevo hogar, actualizar su información base (como el nombre o la moneda), y consultar los detalles de los hogares a los que pertenece el usuario autenticado.
* **`HouseholdMembersController`:** Maneja las peticiones relacionadas con los integrantes de un grupo específico. Expone rutas para listar a los miembros actuales, actualizar sus roles internos (`HouseholdRole`), o procesar la salida/eliminación de un integrante del hogar.
* **`InvitationsController`:** Gestiona el flujo de integración de nuevos usuarios. Expone endpoints para generar un nuevo token o enlace de invitación, consultar el estado de una invitación y procesar la aceptación de la misma por parte de un usuario invitado.

**Data Transfer Objects (DTOs / Resources):**
Para aislar el modelo de dominio de los contratos de la API, se implementan recursos de entrada y salida para estructurar la información:
* **Request Resources:** Clases como `CreateHouseholdResource`, `UpdateMemberRoleResource`, o `GenerateInvitationResource`, encargadas de encapsular los datos enviados por el cliente y aplicar validaciones de formato (Data Annotations) antes de que la petición ingrese al sistema.
* **Response Resources:** Clases como `HouseholdResponse`, `HouseholdMemberResponse`, e `InvitationResponse`, diseñadas para mapear las entidades internas y devolver al cliente únicamente la información estructurada, segura y necesaria para la interfaz de usuario.

#### 2.6.3.3. Application Layer

La capa de aplicación (Application Layer) en el Bounded Context de **Household Management** actúa como el orquestador central de los casos de uso relacionados con la administración de los grupos. Su función primordial es recibir las intenciones de los usuarios desde la capa de interfaz, recuperar las entidades pertinentes a través de los repositorios, invocar las reglas de negocio del dominio y coordinar la persistencia de los cambios de estado.

Para garantizar un código mantenible, escalable y con responsabilidades segregadas, esta capa implementa el patrón CQRS (Command and Query Responsibility Segregation), dividiendo el flujo de ejecución en operaciones de escritura y de lectura:

**Commands (Operaciones de Escritura) y Command Handlers:**
Encapsulan las solicitudes que mutan o alteran el estado organizativo de los hogares. Los servicios o *Handlers* encargados orquestan el flujo transaccional:
* **`HouseholdCommandService` / Handlers:** Orquesta casos de uso fundamentales como `CreateHouseholdCommand` (que inicializa un nuevo grupo) y `UpdateHouseholdCommand` (para modificar metadatos del hogar).
* **`HouseholdMemberCommandService` / Handlers:** Gestiona la administración del equipo humano mediante comandos como `AddMemberToHouseholdCommand`, `UpdateMemberRoleCommand` (para escalar o reducir privilegios locales) y `RemoveMemberCommand`.
* **`InvitationCommandService` / Handlers:** Controla el flujo de seguridad e integración ejecutando comandos críticos como `GenerateInvitationCommand`, `RevokeInvitationCommand` y, especialmente, el `AcceptInvitationCommand`, el cual orquesta la transición de una invitación aceptada a la creación de un nuevo `HouseholdMember`.

**Queries (Operaciones de Lectura) y Query Handlers:**
Encapsulan las solicitudes de información, diseñadas para consultar el estado del sistema sin producir efectos secundarios, optimizando la lectura de datos:
* **`HouseholdQueryService` / Handlers:** Resuelve consultas como `GetHouseholdByIdQuery` y `GetHouseholdsByUserIdQuery`, permitiendo al cliente saber a qué grupos pertenece el usuario autenticado.
* **`HouseholdMemberQueryService` / Handlers:** Atiende solicitudes como `GetMembersByHouseholdIdQuery`, vital para renderizar la lista de participantes y sus roles dentro de la interfaz de la aplicación.
* **`InvitationQueryService` / Handlers:** Gestiona consultas como `GetInvitationByTokenQuery`, utilizada para validar que el enlace o código que ingresa un usuario invitado siga vigente antes de permitirle unirse.

Mediante esta arquitectura, la capa de aplicación coordina eficientemente la gestión del ciclo de vida de los hogares, delegando la complejidad técnica a la infraestructura y las reglas organizativas a la capa de dominio.

#### 2.6.3.4 Infrastructure Layer

La capa de infraestructura (Infrastructure Layer) para el Bounded Context de **Household Management** es la encargada de proveer las implementaciones tecnológicas concretas para las abstracciones definidas en la capa de dominio. Su rol principal es gestionar el acceso a la base de datos relacional y coordinar la integración con servicios externos, manteniendo el núcleo de la aplicación completamente agnóstico respecto a la infraestructura física.

En este contexto delimitado, la infraestructura se organiza mediante los siguientes componentes técnicos:

**Persistencia de Datos y ORM:**
La persistencia transaccional se maneja a través de Entity Framework Core (EF Core), utilizando un contexto de base de datos específico para el módulo (o un esquema delimitado) que aísla las tablas organizativas del resto del sistema.
* **Mapeo de Entidades (Fluent API):** Se configuran las reglas de mapeo objeto-relacional (O/RM) garantizando la integridad referencial. Se establecen las relaciones estructurales, como la relación de uno a muchos (1..*) entre un `Household` y sus múltiples `HouseholdMembers` e `Invitations`.
* **Configuración de Enumeradores y Restricciones:** Los Value Objects y estados transicionales (como `InvitationStatus` y `HouseholdRole`) se configuran para ser persistidos eficientemente (generalmente como cadenas de texto o enteros), mientras que se aplican restricciones de base de datos, como índices únicos para los tokens de invitación, evitando duplicidades.

**Implementación de Repositorios:**
Se proveen las clases concretas que implementan las interfaces del dominio, interactuando directamente con el `DbContext`:
* **`HouseholdRepository`:** Implementa la lógica SQL/LINQ para la inserción, actualización y consulta de los metadatos de los hogares.
* **`HouseholdMemberRepository`:** Gestiona el almacenamiento de los vínculos entre los usuarios y los grupos, incluyendo la persistencia de los roles y permisos locales asignados a cada integrante.
* **`InvitationRepository`:** Encargado de registrar los tokens de invitación generados, actualizar su estado (ej. de *Pending* a *Accepted* o *Expired*) y recuperar validaciones críticas directamente desde la base de datos.

**Integración con Servicios Externos:**
* **Email / Notification Service (Adapter):** Para dar soporte al sub-dominio de `Invitations`, esta capa puede incluir la implementación de adaptadores que se conecten con proveedores de mensajería externos (ej. SendGrid o un SMTP Server). De esta forma, cuando el dominio ordena el envío de una invitación, la capa de infraestructura materializa el envío físico del correo electrónico o notificación al destinatario sin acoplar la lógica de negocio al proveedor de correo.

#### 2.6.3.5 Bounded Context Software Architecture Component Level Diagrams

El siguiente diagrama a nivel de componentes ilustra la arquitectura de software interna del Bounded Context de **Household Management**. Esta representación visual demuestra cómo los sub-dominios lógicos (Households, HouseholdMembers e Invitations) están estructurados utilizando las capas de Clean Architecture y el enfoque del Modelo C4.

El diagrama detalla el flujo de control y las dependencias a través de las cuatro capas principales:
* **Interface Layer:** Expone los endpoints de la API REST (`HouseholdsController`, `HouseholdMembersController`, `InvitationsController`) responsables de recibir y manejar las peticiones HTTP provenientes de las aplicaciones cliente.
* **Application Layer:** Orquesta los casos de uso centrales a través de servicios de tipo Command y Query, gestionando el ciclo de vida de los grupos y el proceso de invitaciones sin contener reglas puras de negocio.
* **Domain Layer:** Actúa como el núcleo aislado del Bounded Context, encapsulando la lógica de negocio, las reglas organizativas y los Agregados principales (`Household`, `HouseholdMember`, `Invitation`).
* **Infrastructure Layer:** Implementa los adaptadores técnicos requeridos. Maneja la persistencia de datos mapeando las entidades del dominio hacia la **Base de Datos Relacional** mediante Entity Framework Core, y se integra con servicios externos de **Email / Notificaciones** (como SendGrid o SMTP) para el envío físico de los enlaces de invitación a los nuevos usuarios.

Este diseño arquitectónico garantiza una alta cohesión dentro de la lógica de gestión de grupos, manteniendo al mismo tiempo un bajo acoplamiento con los proveedores de bases de datos y los servicios de comunicación externos.

![Diagrama de componentes Household Management](images/Household%20Management%20-%20component%20diagram.png)

### 2.6.3.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.3.6.1. Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio ilustra el modelo conceptual de negocio estructurado específicamente para el Bounded Context de **Household Management**. Este esquema visualiza las entidades centrales y Aggregate Roots que conforman este límite transaccional, respetando estrictamente los principios tácticos de Domain-Driven Design (DDD).

En el modelo se identifica a `Household` como el Aggregate Root principal, responsable de mantener la consistencia del grupo u hogar. A esta raíz se asocian de manera transaccional las entidades subordinadas `HouseholdMember` (que define el vínculo usuario-hogar y su rol interno) e `Invitation` (que gestiona el ciclo de vida de los accesos organizativos). 

Se detallan además los enumeradores necesarios (`HouseholdRole`, `InvitationStatus`) y los métodos de comportamiento (tales como `Accept()`, `AddMember()` o `CreateInvitation()`), asegurando un modelo cohesivo que permanece agnóstico de frameworks externos o detalles de persistencia.

![Diagrama de contexto Household Management](images/Household%20Management%20BC%20-%20diagram%20-%20context.png)

#### 2.6.3.6.2. Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos estructurado específicamente para dar soporte al Bounded Context de **Household Management**. Este esquema aísla las tablas responsables de almacenar la estructura organizativa de los grupos dentro de la plataforma.

En el diagrama se observa la tabla principal `households` (que almacena los metadatos de los grupos), relacionada mediante claves foráneas (FK) con las tablas subordinadas `household_members` (que registra la unión de los usuarios con el grupo y sus roles locales) e `invitations` (que persiste los tokens de acceso temporales y su estado de vigencia). 

Este diseño garantiza la integridad referencial de la organización de los equipos, manteniendo estas tablas lógicamente separadas de otros dominios de la base de datos, como las transacciones financieras o la gestión global de identidades (IAM).

![Diagrama de base de datos Household Management](images/diagrama%20-%20base%20de%20datos%20-%20Household%20Management.png)

### 2.6.4. Bounded Context: App Management

El Bounded Context de **App Management** actúa como la columna vertebral operativa y de infraestructura de la plataforma. A diferencia de los módulos centrales que manejan la lógica matemática de las deudas o la organización de los hogares, este contexto se enfoca exclusivamente en los aspectos transversales necesarios para el funcionamiento, la personalización y la integración técnica del sistema.

Bajo la perspectiva de Domain-Driven Design (DDD), este límite transaccional agrupa dos sub-dominios clave que dictan el comportamiento global de la aplicación y su comunicación con servicios financieros externos:

* **Settings:** Responsable de administrar las preferencias y configuraciones, tanto a nivel de sistema como de usuario. Esto incluye la gestión de metadatos de la aplicación, preferencias de notificaciones, localización (idioma/moneda por defecto), temas visuales (Dark/Light mode) y el versionado de políticas operativas.
* **Payment Gateway:** Funciona como una Capa Anticorrupción (Anti-Corruption Layer) diseñada para integrar y gestionar la comunicación con procesadores de pago externos (como Stripe, PayPal o pasarelas locales). Su responsabilidad es encapsular la complejidad técnica de las transacciones reales, la tokenización de métodos de pago y el procesamiento de *webhooks*, aislando al resto del sistema de los cambios en las APIs de terceros.

#### 2.6.4.1. Domain Layer

La capa de dominio (Domain Layer) para el Bounded Context de **App Management** encapsula la lógica central enfocada en la personalización de la experiencia del usuario y las reglas de validación para las transacciones financieras externas. Esta capa se mantiene estrictamente aislada de los detalles de implementación tecnológica, como la base de datos o los SDKs específicos de los proveedores de pago (ej. Stripe, PayPal o Niubiz).

A continuación, se detallan los elementos tácticos que estructuran esta capa, reflejando la consolidación de los submódulos de *Settings* y *Payment Gateway*:

**Aggregates y Entities:**
* **`UserSetting` (Aggregate Root):** Es la entidad encargada de gestionar las preferencias transversales de un usuario dentro de la plataforma. Centraliza la configuración de la experiencia, manejando atributos como el idioma preferido, el tema de la interfaz (modo oscuro/claro) y los permisos generales de notificaciones.
* **`PaymentIntent` / `TransactionRecord` (Aggregate Root):** Entidad que representa y rastrea una solicitud de pago canalizada hacia un proveedor externo. Encapsula datos críticos como el monto total, la moneda, el identificador externo de la transacción y la fecha de inicio, controlando el ciclo de vida del pago de forma agnóstica.
* **`PaymentMethodProfile` (Entity):** Representa un método de pago previamente guardado y tokenizado de un usuario. Por razones de seguridad y cumplimiento normativo (PCI-DSS), no almacena datos sensibles reales (como el número completo de tarjeta o el CVV), sino únicamente el token de referencia provisto por la pasarela de pagos.

**Value Objects y Enumeradores:**
* **`TransactionStatus`:** Enumerador que define las transiciones de estado de un intento de pago (por ejemplo: *Pending*, *RequiresAction*, *Succeeded*, *Failed*, *Refunded*).
* **`ThemePreference`:** Enumerador para los ajustes visuales de la aplicación (*Light*, *Dark*, *SystemDefault*).
* **`Money` (Value Object):** Estructura inmutable que combina la cantidad y la divisa (código ISO), asegurando que todas las solicitudes enviadas a la pasarela de pagos tengan precisión decimal y validación económica correcta.

**Repositories y Domain Services (Interfaces):**
Para establecer una Capa Anticorrupción (ACL) y asegurar el principio de Inversión de Dependencias (Dependency Inversion), el dominio expone los siguientes contratos:
* **`IUserSettingRepository`:** Contrato para recuperar, crear y actualizar las preferencias de la aplicación para un usuario específico.
* **`IPaymentTransactionRepository`:** Contrato responsable de registrar y auditar el historial de los intentos de pago.
* **`IPaymentGatewayService` (Domain Service Contract):** Contrato vital que define las operaciones permitidas con el procesador de pagos externo (por ejemplo, `ChargeTokenizedCard()`, `GeneratePaymentLink()`, `RefundTransaction()`). La implementación real residirá en la capa de infraestructura, blindando el núcleo de **Splitly** ante cualquier cambio en las APIs de terceros.

#### 2.6.4.2. Interface Layer

La capa de interfaz (Interface Layer) para el Bounded Context de **App Management** actúa como la frontera de comunicación entre las aplicaciones cliente (Web y Móvil) y los procesos transversales del sistema. Su responsabilidad principal es gestionar las peticiones HTTP relacionadas con las preferencias del usuario y procesar de forma segura las interacciones con los proveedores de pago externos, incluyendo la recepción vital de eventos asíncronos (Webhooks).

Basándose en las entidades y contratos definidos en el dominio, esta capa expone los siguientes controladores RESTful y componentes:

**REST Controllers:**
* **`SettingsController`:** Constituye el punto de entrada para la personalización de la experiencia del usuario. Expone endpoints para consultar la configuración actual, actualizar preferencias de visualización (como el tema oscuro/claro o el idioma base), y modificar los permisos de notificaciones u otras métricas operativas.
* **`PaymentsController`:** Maneja el flujo de transacciones financieras desde la perspectiva del cliente. Expone rutas para generar intenciones de pago (Payment Intents), gestionar la tokenización de métodos de pago de forma segura (sin exponer datos de tarjetas al backend) y consultar el estado histórico de una transacción.
* **`PaymentWebhooksController`:** Un controlador crítico y especializado en escuchar los eventos asíncronos (callbacks) enviados directamente por el proveedor externo de pagos (ej. Stripe, PayPal o Niubiz). Su responsabilidad es validar las firmas criptográficas de las peticiones entrantes para confirmar eventos de éxito, fallo o reembolso, delegando luego la actualización del estado al sistema.

**Data Transfer Objects (DTOs / Resources):**
Para mantener el aislamiento estructural y asegurar que la información de la pasarela y las configuraciones no expongan el modelo de dominio interno, se implementan los siguientes contratos de datos:
* **Request Resources:** Clases como `UpdateUserSettingResource` o `CreatePaymentIntentResource`, encargadas de encapsular los datos enviados por el cliente y ejecutar validaciones de formato mediante Data Annotations antes de que la petición ingrese a la capa de aplicación.
* **Response Resources:** Clases como `SettingResponse` y `PaymentTransactionResponse`, que estructuran y filtran los datos de salida, asegurando que el frontend reciba exactamente la información necesaria para renderizar la interfaz o procesar el flujo de caja.

#### 2.6.4.3. Application Layer

La capa de aplicación (Application Layer) en el Bounded Context de **App Management** actúa como el orquestador central de los casos de uso relacionados con las preferencias del sistema y la integración de pagos. Su función principal es recibir las solicitudes desde la capa de interfaz, interactuar con los repositorios y servicios de dominio para aplicar las reglas de negocio, y delegar la ejecución técnica de las transacciones financieras a los servicios de infraestructura externos.

Para garantizar un código mantenible y altamente cohesivo, esta capa implementa el patrón CQRS (Command and Query Responsibility Segregation), dividiendo el flujo en operaciones de lectura y escritura:

**Commands (Operaciones de Escritura) y Command Handlers:**
Encapsulan las solicitudes que mutan el estado de las configuraciones o inician y procesan transacciones financieras. Los servicios encargados orquestan el flujo transaccional:
* **`SettingsCommandService` / Handlers:** Orquesta casos de uso para la personalización de la experiencia mediante comandos como `CreateDefaultSettingsCommand` (ejecutado al registrar un nuevo usuario) y `UpdateUserSettingCommand` (para modificar preferencias de idioma, temas o notificaciones).
* **`PaymentCommandService` / Handlers:** Gestiona el ciclo de vida de los pagos mediante comandos como `CreatePaymentIntentCommand` (que orquesta la creación de una intención de pago a través de los contratos del dominio) y `SavePaymentMethodCommand` (para asociar de forma segura un token de tarjeta al usuario).
* **`PaymentWebhookCommandService` / Handlers:** Un orquestador crítico que procesa eventos asíncronos recibidos desde el exterior. Mediante el `ProcessWebhookEventCommand`, recibe la confirmación de la pasarela de pagos (éxito, fallo o fraude) y actualiza el estado transaccional interno, actuando como puente seguro entre el proveedor externo y el núcleo del sistema.

**Queries (Operaciones de Lectura) y Query Handlers:**
Encapsulan las solicitudes de información, optimizando la lectura de datos sin generar efectos secundarios en el sistema:
* **`SettingsQueryService` / Handlers:** Resuelve consultas como `GetUserSettingsByUserIdQuery`, permitiendo a la interfaz de usuario cargar rápidamente las preferencias visuales y de localización en el arranque de la aplicación.
* **`PaymentQueryService` / Handlers:** Atiende solicitudes como `GetTransactionStatusByIdQuery` y `GetUserPaymentMethodsQuery`, brindando a los clientes un historial claro de sus transacciones y métodos de pago guardados (tokenizados).

Mediante esta arquitectura, la capa de aplicación coordina eficientemente la integración con pasarelas de pago y la gestión de configuraciones, asegurando que el núcleo de **Splitly** permanezca completamente agnóstico de las librerías o SDKs de proveedores de terceros (como Stripe o PayPal), delegando dicha complejidad técnica a la capa de infraestructura.

#### 2.6.4.4 Infrastructure Layer

La capa de infraestructura (Infrastructure Layer) para el Bounded Context de **App Management** es la responsable de proporcionar las implementaciones tecnológicas concretas para los contratos y abstracciones definidos en la capa de dominio. En este módulo en particular, su rol es doblemente crítico: gestionar la persistencia de las configuraciones y actuar como una Capa Anticorrupción (Anti-Corruption Layer - ACL) física frente a los proveedores de pagos externos.

Los componentes técnicos que estructuran esta capa se dividen de la siguiente manera:

**Persistencia de Datos y ORM:**
Al igual que en los demás Bounded Contexts, la persistencia se gestiona mediante Entity Framework Core (EF Core), utilizando un contexto de base de datos (`DbContext`) delimitado para aislar estas operaciones:
* **Mapeo de Entidades:** Se configuran las reglas de mapeo (Fluent API) para las tablas de configuraciones (`user_settings`) y el registro histórico de transacciones (`payment_transactions`).
* **Seguridad y Cumplimiento:** A nivel de configuración de base de datos, se asegura que la tabla de métodos de pago (`payment_methods`) únicamente almacene identificadores o *tokens* provistos por la pasarela de pagos, garantizando el cumplimiento de normativas de seguridad (como PCI-DSS) al no guardar nunca datos sensibles de tarjetas de crédito o débito.

**Implementación de Repositorios:**
Se proveen las clases concretas que implementan las interfaces del dominio:
* **`UserSettingRepository`:** Implementa la lógica SQL/LINQ para consultar y modificar las preferencias de visualización, notificaciones y localización de cada usuario.
* **`PaymentTransactionRepository`:** Encargado de registrar en la base de datos local cada intento de pago, actualizando su estado (ej. de *Pending* a *Succeeded*) conforme los *webhooks* confirman los resultados.

**Integración con Servicios Externos (Payment Gateway Adapters):**
Esta es la sección más crítica de la infraestructura de este módulo, ya que encapsula los SDKs y las librerías de terceros (ej. Stripe.net, PayPal SDK o Niubiz):
* **`StripePaymentGatewayAdapter` (o equivalente):** Es la clase concreta que implementa la interfaz `IPaymentGatewayService` del dominio. Su responsabilidad es traducir los comandos del sistema interno (como "Cobrar 50 Soles") al formato y las llamadas HTTP específicas que exige la API del proveedor de pagos. 
* Si en el futuro **Splitly** decide cambiar de pasarela de pagos (por ejemplo, migrar de Stripe a PayPal), los cambios tecnológicos se limitarán exclusivamente a crear un nuevo adaptador en esta capa, sin que la capa de dominio o de aplicación sufran la más mínima alteración.

#### 2.6.4.5. Bounded Context Software Architecture Component Level Diagrams

El siguiente diagrama a nivel de componentes ilustra la arquitectura de software interna del Bounded Context de **App Management**. Esta representación visual demuestra cómo los sub-dominios transversales (Settings y Payment Gateway) se estructuran respetando los principios de Clean Architecture y el Modelo C4, aislando la complejidad técnica del proveedor de pagos.

El diagrama detalla el flujo de control y las dependencias a través de las cuatro capas principales, destacando el ciclo de vida de las transacciones financieras:
* **Interface Layer:** Expone los endpoints de la API REST para las configuraciones y actúa como receptor asíncrono (`PaymentWebhooksController`) para los eventos enviados por el procesador de pagos.
* **Application Layer:** Orquesta los casos de uso a través de servicios dedicados, procesando la intención de los usuarios y desencriptando/validando los eventos (webhooks) recibidos desde el exterior.
* **Domain Layer:** El núcleo agnóstico del Bounded Context, donde residen entidades críticas como `UserSetting` y `PaymentIntent`, modelando el estado de la transacción sin acoplarse a SDKs externos.
* **Infrastructure Layer:** Implementa la Capa Anticorrupción (ACL) mediante el `PaymentGatewayAdapter`, el cual traduce las directivas del dominio en llamadas HTTP a la **External Payment Gateway** (ej. Stripe o PayPal). Adicionalmente, maneja la persistencia en la **Base de Datos Relacional** mediante Entity Framework Core, garantizando que no se almacene información sensible (PCI-DSS).

Esta arquitectura asegura un flujo circular robusto: la infraestructura inicia los cobros, y la pasarela externa confirma el resultado enviando *webhooks* de vuelta a la capa de interfaz.

![Diagrama de componentes App Management](images/BC%20App%20-%20diagrama%20-%20componentes.png)

### 2.6.4.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.4.6.1. Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio ilustra el modelo conceptual diseñado para el Bounded Context de **App Management**. Este esquema visualiza las entidades y Aggregate Roots responsables de gestionar la infraestructura transversal de la aplicación, incluyendo las preferencias del usuario y la integración con las pasarelas de pago.

El modelo se divide en dos enfoques principales:
* Por un lado, `UserSetting` actúa como un Aggregate Root aislado que centraliza la personalización de la experiencia del usuario (idioma, tema visual y notificaciones).
* Por otro lado, se definen los elementos del sub-dominio de pagos, donde `PaymentIntent` (Aggregate Root) orquesta el ciclo de vida de una transacción financiera, y se relaciona de manera segura con `PaymentMethodProfile`. Esta última entidad es crítica para la seguridad (cumplimiento PCI-DSS), ya que únicamente almacena el token externo (`ExternalToken`) provisto por el proveedor de pagos, en lugar de los datos sensibles de la tarjeta.

El diseño asegura que la lógica de cobros y configuraciones permanezca fuertemente tipada a través de enumeradores como `TransactionStatus` y `ThemePreference`, manteniendo el dominio limpio de implementaciones tecnológicas específicas.

![Diagrama de clases App Management](images/app%20%20BC%20-%20diagrama%20contexto.png)

#### 2.6.4.6.2. Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos estructurado para el Bounded Context de **App Management**. Este esquema aísla las tablas responsables de almacenar las preferencias transversales de la aplicación y el registro histórico de la interacción con la pasarela de pagos.

En el diagrama se observan tres tablas principales, todas fuertemente vinculadas al identificador del usuario (delegado del módulo IAM):
* **`user_settings`**: Almacena las preferencias de localización y experiencia visual (idioma, tema y notificaciones).
* **`payment_transactions`**: Funciona como un registro auditable de los intentos de cobro, guardando el monto, la moneda, el estado de la transacción y, de forma crucial, el `external_transaction_id` que permite la conciliación con el proveedor externo (ej. Stripe).
* **`payment_methods`**: Almacena los perfiles de pago del usuario cumpliendo con los estándares de seguridad (PCI-DSS). No guarda datos sensibles, sino únicamente el `external_token` provisto por la pasarela y los últimos 4 dígitos de la tarjeta (`card_last_4`) para fines de visualización en la interfaz.

Este diseño asegura que el núcleo del negocio esté completamente separado de la configuración técnica y de los detalles de infraestructura de cobros.

![Diagrama de base de datos App Management](images/base%20de%20datos%20-%20diagrama%20-%20app%20BC.png)