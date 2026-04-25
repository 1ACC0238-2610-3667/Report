<p align="center">
    <img src="./assets/logo-upc.png" alt="upc-logo" width="80px" height="80px"/>
</p>

<h1 align="center">
    Universidad Peruana de Ciencias Aplicadas
</h1>

<h3 align="center">
    Carrera: Ingeniería de Software
    <br> <br>
    Curso: 1ACC0238 - Aplicaciones para Dispositivos Móviles
    <br> <br>
    Sección: 3667
    <br> <br>
    Profesor: Eduardo Martin Reyes Rodriguez
    <br> <br>
    Ciclo: 2026-01
    <br> <br>
    Informe de Trabajo Final
    <br> <br>
    Startup: GroupFund
    <br> <br>
    Producto: Splitly  
</h3>

<div align="center">

| <div style="width:300px">Alumno</div>       | <div style="width:125px">Código</div> |
|:-------------------------------------------:|:-------------------------------------:|
|  Martínez Valdivia, José Luis               |              u202213989               |
|       Ríos Pacheco, Héctor Javier           |              u20231c540               |
| Cuentas Peña, JoaquinAlberto                |              u20201f788               |
|       Ramirez Escalante, Walter Luis        |              u202221632               |
|       Miraval Pomalaya, Rodrigo Jesús       |              u202311082               |

</div>

<div align="center"> Abril 2026 </div>


## Registro de Versiones del Informe
| Versión | Fecha      | Autor(es)      | Descripción de modificación       |
| ------- | ---------- | -------------------------------------------------------- | --------- |
| 0.1     | 22/04/2026 |            |         |



## Project Report Collaboration Insights  
**TB1**

# Tabla de Contenidos

