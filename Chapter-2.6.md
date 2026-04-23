## 2.6. Tactical-Level Domain-Driven Design

## 2.6. Bounded Contexts

### 2.6.1. Bounded Context: Identity and Access Management (IAM)

Este contexto delimitado es de alcance global y de naturaleza técnica. Su responsabilidad es gestionar la identidad de los usuarios registrados en Splitly y proporcionar los mecanismos de autenticación y autorización mediante tokens, abstrayéndose completamente de la lógica de negocio de la distribución de gastos.

#### 2.6.1.1. Domain Layer (Model)

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