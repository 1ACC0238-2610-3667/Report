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
| **Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software.** |  **Héctor Rios:** Contribuí realizando el capítulo 1 y organizando las ideas para la continuación del proyecto <br><br> **Jose Luis Martínez Valdivia:** Contribui en El desarrollo del capitulo 2 - Strategic Level Domain Driven Design <br><br> **Joaquin Alberto Cuentas Peña:** Contribuí en El desarrollo del capítulo 2 – con el análisis de segmentos objetivos, entrevistas y elaboración de personas <br><br> **Walter Luis Fajardo Monrroy:** Contribuí en el desarrollo de diagramas, así como segmentación de bounded context  <br><br> **Rodrigo Jesus Miraval Pomalaya:** Contribui realizando parte del capítulo 2, con las user historias, el impact mapping y el product backlog. <br><br>|    **Héctor Rios** **TB1:** El desarrollo del capítulo 1 me permitió reforzar mis conocimientos sobre la estructura inicial de un proyecto de software. Sentí que este proceso me ayudó a entender mejor cómo plantear una base sólida, lo cual considero clave para mi crecimiento profesional. <br><br>   <br><br> **Jose Luis Martínez Valdivia:** El desarrollo del capitulo 2 me permitió comentar y enriquecer mis conocimientos de DDD y la forma en la que se debaten ideas para implementar una solución de Servicio Web <br><br> **Joaquin Alberto Cuentas Peña:** El desarrollo de este capítulo me permitió conocer la perspectiva de los usuarios que usarán la aplicación. <br><br>  **Walter Luis Fajardo Monrroy:** El desarrollo de este capítulo permitirá a los desarrolladores asignar los bounded context y hacer consultas de funcionamiento e interconexión. <br><br> **Rodrigo Jesus Miraval Pomalaya:** El desarrollo del capítulo 2 me permitió profundizar en la construcción de artefactos clave como las user historias, el impact mapping y el product backlog. A través de este proceso, logré entender mejor cómo traducir necesidades del negocio en requerimientos claros y estructurados, facilitando una mejor organización del trabajo y priorización de funcionalidades dentro del proyecto. <br><br>|
| **Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones detecnologías de ingeniería de software** | **Héctor Rios:** Contribuí realizando el capítulo 1,sedimentando las bases del proyecto <br><br> **Jose Luis Martínez Valdivia:** Contribui en El desarrollo del capitulo 2 - Strategic Level Domain Driven Design <br><br> **Joaquin Alberto Cuentas Peña:** Reconocí las necesidades de los usuarios a través de entrevistas, así como sus gustos y molestias <br><br> **Walter Luis Fajardo Monrroy:** Reconocí segmentos, funcionalidades y los convertí en bounded context para desarrollo  <br><br> **Rodrigo Jesus Miraval Pomalaya:** Contribui realizando parte del capítulo 2, con las user historias, el impact mapping y el product backlog. <br><br>| **Héctor Rios** **TB1:** A lo largo del desarrollo del capítulo 1, comprendí que siempre hay aspectos que mejorar y aprender. Esta experiencia me hizo reflexionar sobre la importancia de mantenerme en constante actualización para poder aportar mejor en futuros proyectos. <br><br> **Jose Luis Martínez Valdivia:** Durante El desarrollo de capitulo 2, logre entender los procesos y requerimientos que se deben llevar acabo para poder delimitar el alcance y arquitectura de desarrollo del proyecto a implementar <br><br> **Joaquin Alberto Cuentas Peña: :** Este conocimiento me permitió hacer un análisis y crear personas para enfocarnos en posibles requisitos funcionales <br><br> **Walter Luis Fajardo Monrroy:** El desarrollo de este capítulo me permitió aprender como segmentar bounded context en el contexto de desarrollo móvil <br><br> **Rodrigo Jesus Miraval Pomalaya:** Durante el desarrollo del capítulo 2, comprendí mejor cómo definir y organizar el alcance del proyecto. El uso de herramientas como el impact mapping y el product backlog me ayudó a estructurar las ideas, priorizar funcionalidades y tener una visión más clara del desarrollo del software.<br><br>|


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
