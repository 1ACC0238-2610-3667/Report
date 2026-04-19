# 2.5. Strategic-Level Domain-Driven Design
## 2.5.1. EventStorming
### 2.5.1.1. Candidate Context Discovery
Para esta etapa se llevó a cabo una sesión, la sesión tuvo una duración aproximada de 90 minutos y permitió identificar los bounded contexts del sistema Splitly. Durante el proceso se aplicaron las técnicas start-with-value, start-with-simple y look-for-pivotal-events, que facilitaron la agrupación de eventos y entidades según su afinidad y valor para el negocio.

Como resultado, se identificaron cuatro bounded contexts:

Identity and Access Management: administración de usuarios, autenticación y control de accesos.
Contributions Distribution: manejo y division de gastos por miembro de hogar
- Bills
- Contributions
- Members Contribution

Household Management: manejo de integrantes de grupo de hogar
 - HouseholdMembers
 - Households
 - Invitations

App Management: manejo de ajustes dentro de la aplicacion
 - Settings
 - Payment Gateway

Link: https://miro.com/app/board/uXjVGgNmWGI=/?share_link_id=935627302895

<br>
<img src="assets/ASE-CandidateContextDiscovery.jpg" alt="CandidateContextDiscovery">
<br>


### 2.5.1.2. Domain Message Flows Modeling

En esta etapa se desarrolló el modelado de flujos de mensajes de dominio (Domain Message Flows) con el objetivo de visualizar cómo colaboran los bounded contexts identificados en el Candidate Context Discovery para resolver los principales casos de negocio del sistema Splitly.

Para la construcción de estos flujos se aplicó la técnica de Domain Storytelling, la cual permite describir las interacciones en un lenguaje natural, mostrando cómo un evento generado en un bounded context desencadena comandos o nuevos eventos en otros contextos. De este modo se logra una visión clara de la cooperación entre módulos y del ciclo de vida de la información dentro de la plataforma

**Historias de dominio (Domain Stories)**

 1. **Identity and Access Management:**
- Cuando un usuario se registra en **Identity and Access Management**, se crea la cuenta y se validan sus credenciales de acceso. Una vez autenticado, este contexto habilita la sesión del usuario y permite que otros bounded contexts accedan a la información básica de identidad.
- Cuando **App Management** necesita consultar o actualizar configuraciones relacionadas con la cuenta, solicita la información al contexto **Identity and Access Management**, el cual valida la autenticidad del usuario antes de procesar la solicitud.
- Además, cuando un usuario inicia sesión exitosamente, el contexto de identidad habilita el acceso a las funcionalidades disponibles según el **rol asignado**, ya sea **Household Representative** o **Household Member**.

 2. **Contributions Distribution:**
- Cuando un **Household Representative** crea un hogar en **Household Management**, se registra la información del grupo y se asocia al usuario creador como administrador del hogar.
- Posteriormente, el representante puede enviar invitaciones a nuevos integrantes. Cuando una invitación es aceptada, el sistema registra al usuario como **Household Member** dentro del hogar correspondiente.
- Una vez actualizado el listado de integrantes, **Household Management** pone esta información a disposición de **Contributions Distribution**, permitiendo que los gastos se distribuyan entre los miembros registrados.

 3. **Household Management:**
- Cuando se registra una cuenta en el módulo **Bills** dentro de **Contributions Distribution**, se genera una nueva contribución asociada al **hogar correspondiente**.
- Luego, el módulo **Contributions** calcula cómo se dividirá el gasto entre los miembros del hogar, generando los registros individuales en **Member Contributions**.
- Cada contribución individual representa el monto que debe asumir cada integrante y se asigna utilizando la información de miembros proporcionada por **Household Management**.
- Cuando se actualiza una contribución, el sistema recalcula los montos pendientes y mantiene actualizado el estado de las obligaciones de cada miembro.

 4. **App Management:**