- Capítulo I: Introducción  
  - [1.1 Startup Profile](#11-startup-profile)  
    - [1.1.1 Descripción de la Startup](#111-descripcion-de-la-startup)  
    - [1.1.2 Perfiles de integrantes del equipo](#112-perfiles-de-integrantes-del-equipo)  
  - [1.2 Solution Profile](#12-solution-profile)  
    - [1.2.1 Antecedentes y problemática](#121-antecedentes-y-problematica)  
    - [1.2.2 Lean UX Process](#122-lean-ux-process)  
      - [1.2.2.1 Lean UX Problem Statements](#1221-lean-ux-problem-statements)  
      - [1.2.2.2 Lean UX Assumptions](#1222-lean-ux-assumptions)  
      - [1.2.2.3 Lean UX Hypothesis Statements](#1223-lean-ux-hypothesis-statements)  
      - [1.2.2.4 Lean UX Canvas](#1224-lean-ux-canvas)  
  - [1.3 Segmentos objetivo](#13-segmentos-objetivo)  

- Capítulo II: Requirements Development and Software Solution Design  
  - [2.1 Competidores](#21-competidores)  
    - [2.1.1 Análisis competitivo](#211-analisis-competitivo)  
    - [2.1.2 Estrategias y tácticas frente a competidores](#212-estrategias-y-tacticas-frente-a-competidores)  

  - [2.2 Entrevistas](#22-entrevistas)  
    - [2.2.1 Diseño de entrevistas](#221-diseno-de-entrevistas)  
    - [2.2.2 Registro de entrevistas](#222-registro-de-entrevistas)  
    - [2.2.3 Análisis de entrevistas](#223-analisis-de-entrevistas)  

  - [2.3 Needfinding](#23-needfinding)  
    - [2.3.1 User Personas](#231-user-personas)  
    - [2.3.2 User Task Matrix](#232-user-task-matrix)  
    - [2.3.3 User Journey Mapping](#233-user-journey-mapping)  
    - [2.3.4 Empathy Mapping](#234-empathy-mapping)  
    - [2.3.5 Big Picture EventStorming](#235-big-picture-eventstorming)  
    - [2.3.6 Ubiquitous Language](#236-ubiquitous-language)  

  - [2.4 Requirements Specification](#24-requirements-specification)  
    - [2.4.1 User Stories](#241-user-stories)  
    - [2.4.2 Impact Mapping](#242-impact-mapping)  
    - [2.4.3 Product Backlog](#243-product-backlog)  

  - [2.5 Strategic-Level Domain-Driven Design](#25-strategic-level-domain-driven-design)  
    - [2.5.1 EventStorming](#251-eventstorming)  
      - [2.5.1.1 Candidate Context Discovery](#2511-candidate-context-discovery)  
      - [2.5.1.2 Domain Message Flows Modeling](#2512-domain-message-flows-modeling)  
      - [2.5.1.3 Bounded Context Canvases](#2513-bounded-context-canvases)  
    - [2.5.2 Context Mapping](#252-context-mapping)  
    - [2.5.3 Software Architecture](#253-software-architecture)  
      - [2.5.3.1 Software Architecture Context Level Diagrams](#2531-software-architecture-context-level-diagrams)  
      - [2.5.3.2 Software Architecture Container Level Diagrams](#2532-software-architecture-container-level-diagrams)  
      - [2.5.3.3 Software Architecture Deployment Diagrams](#2533-software-architecture-deployment-diagrams)  

  - [2.6 Tactical-Level Domain-Driven Design](#26-tactical-level-domain-driven-design)  
    - [2.6.x Bounded Context](#26x-bounded-context)  
      - [2.6.x.1 Domain Layer](#26x1-domain-layer)  
      - [2.6.x.2 Interface Layer](#26x2-interface-layer)  
      - [2.6.x.3 Application Layer](#26x3-application-layer)  
      - [2.6.x.4 Infrastructure Layer](#26x4-infrastructure-layer)  
      - [2.6.x.5 Component Level Diagrams](#26x5-component-level-diagrams)  
      - [2.6.x.6 Code Level Diagrams](#26x6-code-level-diagrams)  
        - [2.6.x.6.1 Domain Layer Class Diagrams](#26x61-domain-layer-class-diagrams)  
        - [2.6.x.6.2 Database Design Diagram](#26x62-database-design-diagram)  

- Capítulo III: Solution UI/UX Design  
  - [3.1 Product Design](#31-product-design)  
    - [3.1.1 Style Guidelines](#311-style-guidelines)  
      - [3.1.1.1 General Style Guidelines](#3111-general-style-guidelines)  

    - [3.1.2 Information Architecture](#312-information-architecture)  
      - [3.1.2.1 Organization Systems](#3121-organization-systems)  
      - [3.1.2.2 Labelling Systems](#3122-labelling-systems)  
      - [3.1.2.3 SEO Tags and Meta Tags](#3123-seo-tags-and-meta-tags)  
      - [3.1.2.4 Searching Systems](#3124-searching-systems)  
      - [3.1.2.5 Navigation Systems](#3125-navigation-systems)  

    - [3.1.3 Landing Page UI Design](#313-landing-page-ui-design)  
      - [3.1.3.1 Landing Page Wireframe](#3131-landing-page-wireframe)  
      - [3.1.3.2 Landing Page Mock-up](#3132-landing-page-mock-up)  

    - [3.1.4 Mobile Applications UX/UI Design](#314-mobile-applications-uxui-design)  
      - [3.1.4.1 Mobile Applications Wireframes](#3141-mobile-applications-wireframes)  
      - [3.1.4.2 Mobile Applications Wireflow Diagrams](#3142-mobile-applications-wireflow-diagrams)  
      - [3.1.4.3 Mobile Applications Mock-ups](#3143-mobile-applications-mock-ups)  
      - [3.1.4.4 Mobile Applications User Flow Diagrams](#3144-mobile-applications-user-flow-diagrams)  
      - [3.1.4.5 Mobile Applications Prototyping](#3145-mobile-applications-prototyping)  

- Capítulo IV: Product Implementation & Validation  
  - [4.1 Software Configuration Management](#41-software-configuration-management)  
    - [4.1.1 Software Development Environment Configuration](#411-software-development-environment-configuration)  
    - [4.1.2 Source Code Management](#412-source-code-management)  
    - [4.1.3 Source Code Style Guide & Conventions](#413-source-code-style-guide--conventions)  
    - [4.1.4 Software Deployment Configuration](#414-software-deployment-configuration)  

  - [4.2 Landing Page & Mobile Application Implementation](#42-landing-page--mobile-application-implementation)  
    - [4.2.1 Sprint n](#421-sprint-n)  
      - [4.2.1.1 Sprint Planning n](#4211-sprint-planning-n)  
      - [4.2.1.2 Sprint Backlog n](#4212-sprint-backlog-n)  
      - [4.2.1.3 Development Evidence for Sprint Review](#4213-development-evidence-for-sprint-review)  
      - [4.2.1.4 Testing Suite Evidence for Sprint Review](#4214-testing-suite-evidence-for-sprint-review)  
      - [4.2.1.5 Execution Evidence for Sprint Review](#4215-execution-evidence-for-sprint-review)  
      - [4.2.1.6 Services Documentation Evidence](#4216-services-documentation-evidence)  
      - [4.2.1.7 Software Deployment Evidence](#4217-software-deployment-evidence)  
      - [4.2.1.8 Team Collaboration Insights](#4218-team-collaboration-insights)  

  - [4.3 Validation Interviews](#43-validation-interviews)  
    - [4.3.1 Diseño de entrevistas](#431-diseno-de-entrevistas)  
    - [4.3.2 Registro de entrevistas](#432-registro-de-entrevistas)  
    - [4.3.3 Evaluaciones según heurísticas](#433-evaluaciones-segun-heuristicas)  

- [Conclusiones](#conclusiones)  
- [Conclusiones y recomendaciones](#conclusiones-y-recomendaciones)  
- [Video App Validation](#video-app-validation)  
- [Video About the Product](#video-about-the-product)  
- [Video About the Team](#video-about-the-team)  



**ABET – EAC - Student Outcome 7**

La capacidad de adquirir y aplicar nuevos
conocimientos según sea necesario,
utilizando estrategias de aprendizaje
apropiadas.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo,
que permiten sustentar el haber alcanzado el logro del ABET – EAC - Student Outcome 7.


| Criterio específico | Acciones realizadas | Conclusiones |
| :--- | :--- | :--- |
| **Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.** |  **Héctor Rios:** Contribuí realizando el capítulo 1 y organizando las ideas para la continuación del proyecto <br><br> **Jose Luis Martínez Valdivia:** Contribui en El desarrollo del capitulo 2 - Strategic Level Domain Driven Design <br><br> **Joaquin Alberto Cuentas Peña:** Contribuí en El desarrollo del capítulo 2 – con el análisis de segmentos objetivos, entrevistas y elaboración de personas <br><br> **Walter Luis Fajardo Monrroy:** Contribuí en el desarrollo de diagramas, así como segmentación de bounded context  <br><br>|    **Héctor Rios** **TB1:** El desarrollo del capítulo 1 me permitió reforzar mis conocimientos sobre la estructura inicial de un proyecto de software. Sentí que este proceso me ayudó a entender mejor cómo plantear una base sólida, lo cual considero clave para mi crecimiento profesional. <br><br>   <br><br> **Jose Luis Martínez Valdivia:** El desarrollo del capitulo 2 me permitió comentar y enriquecer mis conocimientos de DDD y la forma en la que se debaten ideas para implementar una solución de Servicio Web <br><br> **Joaquin Alberto Cuentas Peña:** El desarrollo de este capítulo me permitió conocer la perspectiva de los usuarios que usarán la aplicación. <br><br>  **Walter Luis Fajardo Monrroy:** El desarrollo de este capítulo permitirá a los desarrolladores asignar los bounded context y hacer consultas de funcionamiento e interconexión. <br><br>|
| **Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones detecnologías de ingeniería de software** | **Héctor Rios:** Contribuí realizando el capítulo 1,sedimentando las bases del proyecto <br><br> **Jose Luis Martínez Valdivia:** Contribui en El desarrollo del capitulo 2 - Strategic Level Domain Driven Design <br><br> **Joaquin Alberto Cuentas Peña:** Reconocí las necesidades de los usuarios a través de entrevistas, así como sus gustos y molestias <br><br> **Walter Luis Fajardo Monrroy:** Reconocí segmentos, funcionalidades y los convertí en bounded context para desarrollo  <br><br>| **Héctor Rios** **TB1:** A lo largo del desarrollo del capítulo 1, comprendí que siempre hay aspectos que mejorar y aprender. Esta experiencia me hizo reflexionar sobre la importancia de mantenerme en constante actualización para poder aportar mejor en futuros proyectos. <br><br> **Jose Luis Martínez Valdivia:** Durante El desarrollo de capitulo 2, logre entender los procesos y requerimientos que se deben llevar acabo para poder delimitar el alcance y arquitectura de desarrollo del proyecto a implementar <br><br> **Joaquin Alberto Cuentas Peña: :** Este conocimiento me permitió hacer un análisis y crear personas para enfocarnos en posibles requisitos funcionales <br><br> **Walter Luis Fajardo Monrroy:** El desarrollo de este capítulo me permitió aprender como segmentar bounded context en el contexto de desarrollo móvil <br><br>|


## Objetivos SMART

## Capítulo I: Introducción

## 1.1 Startup Profile

### 1.1.1 Descripción de la Startup

**GroupFund** es una empresa emergente del sector tecnológico dedicada a desarrollar soluciones innovadoras para la gestión financiera en entornos de convivencia. Su producto principal, **Splitly**, está diseñado para facilitar la organización y distribución equitativa de los gastos compartidos del hogar, considerando los ingresos de cada miembro.  

A través de un sistema digital automatizado, claro y accesible, Splitly fomenta la responsabilidad económica, la comunicación eficaz y la adecuada gestión del presupuesto común, reduciendo conflictos y fortaleciendo una cultura de colaboración dentro del hogar.

**Título:** Splitly  

**Misión:** Brindar un manejo eficiente de las finanzas compartidas mediante una solución orientada a dispositivos móviles que distribuye los gastos de forma proporcional a los ingresos de cada integrante, fomentando la equidad, la claridad y una convivencia armoniosa.

**Visión:** Convertirse en la plataforma líder en la gestión financiera compartida en los hogares, reconocida por empoderar a las personas para tomar decisiones económicas justas, responsables y colaborativas. 

**Principios:** Transparencia, justicia y colaboración. 

### 1.1.2 Perfiles de integrantes del equipo

| Integrante | Descripción Personal | Conocimientos Técnicos |
|-------------|----------------------|-------------------------|
| **José Luis Martínez Valdivia - u202213989** <br> <img src="assets/integrantes/FOTO_JOSE.jpg" alt="foto-jose" width="170px"/> | Soy una persona responsable, comprometida con mis objetivos y con gran disposición para aprender continuamente. Me adapto con facilidad al trabajo en equipo, aportando ideas y soluciones. Valoro mucho la eficiencia, la ética profesional y la mejora constante. Me esfuerzo por entregar siempre resultados de calidad, gestionando mis tareas con orden y enfoque.      | Desarrollador de resolución de problemas de .NET con experiencia en C#, JavaScript, TypeScript, C++, HTML CSS. Además de .NET, .Net Core, Angular, React.Trabajo bien tanto individualmente como en un ambiente de equipo.         |
| **Héctor Javier Rios Pacheco - u20231c540**<br> <img src="assets/integrantes/FotoHector.png" alt="foto-hector" width="170px"/>   |  Soy responsable, me gusta involucrarme activamente en los proyectos, aportar ideas útiles y cumplir con mis tareas a tiempo. Siempre estoy dispuesto a colaborar y ayudar al equipo a avanzar de la mejor manera posible.     |  Cuento con formación en desarrollo de software, incluyendo estructuras de datos, algoritmos y arquitecturas orientadas a servicios. Trabajo con lenguajes como Java, TypeScript, JavaScript, HTML5 y CSS3, y utilizo herramientas y frameworks como Angular, Spring Boot, Git/GitHub, Swagger y bases de datos relacionales.       |
| **Joaquin Alberto Cuentas Peña - u20201f788**<br> <img src="assets/integrantes/fotojoaquin.jpg" alt="foto-joaquin" width="170px"/>|   Soy responsable, me gusta aprender cosas nuevas y apoyar a mis compañeros cuando lo necesitan. Siempre estoy dispuesto a desafiarme y a desafiar a mis compañeros para sacar lo mejor de nosotros    |   Mi experiencia en desarrollo de software incluye conocimientos de algoritmos hasta estructuras de datos en distintos lenguajes como C++ y python. Asimismo he trabajado con tecnologías como angular, vue, flask y fast Appi. Me intereso en expandir mis conocimientos en backend.       |
| **Walter Luis Fajardo Monrroy - u202221632**<br> <img src="assets/integrantes/fotowalter.jpeg" alt="foto-walter" width="170px"/>   |   Soy un integrante comprometido y adaptable, apasionado por adquirir nuevos conocimientos que agreguen valor al proyecto. Priorizo el éxito del equipo brindando apoyo constante a mis compañeros, a quienes motivo a superar sus límites    |    Mi formación técnica abarca desde la lógica algorítmica hasta la gestión de estructuras de datos complejas en lenguajes como C++ y Rust. He trabajado en el ecosistema frontend con Svelte y Vue, complementando mi perfil con el manejo de herramientas como Go y NestJS     |
| **Rodrigo Jesús Miraval Pomalaya - u202311082**<br> <img src="assets/integrantes/FotoRodrigo.png" alt="foto-rodrigo" width="170px"/>    |  Mi nombre es Rodrigo Jesus Miraval Pomalaya y estudio Ingeniería de Software en la Universidad Peruana de Ciencias Aplicadas. Me considero una persona adaptable y detallista, siempre en busca de aprender y mejorar en lo que hago. Me gusta aplicar lo aprendido en proyectos académicos y trabajar en equipo, ya que compartir ideas no solo ayuda a obtener mejores resultados, sino también a ampliar mi visión en la carrera.       | Tengo conocimientos en Python, JavaScript, HTML y CSS, además de un nivel intermedio en SQL Server y MySQL.       |


## 1.2. Solution Profile

**Splitly**, producto desarrollado por **GroupFund**, es una solución integral compuesta por una aplicación móvil (nativa/multiplataforma) y un sitio web estático (Landing Page)l diseñada para facilitar la distribución equitativa de los gastos del hogar entre sus miembros, considerando los ingresos personales de cada individuo. La plataforma calcula automáticamente el aporte correspondiente de cada integrante, basándose en su situación económica, y garantiza así una distribución justa de los gastos compartidos como alquiler, servicios esenciales y alimentos.  

Técnicamente, la aplicación móvil aprovecha las capacidades del dispositivo para optimizar la experiencia del usuario: soporte de almacenamiento local, y acceso a recursos internos del dispositivo (como la cámara para registrar recibos y pagos realizados). Además, toda la lógica de negocio se integra de forma segura con un servicio RESTful de desarrollo interno, y se conecta a un servicio externo de terceros (pasarela de pagos) para procesar y validar las transferencias directamente desde la app.

Los usuarios pueden registrar sus ingresos, conocer cuánto deben contribuir y monitorear sus pagos, mientras que la persona responsable de la gestión del hogar obtiene una visión integral del proceso. Además, Splitly ofrece monitoreo en tiempo real, informes mensuales claros y alertas de pagos pendientes mediante notificaciones push en sus dispositivos.

Con una interfaz intuitiva y accesible, la aplicación no solo simplifica la gestión de las finanzas, sino que también promueve la transparencia, la confianza y la cooperación entre los integrantes del hogar, reduciendo posibles conflictos y asegurando un manejo económico eficaz y equilibrado.  

### 1.2.1. Antecedentes y Problemática

Enunciado del problema: La ausencia de un método equitativo para distribuir los gastos compartidos en pequeñas comunidades genera tensiones financieras y de convivencia entre sus integrantes.

Objetivos del Proyecto: Desarrollar una aplicación móvil que automaticen el cálculo de aportes proporcionales, faciliten la visibilidad de los gastos mediante servicios RESTful y permitan registrar y pagar deudas usando integración con APIs de terceros.

Restricciones: La solución móvil debe ser nativa o multiplataforma, implementando obligatoriamente almacenamiento local, uso de recursos del hardware (cámara) e integración con servicios de terceros y propios.

La metodología **5W y 2H** es un recurso utilizado para analizar la causa fundamental de un problema, error o discrepancia en los sistemas. Esta metodología, promovida por Toyota, constituye un pilar del Sistema de Producción Toyota (TPS). Según Taichii Ohno, permite comprender con claridad los problemas y facilita la implementación de acciones correctivas o preventivas (Palko et al., 2015). Asimismo, es un enfoque adaptable que puede aplicarse en diversos tipos de organizaciones, convirtiéndose en una herramienta valiosa para la resolución de disputas y la optimización de procesos.  


---

### What – ¿Cuál es la dificultad?

La cuestión central se encuentra en la ausencia de una repartición equitativa de los gastos en hogares con ingresos desiguales. Esto origina contribuciones desiguales que producen tensiones y posibles disputas entre los miembros, especialmente cuando se intenta repartir los gastos sin tener en cuenta la situación económica de cada individuo.

**¿Cuál es el vínculo con la persona mencionada?**  
El sistema tiene como objetivo que cada miembro pueda observar su contribución correspondiente desde su dispositivo móvil y cumplir con ella de forma equitativa. El responsable del hogar asume la tarea de supervisar el proceso y asegurar la igualdad en las aportaciones.

---

### When – ¿Cuándo ocurre el inconveniente?

La dificultad aparece principalmente en los momentos en que se deben pagar las facturas del hogar, las cuales suelen ser mensuales. Al repartir los gastos sin un cálculo justo, las discrepancias en los ingresos se hacen visibles y provocan problemas.

**¿Cuándo emplea el consumidor el artículo?**  
El producto se utiliza cada vez que se incurre en un gasto compartido, como servicios, alquiler, alimentos o compras en general. Al concluir cada mes, los usuarios pueden revisar desde la app el estado de los pagos efectuados y las deudas por saldar.

---

### Where – ¿Dónde ocurre?

**¿En qué lugar se encuentra el cliente al utilizar el producto?**  
EEl cliente suele estar en su casa o en cualquier lugar con conexión a Internet, mediante un dispositivo móvil.

**¿Hacia dónde se encamina?**  
El usuario ingresa al panel principal de la app móvil para examinar en detalle los gastos, las contribuciones que debe efectuar y los pagos pendientes.

**¿Cuál es el origen del problema?**  
El conflicto se origina en el hogar, cuando es necesario dividir los gastos compartidos (como luz, agua, alimentos, alquiler, etc.) y no se dispone de un método digital y accesible en todo momento que permita realizar esta división de manera equitativa y proporcional.

---

### Why – ¿Por qué ocurre?

La razón principal es la falta de un sistema claro y justo que facilite el cálculo de las contribuciones conforme a los ingresos de cada individuo. La ausencia de proporcionalidad provoca que algunos paguen más de lo que les corresponde y otros menos, generando descontento y disputas.

---

### Who – ¿Quiénes están involucrados?

**¿Quiénes están involucrados?**  
Los actores principales son los integrantes del hogar que comparten los costos, así como el encargado de gestionar dichos gastos.

**¿A quiénes les ocurre el problema?**  
Afecta a todas las personas que conviven y comparten responsabilidades financieras: familias, parejas o compañeros de vivienda con distintos niveles de ingresos.

**¿Quién hará uso de esto?**  
Todos los integrantes del hogar, ya que cada uno podrá revisar su aporte proporcional llevando el control en sus propios smartphones. El representante será responsable de planificar y supervisar la adecuada distribución de los gastos.

---

### How - ¿Cómo ocurre el problema?

#### ¿Cómo ocurre el problema?

La dificultad surge al momento de repartir los gastos compartidos (alquiler, servicios básicos, alimentos, entre otros) sin considerar un criterio proporcional a los ingresos de cada miembro, lo que provoca aportes desiguales.

#### ¿En qué condiciones los clientes usan nuestro producto?

Los usuarios recurrirán al producto cuando deseen calcular su aporte proporcional en los gastos del hogar o revisar cuánto han abonado y qué parte aún tienen pendiente de acuerdo con sus ingresos. Asimismo, podrán emplearlo para llevar un control más ordenado de las finanzas compartidas.

#### ¿Qué llevará a la persona a usar nuestro producto?

La persona recurrirá al producto ante la necesidad de dividir los gastos del hogar de manera justa, la falta de claridad en las aportaciones o el interés por prevenir conflictos financieros dentro de la convivencia. Del mismo modo, si desean consultar los montos pendientes de forma clara y en tiempo real, la inmediatez de una app móvil funcionará como una herramienta práctica.

<p align="center"><strong>Representación de costo promedio de errores en cálculos manuales - 2020</strong></p>
<p align="center">
  <img src="https://imgur.com/x2N1egQ.png" alt="Gráfico de errores manuales" width="500">
</p>
<p align="center">Fernando Blanco P. (2020). Gráfico de LDL – ESTADÍSTICA VISUAL (VIII). Gráficos con barras de error: manual de usuario – Lima, 2020</p>
<p align="center"><em>Figura: Representación visual del costo promedio de errores manuales.</em></p>

---

### How much - ¿Cúanto?

#### ¿Cuánto impacta en la convivencia y las finanzas no dividir equitativamente los gastos?

Genera tensiones, discusiones y desequilibrios económicos dentro del hogar, mientras que con la implementación de la aplicación se logra transparencia, justicia en las aportaciones y una mejor organización financiera compartida.

## 1.2.2 Lean UX Process

El Lean UX se define como un proceso en el que varios colaboradores trabajan juntos de manera continua y repetitiva, centrado en la experimentación y el aprendizaje constante. A diferencia de los métodos convencionales, este enfoque no se centra en la creación de una documentación detallada, sino que enfatiza la elaboración de prototipos y la ejecución de pruebas rápidas. Estas pruebas se realizan con usuarios auténticos y en situaciones específicas, lo que facilita la validación de hipótesis y la realización de cambios en el producto basados en la evidencia recopilada. Su propósito esencial es minimizar el desperdicio de recursos y optimizar la eficiencia en el ciclo de desarrollo, facilitando que los equipos de diseño y desarrollo puedan adaptarse con mayor agilidad a las demandas y expectativas de los usuarios (Gothelf & Seiden, 2013).

### 1.2.2.1 Lean UX Problem Statements

Los miembros de un mismo hogar con ingresos desiguales (como roommates, parejas o familias) enfrentan dificultades constantes al intentar dividir sus gastos compartidos de manera justa. Las herramientas tradicionales no consideran la capacidad adquisitiva real de cada integrante o no permiten una división rápida y auditable por el resto, lo que resulta en un sistema de cobro rígido.

Hemos observado que esta falta de proporcionalidad genera tensiones, desconfianza y conflictos domésticos entre los convivientes, afectando negativamente la organización económica del hogar. Al no contar con una plataforma accesible y transparente que refleje su realidad, los usuarios sienten que asumen cargas financieras injustas, lo que provoca desmotivación y un manejo ineficiente del presupuesto común.

¿Cómo podríamos desarrollar una aplicación móvil que automatice la distribución de los gastos del hogar de forma proporcional a los ingresos de cada integrante, facilitando el registro de recibos y el pago de cuotas, para fortalecer la equidad, la transparencia y la convivencia financiera?


### 1.2.2.2 Lean UX Assumptions

### Supuestos del Negocio – Splitly

1. **Creo que mis clientes tienen la necesidad de:**  
   Organizar, transparentar y distribuir equitativamente los gastos compartidos del hogar (alquiler, servicios, alimentos) basándose en los ingresos reales de cada miembro, para evitar tensiones financieras y conflictos de convivencia.

2. **Estas necesidades pueden resolverse con:**  
   Splitly, una solución digital conformada por una aplicación móvil, que calcula aportes proporcionales automáticamente, permite escanear recibos físicos usando la cámara del dispositivo, y facilita la liquidación de deudas mediante la integración con una pasarela de pagos de terceros.

3. **Mis clientes iniciales son (o serán):**  
   - Jóvenes profesionales y estudiantes universitarios que comparten departamento (roommates).  
   - Parejas jóvenes o familias con ingresos económicos dispares que buscan mayor transparencia financiera.

4. **El principal valor que un cliente quiere obtener de mi servicio es:**  
   Justicia financiera, transparencia y reducción drástica de las discusiones por dinero dentro del hogar.  
   **También pueden obtener estos beneficios adicionales:**  
   Ahorro de tiempo en cálculos manuales, recordatorios automáticos de pago (notificaciones push), y un historial claro y accesible del estado de las finanzas.

5. **Adquiriré la mayoría de mis clientes a través de:**  
   - Nuestro sitio web estático (Landing Page) optimizado para motores de búsqueda (SEO).  
   - Marketing digital en redes sociales dirigido a grupos demográficos jóvenes.  
   - Recomendaciones "boca a boca" e invitaciones directas enviadas desde la app por el representante del hogar hacia sus convivientes.

6. **Ganaré dinero mediante:**  
   - Modelo Freemium: acceso gratuito a las funciones de cálculo proporcional básico.     
   - Comisiones transaccionales derivadas de los pagos procesados a través de nuestra integración API con pasarelas de pago.

7. **Mi principal competencia en el mercado será:**  
   Aplicaciones genéricas de división de gastos, hojas de cálculo manuales (Excel) y la simple memoria o acuerdos informales.  
   **Superaremos a la competencia debido a:**  
   Nuestro algoritmo de cálculo enfocado estrictamente en la proporcionalidad de los ingresos, el uso de hardware (cámara) para automatizar ingresos de recibos, y la experiencia fluida de liquidar la deuda directamente desde la misma app móvil.

8. **El mayor riesgo de mi producto es:**  
   La desconfianza de los usuarios al tener que registrar sus ingresos reales en una plataforma digital o la reticencia a enlazar métodos de pago en una app nueva.  
   **Lo resolveremos mediante:**  
   Políticas de privacidad estrictas, encriptación de datos, un diseño que denote seguridad institucional, y alianzas con pasarelas de pago de terceros ampliamente reconocidas y confiables.

9. **Otras suposiciones que, si se demuestran falsas, harán que nuestro negocio fracase:**  
   - Que las personas están dispuestas a transparentar su nivel de ingresos con sus convivientes.  
   - Que los usuarios prefieran descargar una app dedicada a este fin en lugar de usar transferencias bancarias directas (Yape/Plin) con cálculos mentales.  
   - Que los usuarios cuenten con dispositivos móviles con capacidad de almacenamiento y características de hardware necesarias para correr la aplicación fluidamente.

   ### Supuestos del Cliente – Splitly

1. **¿Quién es el cliente?**  
   Jóvenes profesionales y estudiantes universitarios que comparten departamento (roommates), así como parejas jóvenes o familias con ingresos económicos dispares que buscan una gestión más justa de los gastos del hogar.

2. **¿Dónde encaja nuestro producto en su vida?**  
   En su vida cotidiana dentro del hogar compartido, específicamente en la gestión mensual de gastos como alquiler, servicios, alimentos y otros gastos comunes.

3. **¿Qué problemas soluciona nuestro producto?**  
   - Conflictos y tensiones por la división desigual o poco clara de los gastos.  
   - Falta de transparencia en los aportes de cada miembro del hogar.  
   - Pérdida de tiempo realizando cálculos manuales.  
   - Dificultad para llevar un registro ordenado de pagos y deudas.

4. **¿Cuándo y cómo se utiliza nuestro producto?**  
   - Uso frecuente al registrar gastos compartidos (diarios o semanales).  
   - Uso mensual al calcular y distribuir los gastos totales del hogar.  
   - Uso puntual al escanear recibos físicos o al realizar pagos entre convivientes.  
   - Acceso a través de la app móvil para gestionar gastos, revisar balances y liquidar deudas.

5. **¿Qué características son importantes?**  
   - Cálculo automático proporcional basado en ingresos.  
   - Integración con pasarelas de pago.  
   - Notificaciones y recordatorios de pago.  
   - Historial claro y accesible de gastos y deudas.

6. **¿Cómo debe verse y comportarse nuestro producto?**  
   - Diseño moderno, intuitivo y fácil de usar.  
   - Interfaz clara que transmita confianza y seguridad.  
   - Navegación fluida en dispositivos móviles.  
   - Respuestas rápidas, cálculos precisos.

### 1.2.2.3 Lean UX Hypothesis Statements

**Hipótesis 1 – Distribución equitativa de gastos**  
Creemos que automatizar la asignación de contribuciones según los ingresos individuales aumentará la equidad y reducirá los conflictos financieros.  
**Consideraremos que hemos alcanzado el éxito cuando** el **70 % de los usuarios** manifieste una **disminución en las discusiones por dinero** y una **mayor satisfacción con la gestión financiera** durante los primeros tres meses.

**Hipótesis 2 – Transparencia y control del representante del hogar**  
Suponemos que al ofrecer reportes automáticos y alertas visuales, el representante del hogar logrará fortalecer la transparencia y el cumplimiento de pagos.  
**Consideraremos que hemos alcanzado el éxito cuando** el número de **pagos atrasados se reduzca en un 50 %**, y el **60 % de los hogares** utilice activamente el panel de control.

**Hipótesis 3 – Adopción y facilidad de uso**  
Creemos que una interfaz intuitiva y adaptable incrementará la adopción del sistema incluso entre usuarios con poca experiencia digital.  
**Consideraremos que hemos alcanzado el éxito cuando** el **80 % de los usuarios** complete el registro y uso básico sin requerir asistencia técnica.

**Hipótesis 4 – Cultura de ahorro cooperativo**  
Consideramos que introducir metas de ahorro compartidas fomentará la planificación y cooperación económica familiar.  
**Consideraremos que hemos alcanzado el éxito cuando** al menos el **50 % de los hogares** cree y mantenga una **meta de ahorro en común** durante los primeros dos meses.

### 1.2.2.4 Lean UX Canvas

<img src="./assets/LeanUX_Canvas.png" alt="Lean UX Canvas" width="100%">


### 1.3 Segmentos objetivo

Para el modelo de negocio de Splitly, se han identificado dos segmentos principales que interactuarán con la solución móvil y web. A continuación, se detallan sus perfiles y el sustento estadístico que valida la necesidad del producto en el mercado.

---

#### Segmento objetivo 1: Convivientes y Roommates (Miembros del hogar)

##### Aspectos demográficos
- Sexo: Masculino y femenino  
- Edad: 18 – 65 años  
- Nivel socioeconómico: Clases A, B y C (alta, media-alta y media)  
- Estado civil: Solteros, casados, convivientes, parejas, compañeros de cuarto  

##### Aspectos geográficos
- Nacionalidad: Peruana  
- Zona geográfica: Urbana y suburbana  
- Departamento: Lima Metropolitana y principales ciudades del país  

##### Aspectos psicográficos
- Buscan una forma justa y equitativa de compartir gastos del hogar (alquiler, servicios, alimentación, etc.)  
- Están interesados en herramientas que brinden transparencia y simplicidad en la gestión de las finanzas  
- Se preocupan por mantener un equilibrio financiero entre los miembros del hogar, asegurando que cada uno aporte de acuerdo a sus ingresos  
- Tienen un estilo de vida basado en la convivencia y la corresponsabilidad, por lo que valoran soluciones que reduzcan discusiones y simplifiquen la organización de pagos  

##### Información estadística de sustento
Según un estudio de Ipsos Perú sobre Perfiles Socioeconómicos, la convivencia entre jóvenes (roommates) o parejas sin casarse ha aumentado significativamente en zonas urbanas debido al alto costo de los alquileres. Además, reportes del sector inmobiliario indican que más del 40% de los jóvenes profesionales optan por compartir departamento para aligerar la carga económica. A nivel de comportamiento financiero, la Superintendencia de Banca, Seguros y AFP (SBS) señala que la población joven y adulta joven es altamente afín a la adopción de billeteras digitales (como Yape o Plin) y aplicaciones móviles para resolver sus transacciones cotidianas, lo que valida la disposición de este segmento a utilizar una app como Splitly para liquidar sus deudas.

---

#### Segmento objetivo 2: Representante o Administrador del hogar

##### Aspectos demográficos
- Sexo: Masculino y femenino  
- Edad: 25 – 50 años  
- Nivel socioeconómico: Clases A, B y C (alta, media-alta y media)  
- Estado civil: Casados, convivientes, parejas con hijos o personas encargadas de la administración financiera del hogar  

##### Aspectos geográficos
- Nacionalidad: Peruana  
- Zona geográfica: Urbana y suburbana  
- Departamento: Lima Metropolitana y principales ciudades del país  

##### Aspectos psicográficos
- Son responsables de la planificación y control de los gastos familiares, buscando asegurar la equidad entre los integrantes  
- Muestran interés en herramientas digitales que permitan monitorear y organizar finanzas de manera práctica  
- Buscan evitar conflictos financieros dentro del hogar mediante claridad y control en los aportes de cada miembro  
- Están comprometidos con la eficiencia en la gestión de recursos y valoran soluciones que distribuyan gastos de manera proporcional y transparente  

##### Información estadística de sustento
De acuerdo con encuestas de Datum Internacional sobre la economía familiar en Perú, más del 65% de las familias y hogares afirman que el pago de servicios básicos (agua, luz, internet) y alimentación representan su mayor carga de estrés a fin de mes. En muchos de estos hogares, suele haber un "administrador principal" (generalmente uno de los miembros de la pareja) que asume la carga mental de recolectar el dinero y pagar los recibos. Por otro lado, datos de la Cámara Peruana de Comercio Electrónico (CAPECE) muestran que la digitalización y el uso de smartphones para la gestión de finanzas creció por encima del 50% en los últimos años en los sectores A, B y C. Esto demuestra que los administradores del hogar ya cuentan con las capacidades tecnológicas y el dispositivo necesario para adoptar Splitly y digitalizar la captura de recibos y el cobro.

# Capítulo II: Requirements Elicitation & Analysis

## 2.1. Competidores

### 2.1.1. Análisis competitivo

Mediante un análisis comparativo, hemos organizado información clave de cada propuesta de valor. Esto nos ayudará a entender mejor en qué se diferencia nuestra solución y compararla con las de nuestros competidores.


| Categoría | Detalle | **Splitly** | **Halfway** | **UnityPay** | **Parity** |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **¿Por qué este análisis?** | **Objetivo** | Automatizar la distribución de los gastos del hogar de forma proporcional a los ingresos de cada integrante. | Identificar el estándar de automatización de gastos en parejas. | Evaluar la flexibilidad de las reglas de equidad financiera. | Analizar la experiencia de usuario en apps de nicho de reciente lanzamiento. |
| **Perfil** | **Overview** | Aplicación móvil y sitio web estático diseñados para facilitar la distribución equitativa de gastos del hogar considerando los ingresos personales de cada individuo. | App que automatiza finanzas compartidas mediante sincronización bancaria directa. | Plataforma de gestión de dinero para parejas que permite configurar "reglas de equidad". | App móvil minimalista enfocada exclusivamente en el cálculo porcentual por ingresos. |
| | **Ventaja Competitiva** | Algoritmo de cálculo enfocado estrictamente en la proporcionalidad de los ingresos, uso de la cámara para automatizar ingresos de recibos y liquidación de deudas directamente desde la app. | Sincronización bancaria en tiempo real (EE.UU./UK) que elimina el registro manual. | Permite gestionar tanto gastos compartidos como metas de ahorro en una sola cuenta. | Interfaz extremadamente simple centrada en el cálculo rápido sin fricciones. |
| **Marketing** | **Mercado Objetivo** | Jóvenes profesionales y estudiantes universitarios que comparten departamento (roommates). Parejas jóvenes o familias con ingresos económicos dispares. | Parejas estables y matrimonios que buscan independencia financiera. | Parejas jóvenes "Tech-savvy" con objetivos financieros comunes (viajes, casa). | Parejas jóvenes (Gen Z y Millenials) que inician su convivencia. |
| | **Estrategias de Marketing** | Sitio web estático optimizado para motores de búsqueda (SEO). Marketing digital en redes sociales. Recomendaciones "boca a boca" e invitaciones directas desde la app. | Marketing de contenido sobre "paz mental" y salud financiera en la relación. | Alianzas con influencers de finanzas personales y estilo de vida. | Redes sociales visuales (TikTok/Instagram) enfocadas en simplicidad. |
| **Producto** | **Productos & Servicios** | Cálculo automático proporcional basado en ingresos. Integración con pasarelas de pago. Notificaciones y recordatorios de pago. Historial claro y accesible de gastos y deudas. | División automática, seguimiento de facturas, reportes mensuales. | Cuentas conjuntas virtuales, reglas de división personalizadas, fondos de ahorro. | Calculadora de proporción salarial, registro manual de gastos, alertas de pago. |
| | **Precios & Costos** | Modelo Freemium con acceso gratuito a funciones de cálculo proporcional básico. Comisiones transaccionales por pagos procesados mediante integración de API. | Modelo Freemium con suscripción para conexión bancaria ilimitada. | Suscripción mensual por pareja para acceder a todas las reglas de equidad. | Gratuita con anuncios o pago único para eliminar publicidad. |
| | **Distribución** | Aplicación móvil (nativa/multiplataforma). Sitio web estático (Landing Page). | iOS y Android (enfocado en mercados anglosajones). | iOS y Android (Global). | Principalmente iOS. |
| **SWOT** | **Fortalezas** | Algoritmo de cálculo proporcional de ingresos. Uso de hardware (cámara) para automatizar el ingreso de recibos físicos. Experiencia fluida para liquidar deudas desde la app. | Robustez tecnológica y automatización real vía API bancaria. | Gran flexibilidad en la personalización de las reglas de división. | Curva de aprendizaje casi nula y diseño moderno. |
| | **Debilidades** | Posible desconfianza de los usuarios para registrar ingresos reales en una plataforma digital o enlazar métodos de pago en una app nueva. | Muy dependiente de la infraestructura bancaria local. | Puede resultar compleja de configurar inicialmente. | Funcionalidades limitadas; no gestiona ahorros ni inversiones. |
| | **Oportunidades** | La población joven es altamente afín a la adopción de billeteras digitales y apps móviles. La digitalización para gestión de finanzas creció más del 50% en los últimos años en sectores A, B y C. | Expansión a mercados internacionales donde el Open Banking crece. | Integración con sistemas de pago directo (como wallets digitales). | Posicionarse como la app de entrada para quienes nunca han compartido gastos. |
| | **Amenazas** | Aplicaciones genéricas de división de gastos y métodos informales (Excel, memoria). Riesgo de que los usuarios prefieran transferencias bancarias directas (Yape/Plin) realizando cálculos mentales. | Apps de banca tradicional lanzando funciones de "cuentas compartidas". | Competencia directa de neobancos que ya incluyen gestión de gastos. | Facilidad de ser copiada por apps de gestión de gastos más grandes. |

### 2.1.2. Estrategias y tácticas frente a competidores
Para que Splitly penetre con éxito en el mercado, la estrategia que seguiremos se enfocará en integrarse fluidamente a los hábitos de pago diarios del segmento joven mediante las pasarelas de paga conocidas en el país. A nivel de producto, el verdadero diferenciador será aprovechar la función de cálculo proporcional no solo para dividir gastos, sino para proyectar metas de ahorro compartidas que mejoren la salud financiera del hogar. 

Asimismo, será crucial implementar un modelo de privacidad y "onboarding" amigable donde los ingresos absolutos se mantengan ocultos para el resto de los convivientes, mostrando únicamente los porcentajes de deuda correspondientes a cada uno. De esta manera, estaremos garantizando la equidad sin vulnerar la confidencialidad de los demás.
## 2.2. Entrevistas

### 2.2.1. Diseño de entrevistas

### Segmento objetivo 1: Convivientes y Roommates (Miembros del hogar)

**Aspectos demográficos y psicográficos clave**

- Sexo: Masculino o femenino
- Edad: 18 a 65 años
- Nivel socioeconómico: A, B, y C
- Estado civil: Solteros, casados, convivientes, parejas, roommates
- Zona: Urbana y suburbana (Perú)

**Preguntas demográficas:**

1. ¿Me podria decir su edad?
2. ¿Cual es su sexo?
3. ¿En que zona vive actualmente?
4. ¿Con cuál de estas opciones se identifica su nivel socioeconómico? (A / B / C)
5. ¿Cuál es su estado civil o situación actual?

**Preguntas Principales:**

1. ¿Con quién vive actualmente y cómo reparten los gastos del hogar?
2. ¿Considera justo el sistema que usan para dividir los pagos? ¿Por qué?
3. ¿Cuáles son los mayores retos al organizar los gastos compartidos?
4. ¿Han tenido desacuerdos por temas de dinero o pagos en el hogar?
5. ¿Han considerado dividir los gastos en función de los ingresos de cada persona?
6. ¿Utilizan alguna app para anotar los pagos del hogar? ¿Cuál y qué tan útil les resulta?
7. ¿Qué funcionalidades cree que debería tener una app ideal para gestionar gastos entre varias personas?
8. ¿Cómo le gustaría visualizar lo que le toca pagar, lo que ya pagó y lo que está pendiente?
9. ¿Cree que una aplicación como Splitly podría ayudar a mejorar la convivencia y la organización en su hogar?

### Segmento objetivo 2: Representante o Administrador del hogar

**Aspectos demográficos y psicográficos clave**

- Sexo: Masculino o femenino
- Edad: 25 a 50 años
- Nivel socioeconómico: A, B, y C
- Estado civil: Casados, convivientes, parejas con hijos, personas responsables de las finanzas del hogar
- Zona: Urbana y suburbana (Perú)

**Preguntas demográficas:**

1. ¿Me podria decir su edad?
2. ¿Cual es su sexo?
3. ¿En que zona vive actualmente?
4. ¿Con cuál de estas opciones se identifica su nivel socioeconómico? (A / B / C)
5. ¿Cuál es su estado civil o situación actual?

**Preguntas Principales:**

1. ¿Cuál es su rol dentro de su hogar en cuanto a la administración del dinero?
2. ¿Cómo organiza actualmente los ingresos y gastos del hogar?
3. ¿Considera que el reparto de los gastos es equitativo para todos los miembros?
4. ¿Qué dificultades enfrenta para lograr un reparto justo de los gastos?
5. ¿Cómo controla que cada miembro cumpla con su parte financiera?
6. ¿Qué herramientas (apps, cuadernos, Excel, etc.) usa actualmente para llevar este control?
7. ¿Qué funcionalidades le gustaría que tenga una app como Splitly?
8. ¿Qué tan importante considera la transparencia financiera dentro del hogar?
9. ¿Estaría dispuesto(a) a registrar los ingresos de cada miembro para que la aplicación calcule automáticamente cuánto debe aportar cada uno?
10. ¿Qué beneficios cree que traería una solución como Splitly en la convivencia familiar?


### 2.2.2. Registro de entrevistas

En esta sección, se registra cada entrevista realizada. En total, se realizaron tres entrevistas por cada segmento objetivo. Se detalla el nombre del miembro entrevistador y el del entrevistado. Además, se redacta un resumen general del contenido de la entrevista realizada.

Segmento Objetivo 1: Miembros del hogar
  
Entrevista 1:  

| Entrevista | Registro |  
| ----- | ----- |  
| <p align="center"><img src="./assets/Entrevista1.png"/></p> | **Zona:** Magdalena <br>**Entrevistada:** Maria Fernanda |  
| [Link](https://upcedupe-my.sharepoint.com/personal/u20201f788_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20201f788%5Fupc%5Fedu%5Fpe%2FDocuments%2Fupc%2Dpre%2D202601%2Dcc238%2D3667%2DSplitly%20needfinding%2Dsprint%2D1%20%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E42e1c332%2Df797%2D4b13%2Dbfa1%2D69414c126315)|  **Entrevistador:** Jose Luis Martinez Valdivia |  
| Timing: Minuto 0:00-4:10| **Resumen:** María Fernanda, de 20 años, es soltera y vive con su familia. En su hogar, los gastos se dividen entre todos los miembros, lo que en general les permite cubrir sus necesidades de manera organizada. Ella considera que el sistema que llevan actualmente para gestionar los gastos es eficiente, ya que cada integrante asume una parte proporcional, pero reconoce que su mayor dificultad está en mantener un registro claro y ordenado de cada desembolso. Para ella, contar con una aplicación que ofrezca registros rápidos y fáciles de consultar sería de gran utilidad, pues le permitiría llevar un control más transparente y evitar confusiones en el futuro. Como tecnologias utiliza un celular iphone con IOS 25.|  

Entrevista 2:  
  
| Entrevista | Registro |  
| ----- | ----- |  
| <p align="center"><img src="./assets/Entrevista2.png"/></p> | **Zona:** Magdalena del Mar <br>**Entrevistado:** Melisa Geraldine Sulca |  
| [Link](https://upcedupe-my.sharepoint.com/personal/u20201f788_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20201f788%5Fupc%5Fedu%5Fpe%2FDocuments%2Fupc%2Dpre%2D202601%2Dcc238%2D3667%2DSplitly%20needfinding%2Dsprint%2D1%20%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E42e1c332%2Df797%2D4b13%2Dbfa1%2D69414c126315)|  **Entrevistador:** Joaquin Alberto Cuentas Peña |  
| Timing: Minuto 4:11-10:26| **Resumen:** Melisa Sulca, de 23 años, es soltera y vive junto a su hermana y su prima. En su hogar, los gastos más importantes, como el pago de servicios principales y compromisos de mayor monto, son asumidos por su padre. En cambio, los gastos comunes, relacionados con el día a día, se dividen entre Harri y su primo. Esta forma de organización les resulta práctica y cómoda, ya que no genera conflictos y todos saben con claridad qué parte les corresponde cubrir. El principal reto que enfrenta al organizar sus finanzas surge al momento de realizar las compras para la casa, aunque señala que no han tenido desacuerdos al repartir los gastos. Melisa no considera necesario dividirlos según los ingresos de cada miembro, ya que como convive con su familia le resulta practico el tema de dividir proporcionalmente los gastos; sin embargo, si viviera con otras personas considera que sí sería provechoso. Como tecnologia movil utiliza un celular android Samsung con Android 15.|  
  
Entrevista 3:  
  
| Entrevista | Registro |  
| ----- | ----- |  
| <p align="center"><img src="./assets/Entrevista3.png"/></p> | **Zona:** San Miguel<br>**Entrevistado:** Diego Avalos |  
| [Link](https://upcedupe-my.sharepoint.com/personal/u20201f788_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20201f788%5Fupc%5Fedu%5Fpe%2FDocuments%2Fupc%2Dpre%2D202601%2Dcc238%2D3667%2DSplitly%20needfinding%2Dsprint%2D1%20%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E42e1c332%2Df797%2D4b13%2Dbfa1%2D69414c126315)|  **Entrevistador:** Joaquin Alberto Cuentas Peña |  
| Timing: Minuto 10:27-15:45| **Resumen:** Diego Avalos, de 20 años, es soltero y comparte vivienda con 2 amigos de la universidad, todos ellos son estudiantes que vienen de provincia y alquilar una vivienda en común cerca a la Universidad. Para organizarse, decidieron dividir los gastos del hogar entre los cuatro. Aunque este método les permite cubrir sus necesidades básicas, Diego comenta que el mayor reto que enfrentan es ponerse de acuerdo sobre quién debe pagar en cada ocasión, así como recordar quién ya cumplió con su parte y quién no lo ha hecho. Esta situación ha generado varios desacuerdos, especialmente al momento de realizar los pagos compartidos. considera que dividir los gastos según los ingresos de cada miembro no sería una alternativa viable, ya que complicaría aún más la organización y la gestión de sus finanzas. Por esta razón, Diego cree que una aplicación con funciones específicas, como recordar los gastos pendientes y notificar las acciones que realizan los demás integrantes, sería de gran utilidad. Como tecnologia movil utiliza un celular Xiaomi con Android 15.  
  
Segmento Objetivo 2: Representante del hogar
  
Entrevista 4:  
  
| Entrevista | Registro |  
| ----- | ----- |  
| <p align="center"><img src="./assets/Entrevista4.png"/></p> | **Zona:** Magdalena del Mar<br>**Entrevistada:** Juan Castillo |  
| [Link](https://upcedupe-my.sharepoint.com/personal/u20201f788_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20201f788%5Fupc%5Fedu%5Fpe%2FDocuments%2Fupc%2Dpre%2D202601%2Dcc238%2D3667%2DSplitly%20needfinding%2Dsprint%2D1%20%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E42e1c332%2Df797%2D4b13%2Dbfa1%2D69414c126315)| **Entrevistador:** Walter Fajardo |  
| Timing: Minuto 15:46-20:38| **Resumen:** Juan Castillo, de 27 años es soltero y vive con su hermano menor. Él se encarga de administrar el dinero destinado a los pagos y la organización de los gastos del hogar. Considera que la distribución de los gastos es equitativa, ya que él trabaja y recibe un salario considerable que le permite cubrir el 70% de los gastos, mientras que su hermano cubre el 30%. Su mayor dificultad al momento de gestionar las finanzas surge cuando realiza compras innecesarias, ya que esto provoca que en ocasiones se exceda del presupuesto establecido. Juan cree que una aplicación que registre los gastos de manera automática y que, además, envíe recordatorios mensuales sobre pagos próximos o recurrentes sería de gran ayuda para evitar retrasos y mantener un control más estricto. También considera muy útil una función que identifique y clasifique los gastos innecesarios, lo que le permitiría reconocer patrones de consumo, tomar decisiones más conscientes y, al mismo tiempo, contar con una herramienta que calcule de forma automática cuánto gasta cada integrante de la familia, garantizando mayor transparencia y equidad en la administración del dinero, y fortaleciendo así la confianza y la organización en el hogar. Como tecnologia movil utiliza un celular android con Android 16.|  

Entrevista 5:  
  
| Entrevista | Registro |  
| ----- | ----- |  
| <p align="center"><img src="./assets/Entrevista5.png"/></p> | **Zona:** San Isidro<br> **Entrevistado:** Frank |  
| [Link](https://upcedupe-my.sharepoint.com/personal/u20201f788_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20201f788%5Fupc%5Fedu%5Fpe%2FDocuments%2Fupc%2Dpre%2D202601%2Dcc238%2D3667%2DSplitly%20needfinding%2Dsprint%2D1%20%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E42e1c332%2Df797%2D4b13%2Dbfa1%2D69414c126315)|  **Entrevistador:** Kevin Patrick Pardo Chumpitazi |  
| Timing: Minuto 20:39-24:45| **Resumen:** Frank, de 25 años, vive con su pareja y es quien se encarga principalmente de los gastos del hogar. Para mantener un control adecuado, organiza un presupuesto mensual en el que contempla tanto los gastos fijos como los variables. Además, utiliza Excel como herramienta de apoyo para calcular y registrar sus finanzas, lo que le permite tener una visión más ordenada de sus ingresos y egresos. Él considera que la forma en que distribuyen los gastos en el hogar es equitativa; sin embargo, reconoce que su mayor dificultad surge con los gastos imprevistos, especialmente aquellos relacionados con urgencias o problemas que no estaban contemplados en el presupuesto inicial. Frank cree que sería de gran utilidad contar con una aplicación que automatice la división de los gastos y que, además, ofrezca reportes claros, alertas y recordatorios. Para él, una herramienta sencilla de usar que le permita organizar mejor las finanzas del hogar, anticiparse a posibles problemas y visualizar de manera clara la distribución de sus recursos sería clave para optimizar la gestión de su dinero. Como tecnología movil utiliza un celular iphone con IOS 25.|  
  
Entrevista 6:  
  
| Entrevista | Registro |  
| ----- | ----- |  
| <p align="center"><img src="./assets/Entrevista6.png"/></p> | **Zona:** Chorrillos<br>**Entrevistada:** Jessica Castillo |  
| [Link](https://upcedupe-my.sharepoint.com/personal/u20201f788_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20201f788%5Fupc%5Fedu%5Fpe%2FDocuments%2Fupc%2Dpre%2D202601%2Dcc238%2D3667%2DSplitly%20needfinding%2Dsprint%2D1%20%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E42e1c332%2Df797%2D4b13%2Dbfa1%2D69414c126315)| **Entrevistador:** Angel Martin Gonzales Castillo |  
| Timing: Minuto 24:45-30:00| **Resumen:** Jessica Castillo, de 47 años es casada y vive con su familia. Ella se encarga de administrar el dinero destinado a los pagos y la organización de los gastos del hogar. Considera que la distribución de los gastos es equitativa, ya que tanto ella como su esposo aportan a las necesidades principales de la familia, cubriendo servicios, alimentación y otros compromisos esenciales. Su mayor dificultad al momento de gestionar las finanzas surge cuando realiza compras innecesarias, ya que esto provoca que en ocasiones se exceda del presupuesto establecido. Jessica cree que una aplicación que registre los gastos de manera automática y que, además, envíe recordatorios mensuales sobre pagos próximos o recurrentes sería de gran ayuda para evitar retrasos y mantener un control más estricto. También considera muy útil una función que identifique y clasifique los gastos innecesarios, lo que le permitiría reconocer patrones de consumo, tomar decisiones más conscientes y, al mismo tiempo, contar con una herramienta que calcule de forma automática cuánto gasta cada integrante de la familia, garantizando mayor transparencia y equidad en la administración del dinero, y fortaleciendo así la confianza y la organización en el hogar. Utiliza como browser Google Chrome y Edge. Como tecnologias utiliza un celular android y una laptop con sistema operativo Windows.|  


### 2.2.3. Análisis de entrevistas ###

En primer lugar, con base en las tres entrevistas realizadas al primer segmento objetivo, conformado por los miembros del hogar, se puede concluir lo siguiente:

* La organización de los gastos depende más de la practicidad que de los ingresos. En primer lugar, Melisa considera que la división de gastos no debería depender estrictamente de los ingresos, sino de la practicidad y comodidad que facilite la convivencia. Diego, por su parte, comparte en parte esta visión, aunque señala que la falta de un método más formal puede generar confusiones con el tiempo.
    
* La principal dificultad surge en el control y la claridad de los pagos. Los entrevistados señalaron que, aunque no ha tenido tantos conflictos, reconocen que la informalidad puede causar olvidos o desbalances en el largo plazo y necesitarían que todos los integrantes de la vivienda reciban notificaciones y plazos iguales para tods.
    
* Existe una necesidad común de apoyo digital para gestionar mejor los gastos. Todos los entrevistados manifiestan una necesidad común de apoyo digital para gestionar los gastos del hogar. Sin embargo, sus prioridades difieren ligeramente: Melisa busca una herramienta práctica y rápida; María Fernanda, una con funciones de recordatorios y reportes; y Diego, una aplicación que permita una división más equitativa y transparente. Estas diferencias muestran que, aunque el interés por una solución digital es compartido, las expectativas y motivaciones varían según la experiencia de cada integrante.


A continuación, se presentan los porcentajes destacados en las respuestas de los entrevistados a las preguntas planteadas:

* Division de gastos:  
    
  <p align="center"><img src="https://i.imgur.com/nUKYnrB.png"/></p>  
    
    En esta imagen, se visualiza una relación de respuestas sobre el tema planteado. Luego del análisis a este gráfico, se concluye que hay una gran mayoría que considera que si se deberia de dividir las gastos segun la ganancia de cada miembro. Pero, hay una pequeña parte que no esta deacuerdo.  
    
* Desacuerdo en los pagos:  
    
  <p align="center"><img src="https://i.imgur.com/AY208xg.png"/></p>  
    
  En esta imagen, se visualiza una relación de respuestas sobre el tema planteado. Luego del análisis a este gráfico, se concluye que hay una gran mayoría que si presento desacuerdos a la hora de realizar sus pagos correspondientes. Pero, hay una pequeña parte que no presenta desacuerdos entre los miembros del hogar.


* Aplicacion que mejora la organizacion:  
    
  <p align="center"><img src="https://imgur.com/3O20Qjl.png"/></p>  
    
  En esta imagen, se visualiza una relación de respuestas sobre el tema planteado. Luego del análisis a este gráfico, se concluye que todos los entrevistados consideran util e imprensindible una aplicacion que mejore la organizacion de sus gastos.  


Segundo, con base en las tres entrevistas realizadas al segundo segmento objetivo, conformado por los representantes del hogar, se puede concluir lo siguiente:

* Uso de métodos previos para gestionar las finanzas. Todos los entrevistados ya emplean algún tipo de organización antes de recurrir a una aplicación digital. Algnunos especificaron hojas de cálculo en Excel para presupuestar y clasificar gastos, mientras que otros también recurren a hacer sus cálculos a mano y notificarlo por mensaje. Esto refleja una clara disposición hacia el orden y la planificación financiera.
* Necesidad de un control más profundo y adaptable. Las principales dificultades giran en torno a factores que desequilibran la organización: Las compras innecesarias, los gastos imprevistos, la variación de ingresos. Todos coinciden en que requieren herramientas que permitan un seguimiento más detallado, con funciones que automaticen cálculos, generen reportes y se adapten a la realidad de cada hogar.
* Preferencia por soluciones digitales prácticas y accesibles. Existe un consenso en valorar una aplicación que sea fácil de usar, amigable e intuitiva. Los entrevistados consideran importantes funciones como reportes automáticos, alertas, subcategorías de gastos, proyecciones futuras y cálculos individuales por integrante.

A continuación, se presentan los porcentajes destacados en las respuestas de los entrevistados a las preguntas planteadas:

* Mantener un control de estructurado de gastos

  <p align="center"><img src="https://imgur.com/NBKCslQ.png"/></p>

  En esta imagen, se visualiza una relación de respuestas sobre el tema planteado. Luego del análisis a este gráfico, se concluye que todos los entrevistados requieren un control mas estructurado de sus gastos.

* Necesidad de controlar gastos

  <p align="center"><img src="https://imgur.com/6Wm3qk8.png"/></p>

  En esta imagen, se visualiza una relación de respuestas sobre el tema planteado. Luego del análisis a este gráfico, se concluye que todos los entrevistados tienen una necesidad para poder controlar de forma mas detallada y adaptable

* Uso de herramientas digitales

    <p align="center"><img src="https://imgur.com/Q8wtZKB.png"/></p>
    
    En esta imagen, se visualiza una relación de respuestas sobre el tema planteado. Luego del análisis a este gráfico, se concluye que todos los entrevistados consideran el uso de herramientas digitales para poder mejorar el control de gastos





## 2.3. Needfinding
A partir del análisis de entrevistas y del Lean UX Canvas presentado en el capítulo 1, se identificaron las principales necesidades y motivaciones de los segmentos objetivo. Los hallazgos confirman los problemas detectados en el Canvas: la falta de equidad en la distribución de gastos, la poca transparencia y la ausencia de herramientas colaborativas adaptadas a la realidad económica de cada hogar.

De esta manera, se presentan a continuación los hallazgos clave que guiarán el desarrollo de la solución
  
## Segmento #1: Convivientes y Roommates

- **Dividir los gastos comunes** forma justa y proporcional a los ingresos de cada miembro.  
- **Contar con visibilidad en tiempo real** sobre pagos realizados y saldos pendientes.  
- **Garantizar transparencia** para evitar malentendidos y conflictos dentro de la convivencia.  
- **Usar una aplicación movil sencilla** que organice los pagos del hogar y reduzca la carga mental.  

## Segmento #2: Representante o Administrador del hoga

- **Gestionar y supervisar** todos los aportes desde un panel centralizado.  
- **Recibir alertas automáticas** y recordatorios de pagos pendientes.  
- **Asegurar que las contribuciones** sean equitativas y basadas en ingresos reales.  
- **Obtener reportes financieros claros** y automáticos para ahorrar tiempo en la planificación y fortalecer la confianza del grupo.  



### 2.3.1. User Personas

- Segmento #1:  Convivientes y Roommates
<p styles="align: left">
  <img src="./assets/Adriana Zambrano.png" width="1100">
</p>

- Segmento #2: Representante o Administrador del hogar

<p styles="align: left">
  <img src="./assets/Miriam Hernandez.png" width="1100">
</p>



### 2.3.2. User Task Matrix.

En esta sección se presenta la *User Task Matrix*, enfocada en los dos segmentos clave de **Splitly**: Convivientes/Roommates y Representante/Administrador.  
Este instrumento permite identificar sus tareas habituales, nivel de importancia y frecuencia, así como los beneficios esperados (*Outcomes*) que el sistema debe ofrecer.  
Su análisis facilita la priorización de funcionalidades y asegura la coherencia con la propuesta de valor del producto: **automatización, transparencia y colaboración en la gestión financiera compartida.**

| **Persona** | **Tarea** | **Importancia** | **Frecuencia** | **Beneficio / Outcome** |
|--------------|------------|------------------|----------------|--------------------------|
| **Adriana (Miembro del hogar)** | Registrar su ingreso mensual | Alta | Baja | Permite que el sistema calcule automáticamente su aporte proporcional. |
|  | Revisar cuánto debe aportar según su ingreso | Alta | Alta | Aumenta la transparencia y confianza en los pagos. |
|  | Recibir recordatorios y confirmar pagos | Media | Media | Reduce los olvidos y mejora la convivencia financiera. |
|  | Consultar historial de pagos | Media | Baja | Brinda control y claridad sobre su participación mensual. |
| **Miriam (Representante del hogar)** | Crear y gestionar gastos compartidos | Alta | Alta | Centraliza la información y simplifica la planificación mensual. |
|  | Supervisar pagos realizados y pendientes | Alta | Alta | Asegura la equidad y el cumplimiento de las contribuciones. |
|  | Enviar recordatorios automáticos | Media | Media | Disminuye la carga operativa y los conflictos por pagos atrasados. |
|  | Generar reportes mensuales | Alta | Baja | Facilita la toma de decisiones y la comunicación con los miembros. |


### 2.3.3. User Journey Mapping.

Aquí se presentan los User Journey Mapping para cada user persona. El recorrido refleja cómo los usuarios reciben notificaciones de nuevos gastos, consultan su historial, calculan su aporte proporcional y completan el pago, asegurando claridad y transparencia en el proceso.

- Segmento #1: Miembro del hogar

<p styles="align: left">
  <img src="./assets/_AdrianaJM.png" width="1100">
</p>

- Segmento #2: Representante del hogar

<p styles="align: left">
  <img src="./assets/_MiriamJM.png" width="1100">
</p>


### 2.3.4. Empathy Mapping.

El Empathy Mapping permite comprender a fondo qué piensan, sienten, ven, escuchan y hacen los usuarios, así como sus frustraciones y motivaciones. Este análisis facilita diseñar soluciones alineadas con sus verdaderas necesidades.

- Segmento #1: Miembro del hogar
  
<p styles="align: left">
  <img src="./assets/AdrianaEM.png" width="1100">
</p>

- Segmento #2: Representante del hogar

<p styles="align: left">
  <img src="./assets/MiriamEM.png" width="1100">
</p>

### 2.3.5. Big Picture EventStorming.

La técnica del Evenstorming funcionará en Splitly para detallar el flujo de acciones que un usuario de la aplicación podrá ejecutar 

  <img src="./assets/Captura de pantalla 2026-04-24 134123.png" width="1100">


### 2.3.6. Ubiquitous Language

En esta sección se presenta el *Ubiquitous Language* definido para **Splitly**, el cual unifica la terminología utilizada por el equipo de desarrollo, los diseñadores y los usuarios.  
Su propósito es garantizar una comprensión común del dominio, evitando ambigüedades en la comunicación y manteniendo la coherencia entre los artefactos de diseño, los modelos de datos y la experiencia de usuario.

| **Término en Inglés** | **Término en Español** | **Definición** |
|------------------------|------------------------|----------------|
| **Household Representative** | **Representante del hogar** | Usuario responsable de administrar el hogar dentro del sistema. Tiene permisos especiales para registrar nuevos miembros, ingresar gastos comunes y visualizar los aportes de todos. |
| **Household Member** | **Miembro del hogar** | Usuario que forma parte de un hogar registrado. Aporta según su capacidad económica y puede visualizar su historial de gastos y contribuciones. |
| **Income-Based Contribution** | **Contribución basada en ingresos** | Mecanismo mediante el cual se calcula la cantidad que debe aportar cada miembro del hogar, según el ingreso personal declarado. Busca que el reparto sea justo y equitativo. |
| **Shared Expense** | **Gasto compartido** | Gasto que afecta a todo el hogar y que debe dividirse proporcionalmente entre sus miembros (por ejemplo, alquiler, servicios o compras comunes). |
| **Spending Record** | **Registro de gastos** | Entrada digital dentro del sistema que detalla la fecha, el monto, la categoría y quién ingresó el gasto. |
| **Contribution Percentage** | **Porcentaje de contribución** | Valor en porcentaje que representa la participación proporcional de cada miembro en los gastos comunes, calculado con base en su ingreso. |
| **Financial Overview** | **Resumen financiero** | Vista general de los ingresos, aportes y gastos de un hogar, accesible para todos los miembros y con mayor detalle para el representante. |
| **Pending Contribution** | **Contribución pendiente** | Monto que un miembro del hogar aún no ha cubierto con respecto a los gastos registrados. Puede generar recordatorios o alertas automáticas. |
| **Expense Category** | **Categoría de gasto** | Clasificación usada para organizar los gastos ingresados (por ejemplo: alimentación, servicios, alquiler, entretenimiento). Facilita el análisis y el seguimiento financiero. |
| **Adjustment Report** | **Reporte de ajustes** | Documento generado automáticamente por el sistema cuando hay variaciones en los ingresos de un miembro, sugiriendo una nueva distribución de aportes. |

## 2.4. Requirements specification
### 2.4.1. User Stories
#### Epics

| EPIC ID | Nombre del Epic                  | Descripción |
|---------|----------------------------------|-------------|
| EP00    | Arquitectura Técnica y Documentación     | Como desarrollador, quiero diseñar y documentar la arquitectura del sistema para garantizar escalabilidad, mantenimiento y comunicación clara entre miembros del equipo |
| EP01    | Registro y Gestión de Perfil     | Como usuario, quiero registrarme y gestionar mi perfil de forma segura y personalizada, para acceder a Splitly desde cualquier dispositivo. |
| EP02    | Panel del Representante del Hogar| Como representante del hogar, quiero gestionar y supervisar las finanzas del hogar de forma centralizada y transparente. |
| EP03    | Panel del Miembro del Hogar      | Como miembro del hogar, quiero registrar mis ingresos, ver mis responsabilidades y mantenerme al día con mis pagos. |
| EP04    | Gestión de Gastos Compartidos    | Como usuario, quiero registrar, clasificar y gestionar gastos para mantener el control financiero del hogar. |
| EP05    | Seguimiento y Recordatorios      | Como usuario, quiero recibir recordatorios y alertas automáticas para no olvidar mis responsabilidades financieras. |
| EP06    | Soporte y Comunidad              | Como usuario, quiero acceder a soporte técnico y a recursos para mejorar mi uso de la plataforma y resolver dudas. |
| EP07    | Exploración como Visitante       | Como visitante, quiero conocer la funcionalidad, beneficios y casos de uso de Splitly desde la landing page para evaluar si la plataforma es útil para mi hogar antes de registrarme. |

### EP01 - Registro y Gestión de Perfil

| User Story ID | Título                          |
|---------------|----------------------------------|
| US01          | Registro de usuario              |
| US02          | Inicio de sesión seguro          |
| US03          | Edición de información personal  |
| US04          | Cierre de sesión desde todos los dispositivos |
| US05          | Configuración de notificaciones personales |
| TS01          | Implementar autenticación JWT |
| TS02          | Cifrar contraseñas en base de datos |
| TS03          | Validar roles de administrador y miembro en backend |
| TS04          | Implementar actualización de perfil a partir de API |  
| TS05          | Conectar formularios de registro y login del front-end con endpoints   |
| TS06          | Validar respuestas del backend en la gestión de perfil del usuario      |

### EP02 - Panel del Representante del Hogar

| User Story ID | Título                          |
|---------------|----------------------------------|
| US06          | Crear hogar                      |
| US07          | Aprobar gastos                   |
| US08          | Ajustar porcentajes de aportes   |
| US09          | Visualizar reportes mensuales    |
| US10          | Configurar métodos de pago aceptados |
| US36          | Manejar errores del servidor en vistas del representante               |

### EP03 - Panel del Miembro del Hogar

| User Story ID | Título                          |
|---------------|----------------------------------|
| US11          | Ingresar ingresos personales     |
| US12          | Ver monto a pagar                |
| US13          | Registrar pagos realizados       |
| US14          | Ver historial de pagos           |
| US15          | Ver distribución de gastos del hogar |
| US37          | Implementar manejo de estados de carga y éxito en el panel del miembro |

### EP04 - Gestión de Gastos Compartidos

| User Story ID | Título                          |
|---------------|----------------------------------|
| US16          | Registrar nuevo gasto            |
| US17          | Adjuntar comprobantes de gasto   |
| US18          | Clasificar gastos por categoría  |
| US19          | Comentar o justificar un gasto   |
| US20          | Visualizar gráficos de gastos    |
| TS07          | Validar que el gasto tiene adjunto al menos 1 comprobante |
| TS08          | Agregar API para filtrar gastos por rango de fecha |
| TS09          | Implementar actualización y eliminación de gastos |  
| TS10          | Verificar integración entre back-end de gastos y sus componentes en front-end |

### EP05 - Seguimiento y Recordatorios

| User Story ID | Título                          |
|---------------|----------------------------------|
| US21          | Recordatorios de pago            |
| US22          | Alertas de pagos pendientes      |
| US23          | Recordatorio de actualización de ingresos |
| US24          | Confirmación de aportes          |
| US25          | Notificación de cambios en el hogar |
| TS11          | API para programar recordatorios de pago |
| TS12          | Integrar cron job para envío de recordatorios |  
| TS13          | Conectar notificaciones del sistema con el backend                     |

### EP06 - Soporte y Comunidad

| User Story ID | Título                          |
|---------------|----------------------------------|
| US26          | Acceso a ayuda en línea          |
| US27          | Chat con soporte técnico         |
| US28          | Reportar un problema             |
| US29          | Sugerencias de mejora            |
| US30          | Foro comunitario                 |
| TS14          | API para dar seguimiento a reportes de problemas |
| TS15          | Implementar comentarios o respuestas en el foro |
| TS16          | Validar seguridad de comunicación entre app y backend (CORS, HTTPS) |
| TS17          | Probar funcionamiento completo en entorno de producción                |

### EP07 - Exploración como Visitante

| User Story ID | Título                          |
|---------------|----------------------------------|
  | US31          | Visualizar información general sobre Harmonix desde la landing page              |
| US32          | Conocer las funciones principales para representantes y miembros del hogar         |
| US33          | Explorar beneficios del sistema de aportes proporcionales  |
| US34          | Ver ejemplos o simulaciones de cómo funciona la plataforma |
| US35          | 	Acceder fácilmente al registro o login desde botones destacados |
| TS18          | Documentar los pasos para desplegar nuevas versiones                   |
| TS19          | Habilitar monitoreo básico del sistema desplegado (logs, uptime)       |

### USER STORIES


| **ID Épica** | **Épica**                         | **ID HU** | **Título HU**                                       | **Descripción HU**                                                                                                                                                                     | **Criterios de Aceptación**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ------------ | --------------------------------- | --------- | --------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| EP01         | Registro y Gestión de Perfil      | US01      | Registro de usuario                                 | Como usuario de ambos segmentos, quiero registrarme en la app para comenzar a usar Splitly.                                                                                   | - **Escenario 1: Registro como miembro del hogar exitoso**<br> Dado que un usuario quiere registrarse como miembro del hogar,<br> Cuando proporciona todos los datos requeridos correctamente,<br> Entonces el sistema registra al usuario como miembro del hogar,<br> Y el usuario puede acceder a las funcionalidades correspondientes a ese rol.<br><br> - **Escenario 2: Registro como representante del hogar exitoso**<br> Dado que un usuario desea registrarse como representante del hogar,<br> Cuando proporciona todos los datos requeridos correctamente,<br> Entonces el sistema lo registra como representante del hogar,<br> Y el usuario puede acceder a las funcionalidades correspondientes a ese rol. |
| EP01         | Registro y Gestión de Perfil      | US02      | Inicio de sesión seguro                             | Como usuario registrado, quiero iniciar sesión de forma segura para acceder a mis datos personales.                                                                                    | - **Escenario 1: Inicio de sesión exitoso**<br> Dado que el usuario está registrado,<br> Cuando proporciona credenciales válidas,<br> Entonces el sistema le permite acceder a su cuenta.<br><br> - **Escenario 2: Inicio de sesión fallido por credenciales incorrectas**<br> Dado que el usuario intenta autenticarse,<br> Cuando las credenciales proporcionadas no son válidas,<br> Entonces el sistema rechaza el intento de acceso,<br> Y le indica que las credenciales no son válidas.                                                                                                                                                                                                                           |
| EP01         | Registro y Gestión de Perfil      | US03      | Edición de información personal                     | Como usuario de ambos segmentos, quiero editar mi información personal para mantenerla actualizada.                                                                                    | - **Escenario 1: Visualización de información personal**<br> Dado que el usuario ya está logueado,<br> Cuando accede a su información de perfil,<br> Entonces el sistema le muestra sus datos personales actuales en formato editable.<br><br> - **Escenario 2: Actualización de datos personales**<br> Dado que el usuario modifica su información personal,<br> Cuando envía los nuevos datos,<br> Entonces el sistema actualiza correctamente la información.                                                                                                                                                                                                                                                         |
| EP01         | Registro y Gestión de Perfil      | US04      | Cierre de sesión desde todos los dispositivos       | Como usuario de ambos segmentos, quiero cerrar sesión desde todos mis dispositivos para mayor seguridad.                                                                               | - **Escenario 1: Cierre de sesión en todos los dispositivos**<br> Dado que el usuario ha iniciado sesión en su cuenta,<br> Cuando solicita cerrar sesión en todos los dispositivos,<br> Entonces el sistema invalida todas las sesiones activas asociadas a su cuenta.                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| EP01         | Registro y Gestión de Perfil      | US05      | Configuración de notificaciones personales          | Como usuario de ambos segmentos, quiero configurar mis notificaciones para recibir alertas relevantes.                                                                                 | - **Escenario 1: Visualización de opciones de notificación**<br> Dado que el usuario accede a su configuración de perfil,<br> Cuando solicita ver las opciones de notificación,<br> Entonces el sistema muestra las opciones disponibles para activar o desactivar alertas.<br><br> - **Escenario 2: Aplicación de configuración de notificaciones**<br> Dado que el usuario selecciona sus preferencias de notificación,<br> Cuando envía la configuración,<br> Entonces el sistema guarda las preferencias y las aplica para futuras alertas.                                                                                                                                                                          |
| EP01         | Registro y Gestión de Perfil      | TS01      | Implementar autenticación JWT                       | Como desarrollador, quiero que el inicio de sesión implemente autenticación JWT para mayor seguridad en el manejo de sesiones.                                                         | - **Escenario 1: Generación del JWT**<br> Dado que el usuario proporciona credenciales correctas,<br> Cuando se autentica,<br> Entonces el backend genera y responde con un JWT válido.<br><br> - **Escenario 2: Validación del JWT**<br> Dado que el JWT se adjunta en el encabezado de la solicitud,<br> Cuando el backend verifica el token,<br> Entonces autoriza el acceso si el token es válido.                                                                                                                                                                                                                                                                                                                   |
| EP01         | Registro y Gestión de Perfil      | TS02      | Cifrar contraseñas en base de datos                 | Como desarrollador, quiero que las contraseñas de los usuarios sean encriptadas antes de guardarlas en la base de datos para garantizar la seguridad.                                  | - **Escenario 1: Almacenar contraseña cifrada**<br> Dado que la contraseña llega en texto plano,<br> Cuando el backend lo encripta,<br> Entonces se almacena en la base de datos de forma cifrada.<br><br> - **Escenario 2: Validar contraseña cifrada durante autenticación**<br> Dado que la contraseña en la base de datos está cifrada,<br> Cuando el backend verifica credenciales,<br> Entonces primero hace el hash de la contraseña ingresada y lo compara con el guardado.                                                                                                                                                                                                                                      |
| EP01         | Registro y Gestión de Perfil      | TS03      | Validar roles de administrador y miembro en backend | Como desarrollador, quiero que ciertos endpoints sean usados solo por determinados roles para asegurar que solo los usuarios autorizados puedan ejecutar determinadas acciones         | - **Escenario 1: Acceso permitido a endpoint por rol administrador**<br> Dado que el rol incluido en el JWT es administrador,<br> Cuando invoque un endpoint de administrador,<br> Entonces el backend permitirá el acceso.<br><br> - **Escenario 2: Acceso denegado a endpoint por rol no autorizado**<br> Dado que el rol incluido en el JWT es miembro,<br> Cuando invoque un endpoint de administrador,<br> Entonces el backend rechazará la solicitud con 403 (Forbidden).                                                                                                                                                                                                                                          |
| EP01         | Registro y Gestión de Perfil      | TS04      | Implementar actualización de perfil a partir de API | Como desarrollador, quiero implementar la actualización del perfil de usuario mediante una API para permitir que los usuarios modifiquen su información de manera segura y controlada. | - **Escenario 1: Actualización exitosa**<br> Dado que el token es válido,<br> Cuando el usuario envía nuevos datos,<br> Entonces el backend actualiza el perfil en la base de datos.<br><br> - **Escenario 2: Solicitud sin autenticación válida**<br> Dado que el token es vencido o inexistente,<br> Cuando el backend recibe la solicitud,<br> Entonces responde con 401 (Unauthorized).                                                                                                                                                                                                                                                                                                                              |
| EP01         | Registro y Gestión de Perfil      | TS05      | Conectar formularios con endpoints                  | Como desarrollador, quiero conectar los formularios de registro y login con los endpoints del backend para que funcionen correctamente.                                                | - **Escenario 1: Envío de datos de registro al backend**<br> Dado que el usuario completa el formulario de registro,<br> Cuando envía el formulario,<br> Entonces el formulario envía la información al endpoint correspondiente.<br><br> - **Escenario 2: Autenticación de usuario mediante el backend**<br> Dado que el usuario ingresa sus credenciales,<br> Cuando el app las envía al endpoint de autenticación,<br> Entonces el backend valida las credenciales.                                                                                                                                                                                                                                              |
| EP01         | Registro y Gestión de Perfil      | TS06      | Validar respuestas del backend                      | Como desarrollador, quiero validar las respuestas del backend para mostrar mensajes adecuados al usuario.                                                                              | - **Escenario 1: Error en el registro**<br> Dado que haya un error del backend al procesar el registro,<br> Cuando el usuario envíe un formulario,<br> Entonces se mostrará un mensaje de error específico.<br><br> - **Escenario 2: Fallo en el inicio de sesión**<br> Dado que el backend retorne un 401 Unauthorized,<br> Cuando se intente iniciar sesión,<br> Entonces el app indicará que las credenciales son inválidas.                                                                                                                                                                                                                                                                                     |
| EP02         | Panel del Representante del Hogar | US06      | Crear hogar                                         | Como representante del hogar, quiero crear un hogar en la app para empezar a gestionar sus finanzas.                                                                                   | - **Escenario 1: Acceso al proceso de creación de hogar**<br> Dado que el usuario ha iniciado sesión como representante del hogar,<br> Cuando accede a la opción de creación de hogar,<br> Entonces podrá ingresar un nombre e ID para el hogar.<br><br> - **Escenario 2: Creación exitosa del hogar**<br> Dado que el usuario completa los campos requeridos,<br> Cuando envía la solicitud de creación,<br> Entonces se crea el hogar y se muestra en su panel.                                                                                                                                                                                                                                                        |
| EP02         | Panel del Representante del Hogar | US07      | Aprobar gastos                                      | Como representante, quiero aprobar gastos para tener control sobre lo que se gasta en el hogar.                                                                                        | - **Escenario 1: Listado de gastos pendientes**<br> Dado que haya gastos sin aprobar,<br> Cuando el representante acceda al panel,<br> Entonces verá una lista de gastos para revisar.<br><br> - **Escenario 2: Aprobación de un gasto**<br> Dado que el representante selecciona un gasto,<br> Cuando confirme su aprobación,<br> Entonces el gasto pasará a estado "Aprobado".                                                                                                                                                                                                                                                                                                                                         |
| EP02         | Panel del Representante del Hogar | US08      | Ajustar porcentajes de aportes                      | Como representante, quiero modificar los porcentajes de contribución de cada miembro según sus ingresos.                                                                               | - **Escenario 1: Acceso a la configuración de aportes**<br> Dado que el representante está autenticado y accede al módulo de gestión del hogar,<br> Cuando accede a la sección de configuración de aportes,<br> Entonces verá una lista editable de miembros.<br><br> - **Escenario 2: Modificación y guardado de aportes**<br> Dado que el representante ha realizado ajustes en los porcentajes,<br> Cuando envía los nuevos valores,<br> Entonces se actualizarán los porcentajes automáticamente.                                                                                                                                                                                                                    |
| EP02         | Panel del Representante del Hogar | US09      | Visualizar reportes mensuales                       | Como representante, quiero ver reportes de ingresos y gastos mensuales para tomar decisiones informadas sobre la economía del hogar.                                                   | - **Escenario 1: Acceso a reportes mensuales**<br> Dado que el representante esté en su dashboard,<br> Cuando accede a la sección de reportes mensuales,<br> Entonces se mostrarán gráficos y resúmenes.<br><br> - **Escenario 2: Descarga de reporte**<br> Dado que el representante ha visualizado un reporte,<br> Cuando solicita su descarga,<br> Entonces el sistema genera un archivo PDF y se descargará el informe correspondiente.                                                                                                                                                                                                                                                                              |
| EP02         | Panel del Representante del Hogar | US10      | Configurar métodos de pago aceptados                | Como representante, quiero configurar qué métodos de pago están habilitados en el hogar.                                                                                               | - **Escenario 1: Ver métodos disponibles**<br> Dado que el usuario acceda a configuración,<br> Cuando seleccione "Métodos de pago",<br> Entonces verá una lista de métodos disponibles.<br><br> - **Escenario 2: Activar métodos**<br> Dado que seleccione métodos específicos,<br> Cuando presione “Guardar”,<br> Entonces esos métodos quedarán habilitados para el hogar.                                                                                                                                                                                                                                                                                                                                             |

| **ID Épica** | **Épica**                         | **ID HU** | **Título HU**                                             | **Descripción HU**                                                                                                     | **Criterios de Aceptación**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------ | --------------------------------- | --------- | --------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| EP02         | Gestión Personal de Finanzas      | US14      | Ver historial de pagos                                    | Como miembro del hogar, quiero consultar un historial de todos mis pagos anteriores para verificar mis contribuciones. | - **Escenario 1: Acceso al historial**<br> Dado que el usuario quiere ver sus aportes anteriores,<br> Cuando acceda a la sección “Historial de pagos” desde su panel,<br> Entonces verá una lista ordenada cronológicamente con fechas, montos, conceptos y comprobantes de cada pago realizado.<br><br> - **Escenario 2: Filtro por periodo**<br> Dado que el usuario desea consultar un periodo específico,<br> Cuando seleccione un mes o rango de fechas,<br> Entonces el sistema mostrará únicamente los pagos correspondientes a ese periodo. |
| EP02         | Panel del Representante del Hogar | US36      | Manejar errores del servidor                              | Como representante, quiero que el sistema maneje errores del servidor de forma clara para entender qué ocurre.         | - **Escenario 1: Error al cargar gastos**<br> Dado que haya una falla en el endpoint de gastos,<br> Cuando se intente acceder al listado,<br> Entonces se mostrará un mensaje "No se pudo cargar los datos".                                                                                                                                                                                                                                                                                                                                        |
| EP03         | Panel del Miembro del Hogar       | US11      | Ingresar ingresos personales                              | Como miembro del hogar, quiero registrar mis ingresos para que el sistema calcule mi aporte.                           | - **Escenario 1: Acceso al formulario de ingresos**<br> Dado que el miembro haya iniciado sesión,<br> Cuando seleccione "Ingresos",<br> Entonces se mostrará el formulario de ingreso de datos.<br><br> - **Escenario 2: Confirmación de ingreso**<br> Dado que complete los datos,<br> Cuando presione "Guardar",<br> Entonces su ingreso quedará registrado en el sistema.                                                                                                                                                                        |
| EP03         | Panel del Miembro del Hogar       | US12      | Ver monto a pagar                                         | Como miembro del hogar, quiero visualizar cuánto debo aportar al hogar basado en mis ingresos.                         | - **Escenario 1: Acceso al panel de pagos**<br> Dado que el usuario haya ingresado sus ingresos,<br> Cuando acceda a "Mis aportes",<br> Entonces verá el monto que le corresponde pagar este mes.                                                                                                                                                                                                                                                                                                                                                   |
| EP03         | Panel del Miembro del Hogar       | US13      | Registrar pagos realizados                                | Como miembro del hogar, quiero registrar que realicé un pago para que el sistema lleve un seguimiento.                 | - **Escenario 1: Ingreso de pago**<br> Dado que el miembro haya realizado un pago,<br> Cuando acceda a "Registrar pago",<br> Entonces podrá indicar el monto, la fecha y el método usado.<br><br> - **Escenario 2: Confirmación**<br> Dado que ingrese los datos,<br> Cuando presione “Guardar”,<br> Entonces el pago quedará registrado correctamente.                                                                                                                                                                                             |
| EP03         | Gestión Personal de Finanzas      | US15      | Ver historial de pagos                                    | Como miembro del hogar, quiero consultar un historial de todos mis pagos anteriores para verificar mis contribuciones. | - **Escenario 1: Acceso al historial**<br> Dado que el usuario quiere ver sus aportes anteriores,<br> Cuando acceda a la sección “Historial de pagos” desde su panel,<br> Entonces verá una lista ordenada cronológicamente con fechas, montos, conceptos y comprobantes de cada pago realizado.<br><br> - **Escenario 2: Filtro por periodo**<br> Dado que el usuario desea consultar un periodo específico,<br> Cuando seleccione un mes o rango de fechas,<br> Entonces el sistema mostrará únicamente los pagos correspondientes a ese periodo. |
| EP03         | Panel del Miembro del Hogar       | US37      | Manejo de estados de carga y éxito                        | Como miembro del hogar, quiero ver indicadores de carga o éxito al registrar mis datos para mejorar la experiencia.    | - **Escenario 1: Indicador de carga**<br> Dado que se envían datos al backend,<br> Cuando aún no se recibe respuesta,<br> Entonces se mostrará un spinner de carga.<br><br> - **Escenario 2: Registro exitoso**<br> Dado que se guarde correctamente,<br> Cuando el servidor responda,<br> Entonces se muestra un mensaje de éxito.                                                                                                                                                                                                                 |
| EP04         | Gestión de Gastos Compartidos     | US16      | Registrar nuevo gasto                                     | Como usuario, quiero registrar un nuevo gasto para mantener actualizados los movimientos financieros.                  | - **Escenario 1: Acceso al formulario**<br> Dado que el usuario haya iniciado sesión,<br> Cuando acceda a "Registrar gasto",<br> Entonces verá un formulario con campos de monto, categoría y descripción.<br><br> - **Escenario 2: Guardado del gasto**<br> Dado que complete el formulario,<br> Cuando presione “Guardar”,<br> Entonces el nuevo gasto se almacenará en el sistema.                                                                                                                                                               |
| EP04         | Gestión de Gastos Compartidos     | US17      | Adjuntar comprobantes de gasto                            | Como usuario, quiero subir comprobantes para respaldar los gastos registrados.                                         | - **Escenario 1: Carga de comprobante**<br> Dado que el usuario registre un gasto,<br> Cuando presione “Adjuntar archivo”,<br> Entonces podrá subir una imagen o PDF como comprobante.<br><br> - **Escenario 2: Visualización**<br> Dado que se haya adjuntado un comprobante,<br> Cuando acceda al gasto,<br> Entonces podrá ver o descargar el archivo.                                                                                                                                                                                           |
| EP04         | Gestión de Gastos Compartidos     | US18      | Clasificar gastos por categoría                           | Como usuario, quiero categorizar los gastos para facilitar su análisis y visualización.                                | - **Escenario 1: Selección de categoría**<br> Dado que el usuario registre un gasto,<br> Cuando acceda a la lista de categorías,<br> Entonces podrá seleccionar entre alimentación, servicios, mantenimiento, etc.<br><br> - **Escenario 2: Filtro**<br> Dado que seleccione una categoría,<br> Cuando aplique el filtro,<br> Entonces se mostrarán solo los gastos correspondientes.                                                                                                                                                               |
| EP04         | Gestión de Gastos Compartidos     | US19      | Comentar o justificar un gasto                            | Como usuario, quiero añadir comentarios para explicar el motivo de un gasto compartido.                                | - **Escenario 1: Comentario en gasto**<br> Dado que el usuario haya registrado un gasto,<br> Cuando seleccione “Añadir comentario”,<br> Entonces podrá escribir y guardar una nota explicativa visible a los miembros del hogar.                                                                                                                                                                                                                                                                                                                    |
| EP04         | Gestión de Gastos Compartidos     | US20      | Visualizar gráficos de gastos                             | Como usuario, quiero ver gráficos de gastos para entender en qué se gasta más.                                         | - **Escenario 1: Acceso a visualizaciones**<br> Dado que el usuario esté en el panel de gastos,<br> Cuando acceda a “Ver gráficos”,<br> Entonces podrá ver gráficos circulares o de barras agrupados por categoría, fecha o usuario.                                                                                                                                                                                                                                                                                                                |
| EP04         | Gestión de Gastos Compartidos     | TS07      | Validar que el gasto tenga adjunto al menos 1 comprobante | Como desarrollador, quiero que cada gasto tenga al menos 1 comprobante adjunto antes de guardarlo.                     | - **Escenario 1: Gasto sin adjunto**<br> Dado que el gasto no tiene comprobante,<br> Cuando el backend recibe la solicitud,<br> Entonces responde con error 400.<br>- **Escenario 2: Gasto con adjunto**<br> Dado que el gasto tiene comprobante,<br> Cuando el backend grava en la base de datos,<br> Entonces lo acepta.                                                                                                                                                                                                                          |
| EP04         | Gestión de Gastos Compartidos     | TS08      | Agregar API para filtrar gastos por rango de fecha        | Como desarrollador, quiero filtrar gastos según rango de fecha.                                                        | - **Escenario 1: Filtrar con rango válido**<br> Dado que envío inicio y fin,<br> Cuando el backend filtra,<br> Entonces responde con gastos en ese rango.<br>- **Escenario 2: Rango sin resultados**<br> Dado que el rango no tiene gastos,<br> Cuando el backend consulta,<br> Entonces responde con una lista vacía.                                                                                                                                                                                                                              |
| EP04         | Gestión de Gastos Compartidos     | TS09      | Implementar actualización y eliminación de gastos         | Como desarrollador, quiero poder actualizar o eliminar gastos.                                                         | - **Escenario 1: Actualización**<br> Dado que el gasto existe,<br> Cuando el administrador envía nuevos datos,<br> Entonces el backend actualiza el registro.<br>- **Escenario 2: Eliminado**<br> Dado que el administrador solicita borrar,<br> Cuando el backend elimina el gasto,<br> Entonces deja de aparecer en futuros reportes.                                                                                                                                                                                                             |
| EP04         | Gestión de Gastos Compartidos     | TS10      | Verificar integración de gastos                           | Como desarrollador, quiero verificar que el backend de gastos esté correctamente conectado al app.                | - **Escenario 1: Mostrar lista de gastos**<br> Dado que haya gastos registrados,<br> Cuando el usuario acceda a la sección de gastos,<br> Entonces se mostrará la información proveniente del backend.<br><br> - **Escenario 2: Agregar gasto**<br> Dado que se complete el formulario,<br> Cuando se presione "Guardar",<br> Entonces se guardará mediante la API y se actualizará la vista.                                                                                                                                                       |
| EP05         | Seguimiento y Recordatorios       | US21      | Recordatorios de pago                                     | Como usuario, quiero recibir recordatorios automáticos de pago para no retrasarme en mis aportes.                      | - **Escenario 1: Activación del recordatorio**<br> Dado que el usuario tenga una fecha límite de pago,<br> Cuando se acerque esa fecha,<br> Entonces recibirá una notificación automática por correo o en la app.<br><br> - **Escenario 2: Configuración**<br> Dado que acceda a ajustes,<br> Cuando edite preferencias,<br> Entonces podrá activar o desactivar los recordatorios.                                                                                                                                                                 |
| EP05         | Seguimiento y Recordatorios       | US22      | Alertas de pagos pendientes                               | Como usuario, quiero ser alertado si tengo pagos atrasados para regularizar mi situación.                              | - **Escenario 1: Detección automática**<br> Dado que el usuario no haya pagado después de la fecha límite,<br> Cuando acceda al sistema,<br> Entonces verá una alerta destacada en su panel.<br><br> - **Escenario 2: Alerta múltiple**<br> Dado que haya varios pagos pendientes,<br> Cuando abra la alerta,<br> Entonces podrá ver el detalle de cada uno.                                                                                                                                                                                        |
| EP05         | Seguimiento y Recordatorios       | US23      | Recordatorio de actualización de ingresos                 | Como usuario, quiero ser recordado de actualizar mis ingresos para mantener la equidad del sistema.                    | - **Escenario 1: Periodicidad**<br> Dado que haya pasado un mes sin actualización,<br> Cuando el usuario inicie sesión,<br> Entonces verá un mensaje solicitando revisar su ingreso.<br><br> - **Escenario 2: Confirmación**<br> Dado que actualice el ingreso,<br> Cuando guarde los cambios,<br> Entonces se reiniciará el periodo de espera.                                                                                                                                                                                                     |
| EP05         | Seguimiento y Recordatorios       | US24      | Confirmación de aportes                                   | Como usuario, quiero recibir confirmación cada vez que realizo un aporte para mayor seguridad.                         | - **Escenario 1: Notificación inmediata**<br> Dado que el usuario registre un pago,<br> Cuando el sistema lo procese,<br> Entonces recibirá una confirmación por correo o notificación dentro de la app.<br><br> - **Escenario 2: Registro visible**<br> Dado que quiera revisar sus confirmaciones,<br> Cuando acceda al historial,<br> Entonces verá las confirmaciones pasadas.                                                                                                                                                                  |
| EP05         | Seguimiento y Recordatorios       | US25      | Notificación de cambios en el hogar                       | Como usuario, quiero ser notificado si hay cambios en el hogar para estar informado.                                   | - **Escenario 1: Nuevo miembro**<br> Dado que un nuevo miembro se una,<br> Cuando sea aprobado por el representante,<br> Entonces se notificará a todos los miembros.<br><br> - **Escenario 2: Cambios administrativos**<br> Dado que el representante edite los porcentajes de aporte,<br> Cuando se guarde el cambio,<br> Entonces se notificará a los afectados.                                                                                                                                                                                 |
| EP05         | Seguimiento y Recordatorios       | TS11      | API para programar recordatorios de pago                  | Como desarrollador, quiero dar de alta recordatorios específicos de pago en el backend.                                | - **Escenario 1: Crear recordatorio**<br> Dado que el administrador proporciona fecha y monto,<br> Cuando el backend graba el recordatorio,<br> Entonces el recordatorio queda incluido en la base de datos.<br>- **Escenario 2: Listar recordatorios**<br> Dado que el administrador consulta,<br> Cuando el backend responde,<br> Entonces proporciona la lista de recordatorios pendientes.                                                                                                                                                      |



### 2.4.2. Impact Mapping

### Segmento 1: Miembros del hogar

<p styles="align: left">
  <img src="assets/ImpactMappingSeg1.png" width="1100">
</p>


### Segmento 2: Representante del hogar

<p styles="align: left">
  <img src="assets/ImpactMappingSeg2.png" width="1100">
</p>

### 2.4.3. Product Backlog

| Prioridad | User Story ID | Título HU                                                 | Story Points |
| --------- | ------------- | --------------------------------------------------------- | ------------ |
| Alta      | US01          | Registro de usuario                                       | 8            |
| Alta      | US02          | Inicio de sesión seguro                                   | 5            |
| Alta      | TS01          | Implementar autenticación JWT                             | 8            |
| Alta      | TS02          | Cifrar contraseñas en base de datos                       | 5            |
| Alta      | TS03          | Validar roles de administrador y miembro en backend       | 8            |
| Alta      | TS05          | Conectar formularios con endpoints                        | 5            |
| Alta      | TS06          | Validar respuestas del backend                            | 3            |
| Media     | US03          | Edición de información personal                           | 5            |
| Media     | US04          | Cierre de sesión desde todos los dispositivos             | 5            |
| Media     | US05          | Configuración de notificaciones personales                | 5            |
| Media     | TS04          | Implementar actualización de perfil a partir de API       | 5            |
| Alta      | US06          | Crear hogar                                               | 8            |
| Alta      | US07          | Aprobar gastos                                            | 5            |
| Alta      | US08          | Ajustar porcentajes de aportes                            | 8            |
| Alta      | US09          | Visualizar reportes mensuales                             | 8            |
| Media     | US10          | Configurar métodos de pago aceptados                      | 5            |
| Media     | US14          | Ver historial de pagos (representante)                    | 5            |
| Media     | US36          | Manejar errores del servidor                              | 3            |
| Alta      | US11          | Ingresar ingresos personales                              | 5            |
| Alta      | US12          | Ver monto a pagar                                         | 5            |
| Alta      | US13          | Registrar pagos realizados                                | 5            |
| Media     | US15          | Ver historial de pagos (miembro)                          | 5            |
| Media     | US37          | Manejo de estados de carga y éxito                        | 3            |
| Alta      | US16          | Registrar nuevo gasto                                     | 8            |
| Media     | US17          | Adjuntar comprobantes de gasto                            | 5            |
| Media     | US18          | Clasificar gastos por categoría                           | 5            |
| Media     | US19          | Comentar o justificar un gasto                            | 3            |
| Media     | US20          | Visualizar gráficos de gastos                             | 8            |
| Alta      | TS07          | Validar que el gasto tenga adjunto al menos 1 comprobante | 5            |
| Media     | TS08          | Agregar API para filtrar gastos por rango de fecha        | 5            |
| Media     | TS09          | Implementar actualización y eliminación de gastos         | 8            |
| Media     | TS10          | Verificar integración de gastos                           | 5            |
| Media     | US21          | Recordatorios de pago                                     | 5            |
| Media     | US22          | Alertas de pagos pendientes                               | 5            |
| Baja      | US23          | Recordatorio de actualización de ingresos                 | 3            |
| Baja      | US24          | Confirmación de aportes                                   | 3            |
| Baja      | US25          | Notificación de cambios en el hogar                       | 3            |
| Media     | TS11          | API para programar recordatorios de pago                  | 5            |


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

- Link: https://miro.com/app/board/uXjVHfgsAFg=/?share_link_id=564858049353

<br>
<img src="assets/C1.png" alt="C1">
<br>

<br>
<img src="assets/C2.png" alt="C2">
<br>

<br>
<img src="assets/C3.png" alt="C3">
<br>

<br>
<img src="assets/C4.png" alt="C4">
<br>

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
