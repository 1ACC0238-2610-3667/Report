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


### 2.5.1.2. Domain Message Flows Modeling
### 2.5.1.3. Bounded Context Canvases
## 2.5.2. Context Mapping
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