- Cuando un usuario modifica configuraciones dentro de **App Management**, el sistema actualiza sus preferencias en el módulo **Settings**, incluyendo ajustes relacionados con la cuenta o preferencias de uso.
- Si la configuración implica métodos de pago o procesamiento de cobros, **App Management** utiliza el módulo **Payment Gateway** para gestionar la operación y registrar la información correspondiente.
- Asimismo, **App Management** consulta a **Identity and Access Management** para validar permisos antes de permitir cambios sensibles en la configuración del usuario.

<br>
<img src="assets/PlantUML.png" alt="DomainMessageFlowsModeling">
<br>

### 2.5.1.3. Bounded Context Canvases
En esta sección se desarrollaron los Bounded Context Canvases de Splitly. El propósito fue delimitar con precisión las responsabilidades, el lenguaje ubicuo y las decisiones de negocio, además de explicitar las comunicaciones (Queries, Commands y Events) y los colaboradores (otros BC, sistemas externos y frontend).

Cada canvas documenta:

- Descripción
- Clasificación estratégica (core, supporting, generic)
- Rol de dominio (draft, execution, analysis, gateway)
- Inbound/Outbound communication
- Lenguaje ubicuo
- Decisiones de negocio
- Colaboradores

Esta definición establece el ownership de los datos, reduce ambigüedades y prepara los contratos de integración que se implementarán en APIs y mensajería.

## 2.5.2. Context Mapping

En la etapa de Context Mapping del sistema Splitly, se identificaron diversos patrones de relación entre bounded contexts propuestos por Domain-Driven Design (DDD), con el objetivo de definir la manera en que los distintos contextos delimitados interactúan entre sí manteniendo la autonomía de sus modelos de dominio.

Los principales patrones identificados fueron:

- Customer-Supplier
- Partnership
- Anti-Corruption Layer
- Open Host Service
- Shared Kernel (para identificadores compartidos)

Estos patrones permitieron modelar adecuadamente las dependencias y colaboraciones entre los bounded contexts de Identity and Access Management, Household Management, Contributions Distribution y App Management.

**CUSTOMER-SUPPLIER**

El patrón Customer-Supplier se aplicó en relaciones donde un bounded context depende de otro para obtener información necesaria para sus procesos.

En Splitly, este patrón se presenta en:

- Household Management → Contributions Distribution
- Identity and Access Management → App Management

En el primer caso, Contributions Distribution utiliza la información de hogares y miembros proporcionada por Household Management para realizar la división de gastos.
En el segundo, App Management depende de Identity and Access Management para acceder a la información del usuario y administrar configuraciones relacionadas con la cuenta.

**PARTNERSHIP**

El patrón Partnership se identificó dentro del bounded context Contributions Distribution, en la relación entre:

- Bills
- Contributions
- Member Contributions

Estos subdominios trabajan de manera coordinada en la distribución de gastos: al registrarse una cuenta, se generan las contribuciones y luego se asignan las contribuciones individuales a cada miembro.
Debido a esta dependencia operativa, mantienen una colaboración estrecha bajo este patrón.

**ANTI-CORRUPTION LAYER**

El patrón Anti-Corruption Layer (ACL) se implementó para evitar el acoplamiento directo entre bounded contexts y proteger la integridad de cada modelo de dominio.

Esta capa permite traducir la información entre contextos sin exponer directamente sus estructuras internas, facilitando la independencia y evolución de cada bounded context.

**OPEN HOST SERVICE**

El patrón Open Host Service se aplicó en Identity and Access Management, ya que este bounded context expone servicios de autenticación y acceso consumidos por otros contextos mediante interfaces definidas.

Estos servicios son utilizados principalmente por App Management, que requiere acceder a la información del usuario para administrar configuraciones dentro de la aplicación.

## 2.5.3. Software Architecture
### 2.5.3.1. Software Architecture Context Level Diagrams
<br>
<img src="assets/HouseholdContext.png" alt="ContextDiagram">
<br>

### 2.5.3.2. Software Architecture Container Level Diagrams

<br>
<img src="assets/ContainerDiagram.png" alt="ContainerDiagram">
<br>

### 2.5.3.3. Software Architecture Deployment Diagrams

<br>
<img src="assets/DeploymentDiagram.png" alt="DeploymentDiagram">
<br>
