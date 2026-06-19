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
|--------------------|--------------------|--------------|
| Actualiza conceptos y conocimientos necesarios para su desarrollo profesional y en especial para su proyecto en soluciones de software | Héctor Rios - AV1: Contribuí realizando el capítulo 1 y organizando las ideas para la continuación del proyecto | Héctor Rios - AV1: El desarrollo del capítulo 1 me permitió reforzar mis conocimientos sobre la estructura inicial de un proyecto de software |
| | Héctor Rios - TB1: Reforcé la estructuración inicial del proyecto documentando y organizando los contenidos base | Héctor Rios - TB1: Comprendí la importancia de establecer bases sólidas para el desarrollo eficiente del proyecto |
| | Héctor Rios - AV2: Amplié la documentación del capítulo 1 incorporando mejoras en la definición del problema y objetivos | Héctor Rios - AV2: Consolidé mis conocimientos sobre la planificación estratégica del proyecto |
| | Jose Luis Martínez Valdivia - AV1: Contribuí en el desarrollo del capítulo 2 - Strategic Level Domain Driven Design | Jose Luis Martínez Valdivia - AV1: El desarrollo del capítulo 2 me permitió enriquecer mis conocimientos de DDD |
| | Jose Luis Martínez Valdivia - TB1: Apoyé en la definición estratégica del dominio y discusión de soluciones basadas en DDD | Jose Luis Martínez Valdivia - TB1: Fortalecí mi capacidad para debatir e implementar soluciones de servicios web |
| | Jose Luis Martínez Valdivia - AV2: Profundicé en la aplicación de patrones de DDD en el capítulo 2 | Jose Luis Martínez Valdivia - AV2: Mejoré mi comprensión sobre la aplicación práctica de DDD |
| | Joaquin Alberto Cuentas Peña - AV1: Contribuí en el desarrollo del capítulo 2 con análisis de segmentos objetivos, entrevistas y elaboración de personas | Joaquin Alberto Cuentas Peña - AV1: Conocí la perspectiva de los usuarios que usarán la aplicación |
| | Joaquin Alberto Cuentas Peña - TB1: Profundicé en el análisis de usuarios y construcción de perfiles enfocados en requisitos | Joaquin Alberto Cuentas Peña - TB1: Logré enfocar mejor los requisitos en función de las necesidades reales del usuario |
| | Joaquin Alberto Cuentas Peña - AV2: Refiné perfiles de usuario y validé segmentos objetivo | Joaquin Alberto Cuentas Peña - AV2: Logré mayor alineación entre usuario y requisitos |
| | Walter Luis Fajardo Monrroy - AV1: Contribuí en el desarrollo de diagramas y segmentación de bounded context | Walter Luis Fajardo Monrroy - AV1: Permitió asignar bounded context y comprender su interconexión |
| | Walter Luis Fajardo Monrroy - TB1: Elaboré diagramas adicionales para mejorar la comprensión de los contextos delimitados | Walter Luis Fajardo Monrroy - TB1: Mejoré mi entendimiento sobre la organización modular del sistema |
| | Walter Luis Fajardo Monrroy - AV2: Ajusté y optimicé diagramas de bounded context | Walter Luis Fajardo Monrroy - AV2: Fortalecí la integración entre contextos |
| | Rodrigo Jesus Miraval Pomalaya - AV1: Contribuí realizando parte del capítulo 2 con user historias, impact mapping y product backlog | Rodrigo Jesus Miraval Pomalaya - AV1: Profundicé en user historias, impact mapping y backlog |
| | Rodrigo Jesus Miraval Pomalaya - TB1: Apoyé en la estructuración de requerimientos y priorización mediante herramientas ágiles | Rodrigo Jesus Miraval Pomalaya - TB1: Comprendí mejor la traducción de necesidades del negocio en requisitos claros |
| | Rodrigo Jesus Miraval Pomalaya - AV2: Mejoré la priorización del backlog | Rodrigo Jesus Miraval Pomalaya - AV2: Afianzé la estructuración ágil de requerimientos |
| Reconoce la necesidad del aprendizaje permanente para el desempeño profesional y el desarrollo de proyectos en soluciones de tecnologías de ingeniería de software | Héctor Rios - AV1: Contribuí realizando el capítulo 1, sedimentando las bases del proyecto | Héctor Rios - AV1: Comprendí la importancia de la actualización constante |
| | Héctor Rios - TB1: Fortalecí la documentación inicial del proyecto para su mejora continua | Héctor Rios - TB1: Reflexioné sobre el aprendizaje continuo como base del crecimiento profesional |
| | Héctor Rios - AV2: Revisé y actualicé la documentación con retroalimentación | Héctor Rios - AV2: Comprendí la importancia de la mejora continua |
| | Jose Luis Martínez Valdivia - AV1: Contribuí en el desarrollo del capítulo 2 - Strategic Level DDD | Jose Luis Martínez Valdivia - AV1: Entendí procesos para delimitar alcance y arquitectura |
| | Jose Luis Martínez Valdivia - TB1: Apoyé en la definición del alcance y arquitectura del proyecto | Jose Luis Martínez Valdivia - TB1: Mejoré mi criterio para planificar soluciones de software |
| | Jose Luis Martínez Valdivia - AV2: Ajusté la arquitectura según nuevas discusiones | Jose Luis Martínez Valdivia - AV2: Reforcé mi adaptabilidad en diseño de sistemas |
| | Joaquin Alberto Cuentas Peña - AV1: Reconocí necesidades de usuarios mediante entrevistas | Joaquin Alberto Cuentas Peña - AV1: Este conocimiento permitió crear personas y requisitos funcionales |
| | Joaquin Alberto Cuentas Peña - TB1: Analicé datos de usuarios para definir posibles funcionalidades | Joaquin Alberto Cuentas Peña - TB1: Fortalecí la identificación de necesidades del usuario |
| | Joaquin Alberto Cuentas Peña - AV2: Validé necesidades con enfoque iterativo | Joaquin Alberto Cuentas Peña - AV2: Fortalecí el aprendizaje basado en feedback |
| | Walter Luis Fajardo Monrroy - AV1: Reconocí segmentos y los convertí en bounded context | Walter Luis Fajardo Monrroy - AV1: Aprendí a segmentar bounded context |
| | Walter Luis Fajardo Monrroy - TB1: Profundicé en la organización de funcionalidades por contexto | Walter Luis Fajardo Monrroy - TB1: Consolidé mi conocimiento en arquitectura basada en contextos |
| | Walter Luis Fajardo Monrroy - AV2: Reorganicé contextos según mejoras | Walter Luis Fajardo Monrroy - AV2: Consolidé conocimientos en arquitectura evolutiva |
| | Rodrigo Jesus Miraval Pomalaya - AV1: Contribuí en user historias, impact mapping y backlog | Rodrigo Jesus Miraval Pomalaya - AV1: Comprendí cómo organizar el alcance del proyecto |
| | Rodrigo Jesus Miraval Pomalaya - TB1: Refiné la priorización del desarrollo | Rodrigo Jesus Miraval Pomalaya - TB1: Mejoré la estructuración del trabajo |
| | Rodrigo Jesus Miraval Pomalaya - AV2: Reestructuré backlog según nuevas prioridades | Rodrigo Jesus Miraval Pomalaya - AV2: Fortalecí la mejora continua en ágiles |


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
    * `ITokenService`: Define el contrato para la gestión de la seguridad basada en tokens. Es responsable de la generación, firma y validación de los JSON Web Tokens (JWT) utilizados para autorizRamírezsolicitudes desde la aplicación móvil.
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

![Diagrama de componentes IAM](assets/IAM%20-%20diagraman%20-%20componentes.png)

### 2.6.1.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.1.6.1 Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio representa el modelo conceptual de negocio para el contexto de **Identity and Access Management (IAM)**. En este esquema se visualizan las entidades fundamentales, como `User` (Aggregate Root) y `Role`, junto con sus atributos esenciales y las relaciones que definen el comportamiento del sistema de identidades. 

Este modelo se mantiene estrictamente agnóstico a factores externos, como la persistencia en base de datos o los protocolos de comunicación, centrándose únicamente en las reglas de dominio que rigen la creación y validación de usuarios y sus niveles de acceso dentro de la plataforma **Splitly**.

![Diagrama de Clases del Dominio](assets/diagram-class-IAM.png)

#### 2.6.1.6.2 Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos (Entity-Relationship) estructurado específicamente para el contexto de **Identity and Access Management (IAM)**. 

En este esquema se visualiza la estructura relacional de las tablas empleadas para la persistencia de identidades y accesos, aislando las tablas `users`, `roles` y la tabla de resolución `user_roles`. Se especifican los atributos, las claves primarias (PK) y las claves foráneas (FK) que garantizan la integridad referencial y modelan correctamente la asignación de permisos a los usuarios registrados en la plataforma **Splitly**.

![Diagrama de Base de Datos](assets/diagram-BD-IAM.png)

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

![Diagrama de Componentes Contributions Distribution](assets/component-diagram-Contributions%20Distribution.png)


### 2.6.2.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.2.6.1 Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio ilustra el modelo conceptual de negocio estructurado específicamente para el Bounded Context de **Contributions Distribution**. 

En este esquema se visualizan las entidades centrales que conforman este límite transaccional, destacando los Aggregate Roots (`Expense` y `Contribution`) y sus entidades relacionadas (`ExpenseLine`, `Payment`, `ContributionItem`). Se detallan sus atributos esenciales, métodos de comportamiento (como `recompute()` y `registerPayment()`) y las multiplicidades que rigen las reglas de división de gastos y liquidación de deudas.

Al omitir intencionalmente detalles de infraestructura y dependencias externas, este modelo demuestra una alta cohesión interna y se mantiene estrictamente agnóstico a frameworks de persistencia o interfaces de usuario, cumpliendo fielmente con los principios tácticos de Domain-Driven Design (DDD).

![Diagrama de contexto Contributions Distribution](assets/diagrama%20-%20context%20domain%20-%20distribution%20contribution.png)


#### 2.6.2.6.2 Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos (Entity-Relationship) estructurado específicamente para dar soporte a la persistencia del Bounded Context de **Contributions Distribution**. 

En este esquema se aíslan las tablas responsables de almacenar la información financiera y transaccional del módulo. Se observan las tablas `bills` (que materializa el agregado de gastos), `contributions` (que almacena las cuotas proporcionales calculadas mediante las políticas de reparto) y `member_contributions` (que registra el estado de los pagos y liquidaciones de cada usuario).

El diagrama detalla los atributos físicos, los tipos de datos implícitos, las claves primarias (PK) y las relaciones de clave foránea (FK) que garantizan la integridad referencial de las reglas de negocio finacieras de **Splitly**, manteniendo este esquema lógicamente separado de otros dominios como la gestión de identidades o el ciclo de vida de los hogares.

![Diagrama de base de datos Contributions Distribution](assets/diagrama%20-%20base%20de%20datos%20-%20contribution%20distributions.png)

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

![Diagrama de componentes Household Management](assets/Household%20Management%20-%20component%20diagram.png)

### 2.6.3.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.3.6.1. Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio ilustra el modelo conceptual de negocio estructurado específicamente para el Bounded Context de **Household Management**. Este esquema visualiza las entidades centrales y Aggregate Roots que conforman este límite transaccional, respetando estrictamente los principios tácticos de Domain-Driven Design (DDD).

En el modelo se identifica a `Household` como el Aggregate Root principal, responsable de mantener la consistencia del grupo u hogar. A esta raíz se asocian de manera transaccional las entidades subordinadas `HouseholdMember` (que define el vínculo usuario-hogar y su rol interno) e `Invitation` (que gestiona el ciclo de vida de los accesos organizativos). 

Se detallan además los enumeradores necesarios (`HouseholdRole`, `InvitationStatus`) y los métodos de comportamiento (tales como `Accept()`, `AddMember()` o `CreateInvitation()`), asegurando un modelo cohesivo que permanece agnóstico de frameworks externos o detalles de persistencia.

![Diagrama de contexto Household Management](assets/Household%20Management%20BC%20-%20diagram%20-%20context.png)

#### 2.6.3.6.2. Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos estructurado específicamente para dar soporte al Bounded Context de **Household Management**. Este esquema aísla las tablas responsables de almacenar la estructura organizativa de los grupos dentro de la plataforma.

En el diagrama se observa la tabla principal `households` (que almacena los metadatos de los grupos), relacionada mediante claves foráneas (FK) con las tablas subordinadas `household_members` (que registra la unión de los usuarios con el grupo y sus roles locales) e `invitations` (que persiste los tokens de acceso temporales y su estado de vigencia). 

Este diseño garantiza la integridad referencial de la organización de los equipos, manteniendo estas tablas lógicamente separadas de otros dominios de la base de datos, como las transacciones financieras o la gestión global de identidades (IAM).

![Diagrama de base de datos Household Management](assets/diagrama%20-%20base%20de%20datos%20-%20Household%20Management.png)

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

![Diagrama de componentes App Management](assets/BC%20App%20-%20diagrama%20-%20componentes.png)

### 2.6.4.6. Bounded Context Software Architecture Code Level Diagrams

#### 2.6.4.6.1. Bounded Context Domain Layer Class Diagrams

El siguiente diagrama de clases de la capa de dominio ilustra el modelo conceptual diseñado para el Bounded Context de **App Management**. Este esquema visualiza las entidades y Aggregate Roots responsables de gestionar la infraestructura transversal de la aplicación, incluyendo las preferencias del usuario y la integración con las pasarelas de pago.

El modelo se divide en dos enfoques principales:
* Por un lado, `UserSetting` actúa como un Aggregate Root aislado que centraliza la personalización de la experiencia del usuario (idioma, tema visual y notificaciones).
* Por otro lado, se definen los elementos del sub-dominio de pagos, donde `PaymentIntent` (Aggregate Root) orquesta el ciclo de vida de una transacción financiera, y se relaciona de manera segura con `PaymentMethodProfile`. Esta última entidad es crítica para la seguridad (cumplimiento PCI-DSS), ya que únicamente almacena el token externo (`ExternalToken`) provisto por el proveedor de pagos, en lugar de los datos sensibles de la tarjeta.

El diseño asegura que la lógica de cobros y configuraciones permanezca fuertemente tipada a través de enumeradores como `TransactionStatus` y `ThemePreference`, manteniendo el dominio limpio de implementaciones tecnológicas específicas.

![Diagrama de clases App Management](assets/app%20%20BC%20-%20diagrama%20contexto.png)

#### 2.6.4.6.2. Bounded Context Database Design Diagram

El siguiente diagrama representa el modelo físico de datos estructurado para el Bounded Context de **App Management**. Este esquema aísla las tablas responsables de almacenar las preferencias transversales de la aplicación y el registro histórico de la interacción con la pasarela de pagos.

En el diagrama se observan tres tablas principales, todas fuertemente vinculadas al identificador del usuario (delegado del módulo IAM):
* **`user_settings`**: Almacena las preferencias de localización y experiencia visual (idioma, tema y notificaciones).
* **`payment_transactions`**: Funciona como un registro auditable de los intentos de cobro, guardando el monto, la moneda, el estado de la transacción y, de forma crucial, el `external_transaction_id` que permite la conciliación con el proveedor externo (ej. Stripe).
* **`payment_methods`**: Almacena los perfiles de pago del usuario cumpliendo con los estándares de seguridad (PCI-DSS). No guarda datos sensibles, sino únicamente el `external_token` provisto por la pasarela y los últimos 4 dígitos de la tarjeta (`card_last_4`) para fines de visualización en la interfaz.

Este diseño asegura que el núcleo del negocio esté completamente separado de la configuración técnica y de los detalles de infraestructura de cobros.

![Diagrama de base de datos App Management](assets/base%20de%20datos%20-%20diagrama%20-%20app%20BC.png)

# Capítulo IV: Product Implementation & Validation
## 4. Product Implementation & Validation

### 4.1. Software Configuration Management

#### 4.1.1. Software Development Environment Configuration

En esta sección, se explica los entornos en donde se decidió llevar a cabo el ciclo de vida de desarrollo de los productos de software relacionados al proyecto del curso.

* **Project Management**

  - En el aspecto de gestión y desarrollo del ciclo de vida del proyecto se utilizó la aplicación DISCORD y GOOGLE MEET para las reuniones de grupo en las cuales se conversan sobre temas relacionados a avances y corrección de aspectos del proyecto. Además, para la documentación del proyecto, se utilizó el formato Mark Down en un repositorio de GitHub para el control de versiones del informe.

* **Requirements Management**

  - Para el manejo de los requisitos (historias de usuario, product backlog, sprint backlog) del producto, se utilizó TRELLO la cual es una herramienta ideal para gestionar proyectos. Además, usando esta herramienta, se puede organizar un product backlog, ya que permite estructurar tareas visualmente en un tablero. También puedes crear listas que representen etapas del flujo de trabajo, y en cada lista añadir tarjetas que describan las user stories o tareas individuales. Estas tarjetas permiten detallar información clave, como prioridades, etiquetas de color, descripciones y checklists, facilitando así el seguimiento y la colaboración del equipo.

* **Product UX/UI Design**

  - Para el desarrollo de plantillas de los user persona, de los Impact Maps y los User Journey Maps se utilizó la aplicación UXPRESSIA la cual es una plataforma especializada en la creación de mapas de experiencia del usuario ofreciendo una interfaz enfocada exclusivamente en UX que facilita la estructuración clara y profesional de estos elementos. Destaca por sus plantillas personalizables, la posibilidad de añadir datos reales, imágenes y métricas, y por permitir la colaboración en tiempo real.

  - Para la creación del Lean UX Canvas se utilizó la aplicación de diseño CANVA. Esta aplicación es una herramienta versátil para crear diversos diseños. Canva facilita la colaboración del equipo y la exportación de los proyectos en archivo PNG o PDF, manteniendo el proceso creativo ordenado y atractivo. Para los Journey Mapping, Empathy Mapping, entre otros mapas,  se decidió utilizar Miro. Esta aplicación permite una colaboración en tiempo real entre equipos, ofrece una interfaz visual e intuitiva, y cuenta con plantillas prediseñadas que agilizan el proceso sin perder calidad metodológica.

  - Finalmente, para el desarrollo de interfaces de usuario (wireframes, mockups y prototipos de aplicación) se decidió utilizar FIGMA. Esta es una herramienta que facilita el diseño de interfaces, permitiéndonos trabajar con colores, imágenes, formas, y otros elementos visuales para crear nuestra aplicación. Nos ofrece la posibilidad de probar diversos modelos de dispositivos. Además, esta plataforma será clave en la creación de nuestro prototipo, ya que brinda una simulación interactiva que permite visualizar y experimentar el proyecto desde la perspectiva del usuario.

* **Software Development**

  - Para el desarrollo del producto de software correspondiente al Landing Page, se utilizarán dos aplicaciones, las cuales son GITHUB y JETBRAINS WEBSTORM. La primera ayuda al equipo a gestionar de manera correcta los avances colaborativos del proyecto. Por otro lado, JetBrains WebStorm ayudará a trabajar el proyecto con lenguajes como HTML5, CSS y JavaScript para el desarrollo del landing page.
 
* **Software Testing**

  - Las pruebas de la Landing Page se realizarán mediante uso del navegador web GOOGLE para verificar que el diseño del mismo cumple con aspectos como el diseño responsivo en cualquier dispositivo desde el que se acceda al landing page del proyecto. Además, para visualizar que se han implementado correctamente elementos visuales que deben aparecer en las distintas secciones de la página.

* **Software Deployment**

  - Para los despliegues de la Landing Page se uso el servicio web de GITHUB PAGES, este servicio se especializa en el despliegue de sitios web staticos directamente desde un repositorio creado en GitHub.

#### 4.1.2. Source Code Management

En esta sección, se describen los medios y esquemas de organización para gestionar de manera efectiva los archivos de proyecto relacionados a Landing Page, Web Services y Frontend Web Applications. En el caso de los repositorios, se usará GitHub para almacenar los archivos. Además, se implementará GitFlow. Esta función de GitHub ayudará al equipo, gracias a las ramas de características de lanzamiento, a poder trabajar paralelamente en el proyecto y a tomar el control de versiones de avance del proyecto.

##### 4.1.2.1. Repositorios

A continuación, se adjuntan los enlaces para acceder a los repositorios donde se almacenarán los archivos y avances de proyecto relacionados al Landing Page, Front-End y Back-End Application.

* **Landing Page: [https://github.com/1ACC0238-2610-3667/Landing-Page](https://github.com/1ACC0238-2610-3667/Landing-Page)**
* **Front End: [https://github.com/1ACC0238-2610-3667/Mobile-App](https://github.com/1ACC0238-2610-3667/Mobile-App)**
* **Backend: [https://github.com/1ACC0238-2610-3667/BackEnd](https://github.com/1ACC0238-2610-3667/BackEnd)**

##### 4.1.2.2. GitFlow

Para el desarrollo de este proyecto, GITFLOW ayudará al equipo de desarrollo a gestionar de manera efectiva el proyecto en su ciclo de vida. En general, GITHUB ayudará a facilitar el desarrollo del proyecto para el equipo ya que es más sencillo desarrollar trabajos en equipo en los repositorios de los archivos de proyecto.

##### 4.1.2.2.1. Main Branches

* **Main Branch**   
  Llamada también rama principal del proyecto, esta es la rama predeterminada del proyecto creado en el repositorio. Esta rama representa el historial del proyecto lo que ayuda a llevar el control de versiones del mismo.
    
* **Develop Branch**  
  Llamada también rama de desarrollo del proyecto. Esta rama es una bifurcación de código original del proyecto para definir nuevos rumbos respecto del proyecto original que servirá para evaluar variaciones del proyecto para su evolución. Además, ayudan a incorporar nuevas funciones al proyecto.

##### 4.1.2.2.2. Supporting Branches

* **Feature Branch**  
  También llamada rama de característica del proyecto, es una rama de desarrollo que ayuda a incorporar nuevas funciones al proyecto en desarrollo. Además, permite el aislamiento de la función agregada y que varios colaboradores puedan trabajar simultáneamente en dicha funcionalidad.

* **Release Branch**  
  También llamada rama de lanzamiento del proyecto, es una versión de código del proyecto que se usa para empezar un nuevo ciclo de lanzamiento del producto de software. Además, en esta rama se pueden realizar correcciones de errores de la versión pasada del proyecto. Finalmente, una vez terminada con esta rama, se suma a la rama principal del proyecto y se le asigna un nuevo número de versión de proyecto.
    
* **Hotfix Branch**  
  También llamada rama de corrección del proyecto, es una rama que permite dar mantenimiento al código del proyecto. Se utiliza principalmente para arreglar errores en alguna sección del producto de software de manera rápida.

##### 4.1.2.3. Release Versioning Conventions

Para la nomenclatura de los lanzamientos de la Landing Page, se utilizará Semantic Versioning que consta de tres partes para describir cambios mayores, cambios menores y parches para corrección de bugs, según la siguiente estructura:

* Número principal: Incrementa cuando se realiza un cambio mayor y significativo al proyecto.  
* Número secundario: Incrementa cuando se realiza un cambio menor al proyecto como arreglo de errores o agregación de características.  
* Número terciario: Incrementa cuando se realiza un parche al proyecto como una corrección de bugs o errores visuales.

##### 4.1.2.3. Commits Conventions

Para los textos de mensajes en los *‘commits’* del proyecto en Git, se utilizará Conventional Commits. Estos son mensajes de confirmación que son fáciles de entender por los colaboradores del proyecto. Finalmente, estos mensajes siguen la siguiente estructura:

<!-- Commits-->
<p align="center">
  <img src="https://i.imgur.com/vfirypa.png" alt="Commits">
</p>

La sección *‘type’* indica el tipo de mensaje de confirmación que se usará. A continuación, la sección *‘description’* indica la descripción que se le agrega al mensaje de confirmación, por ejemplo, una característica agregada. Además, la sección *‘body’* incluye una descripción más detallada del cambio aplicado al proyecto.  
Luego, se tienen distintos tipos de mensajes de confirmación. Por ejemplo, se tiene el mensaje tipo *‘fix’* que incluye una corrección al proyecto. Utilizar este tipo conlleva aumentar el número terciario de la versión del proyecto (por ejemplo, de 1.0.0. a 1.0.1.). Después, utilizar el mensaje de tipo *‘feat’* conlleva agregar una nueva función a la aplicación, por lo tanto, se debe aumentar el número secundario de la versión (por ejemplo, de 1.0.0. a 1.1.0.). Finalmente, si se agrega una sección de tipo ‘BREAKING CHANGE’ indicaría que las versiones anteriores del proyecto dejarán de ser compatibles entre sí, lo que conlleva un cambio significativo y el aumento del número principal de la versión (por ejemplo, de 1.0.0. a 2.0.0.).

#### 4.1.3. Source Code Style Guide & Conventions

En esta sección, se definen las referencias que se usaron para adoptar estrategias de nomenclatura de elementos de programación en los lenguajes y tecnologías que se usarán para la solución móvil (**Kotlin, C#, Android Studio y SQLite**). En general, la nomenclatura de los archivos y secciones en la programación se hará en inglés.

* **Nomenclatura en Kotlin:** Para la codificación del aplicativo móvil en Kotlin, se utilizará el documento oficial *“Kotlin Coding Conventions”.* Este artículo contiene información útil y necesaria para conocer cómo debe ser la nomenclatura de los diversos aspectos que conforman un proyecto desarrollado en Kotlin, abarcando desde la capitalización de clases y variables hasta el formato y diseño del código idiomático.  
  **Referencia:** [https://kotlinlang.org/docs/coding-conventions.html](https://kotlinlang.org/docs/coding-conventions.html)  
  Finalmente, se aplicará el contenido del artículo para el desarrollo del Front-End de la aplicación móvil de Harmonix.

* **Nomenclatura en Android Studio (Recursos y XML):** Para la organización del proyecto y diseño de interfaces en Android Studio, se utilizará la documentación *“App resources overview”* y las guías de estilo para desarrolladores de Android. Estos documentos contienen información sobre cómo nombrar correctamente los archivos de recursos (layouts, strings, drawables, colores) usando convenciones como *snake_case* y los prefijos adecuados para las vistas en XML.  
  **Referencia:** [https://developer.android.com/guide/topics/resources/providing-resources](https://developer.android.com/guide/topics/resources/providing-resources)  
  Finalmente, se aplicará el contenido para la estructuración visual e internacionalización de la aplicación móvil a desarrollar.

* **Nomenclatura en C#:** Para la codificación del proyecto en C#, se utilizará el artículo *“C# Coding Conventions”.* Este artículo contiene información útil y necesaria para conocer cómo debe ser la nomenclatura de los diversos aspectos que conforman un proyecto desarrollado en C#, según las convenciones oficiales de codificación establecidas por Microsoft. Se trata de la guía de convenciones de estilo de código para C# publicada por Microsoft, la cual proporciona una serie de recomendaciones para escribir código claro, coherente y mantenible en aplicaciones .NET.  
  **Referencia:** [https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions)  
  Finalmente, se aplicará el contenido del artículo para los Web Services de Harmonix.

* **Nomenclatura en ASP.NET:** Para la codificación del proyecto en ASP.NET, se utilizará el artículo *“Microsoft ASP.NET Core Coding Guidelines”.* Este artículo contiene información útil y necesaria para conocer cómo debe ser la nomenclatura y el estilo de los diversos aspectos que conforman un proyecto desarrollado con ASP.NET Core. Se trata de la guía de ingeniería oficial del equipo de ASP.NET Core, en la cual se detallan las convenciones recomendadas para escribir código claro, consistente y fácil de mantener.  
  **Referencia:** [https://github.com/dotnet/aspnetcore/wiki/Engineering-guidelines#codingguidelines](https://github.com/dotnet/aspnetcore/wiki/Engineering-guidelines#codingguidelines)  
  Finalmente, se aplicará el contenido del artículo para los Web Services de Harmonix.

* **Nomenclatura para RESTful API:** Para la nomenclatura de endpoints a implementar en la aplicación Back-End, se usó el artículo *"REST API URI Naming Conventions and Best Practices".* Este mismo contiene información sobre consejos y buenas prácticas al momento de nombrar correctamente a los endpoints en una aplicación back-end que use el esquema REST.  
  **Referencia:** [https://restfulapi.net/resource-naming/](https://restfulapi.net/resource-naming/)

* **Nomenclatura en SQLite:** Para la nomenclatura de objetos en la base de datos local embebida usando SQLite, se utilizará la guía *"SQL Style Guide"*. Dado que SQLite es altamente flexible, adoptar un estándar de la industria asegura una correcta nomenclatura de tablas, columnas y llaves foráneas consistentes. Este documento detalla las mejores prácticas como el uso de *snake_case* y sustantivos colectivos.  
  **Referencia:** [https://www.sqlstyle.guide/](https://www.sqlstyle.guide/)  
  Finalmente, se aplicará el contenido para el diseño y persistencia de datos locales dentro de la aplicación móvil de Harmonix.

#### 4.1.4. Software Deployment Configuration

En esta sección, se especifica la configuración para realizar el despliegue de la solución en el repositorio. Para realizar esto, se usó GITHUB PAGES para desplegar el landing page.

## Sitio web estático ##
* **Paso 1: Creación del repositorio**  
  Como primer paso, se debe crear el repositorio en GitHub que será el lugar donde se aloja todo lo relacionado al Landing Page.

* **Paso 2: Carga de archivos necesarios**  
  Como segundo paso, se importan todos los archivos necesarios para el desarrollo de la landing page como imágenes, archivos HTML, CSS y JavaScript.

* **Paso 3: Preparar el lanzamiento**  
  Como tercer paso, se juntan todas las características del proyecto en una sola para verificar el correcto funcionamiento de cada una. Luego, se envía todo a la rama principal donde se encuentra, por defecto, el proyecto.

* **Paso 4: Desplegar la Landing Page**  
  Como cuarto paso, cuando todo se encuentre en la rama principal, se accede a la sección Configuración del repositorio, luego, se selecciona la opción “GitHub Pages” y se seleccionará la rama principal que es la que se desea desplegar.

* **Paso 5: Acceder al Landing Page**  
  Como paso final, el entorno otorgará un enlace para poder acceder al proyecto desplegado.
  
![Link del despliegue](assets/landing%20page.png)

![Pagina desplegada](assets/despliegue.png)

## Despliegue del Backend en Render ##

* **Paso 1: Creación del servicio y conexión** Como primer paso, se crea un nuevo "Web Service" dentro de la plataforma de Render y se conecta con el repositorio de GitHub que contiene el código del backend, seleccionando la rama principal (`main`).

* **Paso 2: Configuración general y entorno** Como segundo paso, se le asigna un nombre al servicio (en este caso, *Splitly-Mobile-Backend*) y se selecciona **Docker** como el entorno de ejecución para el proyecto.

* **Paso 3: Configuración del Dockerfile** Como tercer paso, se le indica a Render dónde encontrar las instrucciones para construir el proyecto. Se especifica la ruta del archivo Docker (en el *Dockerfile Path* como `com.split.backend/Dockerfile`) y el directorio base (*Build Context* como `.`).

* **Paso 4: Variables de Entorno** Como cuarto paso, se accede a la sección "Environment" para configurar de forma segura las variables de entorno que necesita el backend para funcionar, como las cadenas de conexión a la base de datos (`ConnectionStrings`).

* **Paso 5: Construcción y Despliegue** Como paso final, Render lee el Dockerfile, construye la imagen y realiza el despliegue automáticamente, otorgando una URL pública para acceder a la API desplegada en producción.

![Despliegue 1](assets/A1.jpeg)

![Despliegue 1](assets/A2.jpeg)

![Despliegue 1](assets/A3.jpeg)

![Despliegue 1](assets/A4.jpeg)


### 4.2. Landing Page & Mobile Application Implementation

* **Paso 1: Creación del repositorio**  
  Como primer paso, se debe crear el repositorio en GitHub que será el lugar donde se aloja todo lo relacionado al Landing Page.

<p align="center">
  <img src="https://i.imgur.com/qpvh4Zt.png" alt="Repository creation">
</p>

* **Paso 2: Carga de archivos necesarios**  
  Como segundo paso, se importan todos los archivos necesarios para el desarrollo de la landing page como imágenes, archivos HTML, CSS y JavaScript.

<p align="center">
  <img src="https://i.imgur.com/KC9BrHf.png" alt="File organization">
</p>

* **Paso 3: Preparar el lanzamiento**  
  Como tercer paso, se juntan todas las características del proyecto en una sola para verificar el correcto funcionamiento de cada una. Luego, se envía todo a la rama principal donde se encuentra, por defecto, el proyecto.

<p align="center">
  <img src="https://i.imgur.com/LZxoPlI.png" alt="Master branch">
</p>

* **Paso 4: Desplegar la Landing Page**  
  Como cuarto paso, cuando todo se encuentre en la rama principal, se accede a la sección Configuración del repositorio, luego, se selecciona la opción “GitHub Pages” y se seleccionará la rama principal que es la que se desea desplegar.

<p align="center">
  <img src="https://i.imgur.com/9dbeFRr.png" alt="List of deployments.">
</p>

* **Paso 5: Acceder al Landing Page**  
  Como paso final, el entorno otorgará un enlace para poder acceder al proyecto desplegado.
  
![Despliegue](assets/splity.jpg)

#### 4.2.1. Sprint 1

A continuación, se presenta el Sprint Planning 1, donde se incluyen las evidencias de planificación e implementación del Landing Page, Mobile App y Backend. También se registran los avances del proyecto e insights de colaboración del equipo a través de GitHub.

##### 4.2.1.1. Sprint Planning n

| **Campo**                              | **Descripción**                                                                                                                                                                                                                                                                                                    |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Sprint #**                           | Sprint 1                                                                                                                                                                                                                                                                                                           |
| **Sprint Planning Background**         |                                                                                                                                                                                                                                                                                                                    |
| **Date**                               | 2026-05-04                                                                                                                                                                                                                                                                                                         |
| **Time**                               | 03:00 PM (GMT -5)                                                                                                                                                                                                                                                                                                  |
| **Location**                           | Modalidad remota por Google Meet                                                                                                                                                                                                                                                                                   |
| **Prepared By**                        | Testigos de Splitly                                                                                                                                                                                                                                                                                              |
| **Attendees (to planning meeting)**    | Equipo Splitly                                                                                                                                                                                                                                                            |
| **Sprint 0 Review Summary**        | Este es el primer sprint, por lo tanto, no hay una revisión de sprint anterior.                                                                                                                                                                                                                                    |
| **Sprint 0 Retrospective Summary** | Al ser el inicio del proyecto, se identificaron aspectos técnicos por aprender, como el uso de frameworks CSS. Se revisó el diseño del Landing Page en Figma, el desarrollo de las pantallas de la Mobile App y el despliegue del backend. Se discutió el contenido a incluir y se definió el objetivo principal: lograr desplegar el Landing Page y Backend al final del sprint. |
| **Sprint Goal & User Stories**         |                                                                                                                                                                                                                                                                                                                    |
| **Sprint 1 Goal**                      | Desplegar un Landing Page y Backend funcional con diseño responsive y estructura definida, accesible públicamente.                                                                                                                                                                                        |
| **Sprint 1 Velocity**                  | 20                                                                                                                                                                                                                                                                                                                  |
| **Sum of Story Points**                | 10                                                                                                                                                                                                                                                                                                                  |




##### 4.2.1.2. Sprint Backlog 1

El Sprint Backlog 1 corresponde a la planificación inicial del desarrollo de la plataforma Splitly, donde se definieron y priorizaron las primeras funcionalidades clave para la Landing Page y la configuración básica de despliegue. En este sprint, el equipo trabajó en la implementación de secciones informativas que presentan los objetivos, beneficios y funcionalidades de la aplicación, así como en la incorporación de ejemplos visuales y accesos directos para el registro e inicio de sesión de usuarios.

Adicionalmente, se incluyeron tareas técnicas relacionadas con la documentación del despliegue y la configuración de monitoreo básico, asegurando que el proyecto cuente con una base sólida para futuras iteraciones.

El trabajo colaborativo del equipo se gestionó en la herramienta Trello, lo que permitió organizar, priorizar y dar seguimiento a cada tarea de manera eficiente.

Link al tablero de Trello: https://trello.com/invite/b/6a04a4676f2c78852edaeb1a/ATTI85b6ff75c99bfbde325e6f171ad6e8b4E226ADCE/splitly-sprint-backlog

| **User Story Id** | **Title** | **Task Id** | **Task Title** | **Description** | **Estimation (Hours)** | **Assigned To** | **Status** |
|------------------|----------|------------|---------------|-----------------|------------------------|-----------------|------------|
| US01 | Registro de usuario | T1 | Registro backend | Implementación de endpoint para registro de usuarios | 4 | Walter Ramirez | To-do |
| US02 | Inicio de sesión seguro | T1 | Login backend | Implementación de autenticación de usuarios | 4 | Héctor Ríos | To-do |
| US03 | Edición de información personal | T1 | Perfil usuario | Endpoint para edición de perfil | 3 | Jose Luis Martinez Validivia | To-do |
| US04 | Cierre de sesión global | T1 | Logout global | Invalidación de sesiones activas | 3 | Joaquin Cuentas | To-do |
| US05 | Configuración de notificaciones | T1 | Preferencias | Gestión de notificaciones del usuario | 3 | TBD | To-do |
| US06 | Crear hogar | T1 | Crear hogar | Endpoint para creación de hogar | 4 | Rodrigo Miraval | To-do |
| US07 | Aprobar gastos | T1 | Aprobación de gastos | Lógica para aprobación de gastos | 4 | Rodrigo Miraval | To-do |
| US08 | Ajustar aportes | T1 | Configuración aportes | Actualización de porcentajes | 3 | Rodrigo Miraval | To-do |
| US10 | Métodos de pago | T1 | Configuración pagos | Gestión de métodos habilitados | 3 | Joaquin Cuentas | To-do |
| US11 | Ingresar ingresos | T1 | Registro ingresos | Endpoint para ingresos personales | 3 | TBD | To-do |
| US12 | Ver monto a pagar | T1 | Cálculo aportes | Lógica de cálculo de pagos | 4 | Walter Ramirez | To-do |
| US13 | Registrar pagos | T1 | Registro pagos | Endpoint para registrar pagos | 3 | Joaquin Cuentas | To-do |
| US16 | Registrar gasto | T1 | Registro gasto | CRUD de gastos | 4 | Walter Ramirez | To-do |
| US18 | Categorizar gastos | T1 | Categorías | Clasificación y filtros | 3 | Héctor Ríos | To-do |
| US21 | Recordatorios de pago | T1 | Recordatorios | Sistema de notificaciones automáticas | 4 | Héctor Ríos | To-do |
| US24 | Confirmación de aportes | T1 | Confirmación pagos | Notificaciones post pago | 3 | Jose Luis Martinez Validivia | To-do |
| US25 | Notificación cambios hogar | T1 | Notificaciones hogar | Eventos de cambios en hogar | 3 | Jose Luis Martinez Validivia | To-do |
| US31 | Visualizar información general | T1 | Información general | Desarrollo sección introductoria | 2 | Jose Luis Martinez Validivia | Done |
| US32 | Funciones principales | T1 | Funciones principales | Explicación de funcionalidades | 2 | Héctor Ríos | Done |
| US33 | Beneficios del sistema | T1 | Beneficios | Mostrar ventajas del sistema | 2 | Joaquin Cuentas | Done |
| US35 | Botones acceso | T1 | Botones login/register | Accesos rápidos | 1 | Rodrigo Miraval | Done |
| US36 | Manejar errores servidor | T1 | Manejo errores | Mensajes de error backend | 2 | Walter Ramirez | To-do |


##### 4.2.1.3. Development Evidence for Sprint Review


- **Landing Page:**

|Repository Branch |  Commit Id  |  Commit Message | Commit Message Body | Commited on (Date)|
|-----------------|--------------|-----------------|---------------------|-------------------|
|Landing Page - develop   |   4c76760…f3dcfd9     |  chores(landingpage): added some translation words    |           |   10/05/2026 |
|Landing Page - develop   |    c62b615…4c76760     |  chore(landingpage): add completed landing page       |           |   11/05/2026 |
|Landing Page - reviews   |   c62b615…3c7fbde      |  feature(reviews): completed landing page-OurSystem - added HTML  |    |12/05/2026|
|Landing Page - home   |   c62b615…7769d76     |  feat: add section home structure and styling    |           |   12/05/2026 |
|Landing Page - about us   |   c62b615…3f0f246     |  update landing page about us   |           |   13/05/2026 |
| Landing Page - pricing |  c62b615…6a35cc4         |  feature(pricing): completed Reviews on an 80%  |    |      13/05/2026    |


- **Mobile App:**

| Repository Branch | Commit Id     | Commit Message                               | Commit Message Body | Commited on (Date) |
|------------------|--------------|-----------------------------------------------|---------------------|-------------------|
| Mobile App - develop | 3861935 | chore(): add sharedPreferences                 |                     | 11/05/2026 |
| Mobile App - develop | b151bf1 | chore(): add drawer and navigation bar        |                     | 11/05/2026 |
| Mobile App - develop | fc52f52 | chore(): add working login flow               |                     | 11/05/2026 |
| Mobile App - develop | bdb50ad | chore(): add entities models                  |                     | 10/05/2026 |
| Mobile App - develop | 023ad09 | chore(): add initial signup screen            |                     | 10/05/2026 |
| Mobile App - develop | fe8c024 | chore(): add new login screen styles          |                     | 10/05/2026 |
| Mobile App - develop | 3312219 | initial commit                                |                     | 10/05/2026 |

##### 4.2.1.4. Testing Suite Evidence for Sprint Review

Durante este sprint no se implementaron pruebas automatizadas (Unit Tests, Integration Tests ni Acceptance Tests), ya que el alcance definido por el equipo contemplaba únicamente la construcción de la Landing Page e implementacion parcial del Mobile App y Backend.

El objetivo principal del sprint fue realizar la Landing Page y Mobile App a nivel de diseño e implementar el backend a un 70%. Todo esto estableciendo la arquitectura modular y los bounded contexts principales del sistema Splitly.

En esta etapa aún no se contaba con un backend definitivo ni con los servicios reales, por lo que las pruebas automatizadas se reprogramaron para el siguiente sprint, donde se incluirán los Integration Tests y Acceptance Tests asociados a los módulos existentes.

Conclusión: La etapa de testing se limitó a verificaciones manuales de flujo, validación visual de componentes y pruebas de integración básicas.

No se realizaron commits relacionados a proyectos o archivos de testing automatizado, dado que esta funcionalidad no formaba parte del alcance planificado para el sprint actual.

##### 4.2.1.5. Execution Evidence for Sprint Review

Durante la realización de este sprint se logró la correcta elaboración y despliegue de la landing page, de igual manera se alcanzó a realizar las principales pantallas relacionadas al core de la aplicación. Asimismo, se logró el desarrollo y deploy del backend.

**Backend:**

<br>
<img src="assets/backend_evidence1.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/backend_evidence2.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/backend_evidence3.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/backend_evidence4.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/backend_evidence5.jpg" alt="CandidateContextDiscovery">
<br>

**Landing Page**

<br>
<img src="assets/landing_evidence1.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_evidence2.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_evidence3.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_evidence4.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_evidence5.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_evidence6.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_evidence7.jpg" alt="CandidateContextDiscovery">
<br>


##### 4.2.1.6. Services Documentation Evidence for Sprint Review

Durante el presente Sprint se implementó y documentó el conjunto de endpoints correspondientes a los módulos de la aplicación.
La documentación fue elaborada utilizando OpenAPI/Swagger, permitiendo describir de manera clara las operaciones disponibles, parámetros requeridos, ejemplos de requests y responses, así como los códigos de estado HTTP soportados.


### MemberContribution




| Endpoint                                                        | Acción Implementada                          | Método HTTP | Sintaxis de Llamada                                             | Parámetros                                        | Descripción del Response                                                                                            |
| --------------------------------------------------------------- | -------------------------------------------- | ----------- | --------------------------------------------------------------- | ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| `/api/v1/member_contribution`                                   | Obtener todas las contribuciones             | GET         | `/api/v1/member_contribution`                                   | No requiere parámetros                            | Retorna la lista completa de contribuciones registradas con información del miembro, monto, estado y fecha de pago. |
| `/api/v1/member_contribution`                                   | Registrar una nueva contribución             | POST        | `/api/v1/member_contribution`                                   | Body JSON: `contributionId`, `memberId`, `amount` | Crea una nueva contribución asociada a un miembro y retorna el objeto creado junto con su identificador y estado.   |
| `/api/v1/member_contribution/bycontributionid/{contributionId}` | Buscar contribuciones por ID de contribución | GET         | `/api/v1/member_contribution/bycontributionid/{contributionId}` | Path Parameter: `contributionId`                  | Retorna la información de las contribuciones asociadas al identificador de contribución especificado.               |
| `/api/v1/member_contribution/bymemberid/{memberId}`             | Buscar contribuciones por ID de miembro      | GET         | `/api/v1/member_contribution/bymemberid/{memberId}`             | Path Parameter: `memberId`                        | Retorna las contribuciones realizadas por un miembro específico.                                                    |
| `/api/v1/member_contribution/{id}`                              | Eliminar contribución                        | DELETE      | `/api/v1/member_contribution/{id}`                              | Path Parameter: `id`                              | Elimina la contribución indicada y retorna la información del recurso eliminado.                                    |



| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/member_contribution` | Ninguno | ```json { "id":"MC001","contributionId":"CON001","memberId":"MEM001","amount":150.0,"status":"PAID","payedAt":"2026-05-14T10:30:00" } ``` | `200 OK` |
| POST | `/api/v1/member_contribution` | Body: `contributionId`, `memberId`, `amount` | ```json { "contributionId":"CON001","memberId":"MEM001","amount":150.0 } ``` | `201 Created`, `400 Bad Request` |
| GET | `/api/v1/member_contribution/bycontributionid/{contributionId}` | Path: `contributionId` | ```json { "id":"MC001","contributionId":"CON001","memberId":"MEM001","amount":150.0,"status":"PAID","payedAt":"2026-05-14T10:30:00" } ``` | `200 OK` |
| GET | `/api/v1/member_contribution/bymemberid/{memberId}` | Path: `memberId` | ```json { "id":"MC001","contributionId":"CON001","memberId":"MEM001","amount":150.0,"status":"PAID","payedAt":"2026-05-14T10:30:00" } ``` | `200 OK` |
| DELETE | `/api/v1/member_contribution/{id}` | Path: `id` | ```json { "id":"MC001","contributionId":"CON001","memberId":"MEM001","amount":150.0,"status":"PAID","payedAt":"2026-05-14T10:30:00" } ``` | `200 OK`, `404 Not Found` |


### Invitation

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/invitations` | Crear invitación | POST | `/api/v1/invitations` | Body JSON: `email`, `householdId`, `description` | Registra una nueva invitación asociada a un hogar y correo electrónico. |
| `/api/v1/invitations/pending` | Obtener invitación pendiente | GET | `/api/v1/invitations/pending?email={email}&householdId={householdId}` | Query Params: `email`, `householdId` | Retorna la invitación pendiente asociada al correo y hogar especificados. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| POST | `/api/v1/invitations` | Body: `email`, `householdId`, `description` | ```json { "email":"user@mail.com","householdId":"HH001","description":"Invitation to join household" } ``` | `200 OK` |
| GET | `/api/v1/invitations/pending` | Query: `email`, `householdId` | ```json { "email":"user@mail.com","householdId":"HH001","description":"Invitation to join household","status":"PENDING" } ``` | `200 OK` |


### Authentication

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/authentication/sign-in` | Iniciar sesión | POST | `/api/v1/authentication/sign-in` | Body JSON: `email`, `password` | Autentica al usuario y retorna la información de acceso correspondiente. |
| `/api/v1/authentication/sign-up` | Registrar usuario | POST | `/api/v1/authentication/sign-up` | Body JSON: `email`, `password`, `name`, `role`, `plan`, `householdId` | Registra un nuevo usuario en el sistema y retorna la información creada. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| POST | `/api/v1/authentication/sign-in` | Body: `email`, `password` | ```json { "email":"user@mail.com","password":"123456" } ``` | `200 OK` |
| POST | `/api/v1/authentication/sign-up` | Body: `email`, `password`, `name`, `role`, `plan`, `householdId` | ```json { "email":"user@mail.com","password":"123456","name":"Juan Perez","role":"MEMBER","plan":1,"householdId":"HH001" } ``` | `200 OK` |


### User

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/user/user/{id}` | Obtener usuario por ID | GET | `/api/v1/user/user/{id}` | Path Parameter: `id` | Retorna la información del usuario asociado al identificador especificado. |
| `/api/v1/user` | Obtener todos los usuarios | GET | `/api/v1/user` | No requiere parámetros | Retorna la lista de usuarios registrados en el sistema. |
| `/api/v1/user/householdid/{mainHouseHoldId}` | Obtener usuarios por household | GET | `/api/v1/user/householdid/{mainHouseHoldId}` | Path Parameter: `mainHouseHoldId`, Query: `houseHoldId` | Retorna los usuarios asociados al household indicado. |
| `/api/v1/user/byemail/{emailAddress}` | Actualizar usuario por email | PUT | `/api/v1/user/byemail/{emailAddress}` | Path Parameter: `emailAddress`, Body JSON: `emailAddress`, `personName`, `password` | Actualiza la información del usuario asociado al correo especificado. |
| `/api/v1/user/byemail/{email}` | Eliminar usuario por email | DELETE | `/api/v1/user/byemail/{email}` | Path Parameter: `email` | Elimina el usuario asociado al correo especificado. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/user/user/{id}` | Path: `id` | ```json { "id":1,"email":"user@mail.com","personName":"Juan Perez" } ``` | `200 OK` |
| GET | `/api/v1/user` | Ninguno | ```json [ { "id":1,"email":"user@mail.com","personName":"Juan Perez" } ] ``` | `200 OK` |
| GET | `/api/v1/user/householdid/{mainHouseHoldId}` | Path: `mainHouseHoldId`, Query: `houseHoldId` | ```json [ { "id":1,"email":"user@mail.com","personName":"Juan Perez","householdId":"HH001" } ] ``` | `200 OK` |
| PUT | `/api/v1/user/byemail/{emailAddress}` | Path: `emailAddress`, Body: `emailAddress`, `personName`, `password` | ```json { "emailAddress":"user@mail.com","personName":"Juan Perez","password":"123456" } ``` | `200 OK` |
| DELETE | `/api/v1/user/byemail/{email}` | Path: `email` | ```json { "message":"User deleted successfully" } ``` | `200 OK` |


### UserIncome

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/user-income` | Crear ingreso de usuario | POST | `/api/v1/user-income` | Body JSON: `id`, `userId`, `income` | Registra un nuevo ingreso asociado a un usuario. |
| `/api/v1/user-income/{id}` | Obtener ingreso por ID | GET | `/api/v1/user-income/{id}` | Path Parameter: `id` | Retorna la información del ingreso asociado al identificador especificado. |
| `/api/v1/user-income/byuserid/{userId}` | Obtener ingreso por usuario | GET | `/api/v1/user-income/byuserid/{userId}` | Path Parameter: `userId` | Retorna los ingresos asociados al usuario especificado. |
| `/api/v1/user-income/byid/{id}` | Actualizar ingreso | PUT | `/api/v1/user-income/byid/{id}` | Path Parameter: `id`, Body JSON: `id`, `income` | Actualiza la información del ingreso asociado al identificador especificado. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| POST | `/api/v1/user-income` | Body: `id`, `userId`, `income` | ```json { "id":"UI001","userId":1,"income":2500.0 } ``` | `201 Created`, `400 Bad Request` |
| GET | `/api/v1/user-income/{id}` | Path: `id` | ```json { "id":"UI001","userId":1,"income":2500.0,"createdDate":"2026-05-14","updatedDate":"2026-05-14" } ``` | `200 OK` |
| GET | `/api/v1/user-income/byuserid/{userId}` | Path: `userId` | ```json { "id":"UI001","userId":1,"income":2500.0,"createdDate":"2026-05-14","updatedDate":"2026-05-14" } ``` | `200 OK` |
| PUT | `/api/v1/user-income/byid/{id}` | Path: `id`, Body: `id`, `income` | ```json { "id":"UI001","income":3000.0 } ``` | `200 OK`, `400 Bad Request`, `404 Not Found` |


### Contribution

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/contribution` | Obtener todas las contribuciones | GET | `/api/v1/contribution` | No requiere parámetros | Retorna la lista de contribuciones registradas. |
| `/api/v1/contribution` | Crear contribución | POST | `/api/v1/contribution` | Body JSON: `billId`, `householdId`, `description`, `deadlineForMembers`, `strategy` | Registra una nueva contribución asociada a un household y recibo. |
| `/api/v1/contribution/{id}` | Obtener contribución por ID | GET | `/api/v1/contribution/{id}` | Path Parameter: `id` | Retorna la contribución asociada al identificador especificado. |
| `/api/v1/contribution/{id}` | Eliminar contribución | DELETE | `/api/v1/contribution/{id}` | Path Parameter: `id` | Elimina la contribución asociada al identificador especificado. |
| `/api/v1/contribution/bybillid/{billId}` | Obtener contribución por billId | GET | `/api/v1/contribution/bybillid/{billId}` | Path Parameter: `billId` | Retorna las contribuciones asociadas al bill indicado. |
| `/api/v1/contribution/byhouseholdid/{householdId}` | Obtener contribuciones por household | GET | `/api/v1/contribution/byhouseholdid/{householdId}` | Path Parameter: `householdId` | Retorna las contribuciones asociadas al household indicado. |
| `/api/v1/contribution/byid/{id}` | Actualizar contribución | PUT | `/api/v1/contribution/byid/{id}` | Path Parameter: `id`, Body JSON: `description`, `deadlineForMembers`, `strategy` | Actualiza la información de la contribución especificada. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/contribution` | Ninguno | ```json { "id":"C001","billId":"B001","householdId":"HH001","description":"Electricity contribution","deadlineForMembers":"2026-05-20","strategy":1 } ``` | `200 OK` |
| POST | `/api/v1/contribution` | Body: `billId`, `householdId`, `description`, `deadlineForMembers`, `strategy` | ```json { "billId":"B001","householdId":"HH001","description":"Electricity contribution","deadlineForMembers":"2026-05-20","strategy":1 } ``` | `201 Created`, `400 Bad Request` |
| GET | `/api/v1/contribution/{id}` | Path: `id` | ```json { "id":"C001","billId":"B001","householdId":"HH001","description":"Electricity contribution","deadlineForMembers":"2026-05-20","strategy":1 } ``` | `200 OK` |
| DELETE | `/api/v1/contribution/{id}` | Path: `id` | ```json { "id":"C001","billId":"B001","householdId":"HH001","description":"Electricity contribution","deadlineForMembers":"2026-05-20","strategy":1 } ``` | `200 OK`, `404 Not Found` |
| GET | `/api/v1/contribution/bybillid/{billId}` | Path: `billId` | ```json { "id":"C001","billId":"B001","householdId":"HH001","description":"Electricity contribution","deadlineForMembers":"2026-05-20","strategy":1 } ``` | `200 OK` |
| GET | `/api/v1/contribution/byhouseholdid/{householdId}` | Path: `householdId` | ```json { "id":"C001","billId":"B001","householdId":"HH001","description":"Electricity contribution","deadlineForMembers":"2026-05-20","strategy":1 } ``` | `200 OK` |
| PUT | `/api/v1/contribution/byid/{id}` | Path: `id`, Body: `description`, `deadlineForMembers`, `strategy` | ```json { "description":"Updated contribution","deadlineForMembers":"2026-05-25","strategy":2 } ``` | `200 OK`, `400 Bad Request`, `404 Not Found` |

### Bills

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/bills` | Obtener todos los bills | GET | `/api/v1/bills` | No requiere parámetros | Retorna la lista de bills registrados en el sistema. |
| `/api/v1/bills` | Crear bill | POST | `/api/v1/bills` | Body JSON: `houseHoldId`, `description`, `amount`, `createdBy`, `paymentDate` | Registra un nuevo bill asociado a un household. |
| `/api/v1/bills/byhousehold/{householdId}` | Obtener bills por household | GET | `/api/v1/bills/byhousehold/{householdId}` | Path Parameter: `householdId` | Retorna los bills asociados al household especificado. |
| `/api/v1/bills/byid/{id}` | Actualizar bill | PUT | `/api/v1/bills/byid/{id}` | Path Parameter: `id`, Body JSON: `description`, `amount`, `paymentDate` | Actualiza la información del bill especificado. |
| `/api/v1/bills/{id}` | Eliminar bill | DELETE | `/api/v1/bills/{id}` | Path Parameter: `id` | Elimina el bill asociado al identificador especificado. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/bills` | Ninguno | ```json { "id":"B001","houseHoldId":"HH001","description":"Electricity bill","amount":120.0,"createdBy":1,"paymentDate":"2026-05-20","createdAt":"2026-05-14","updatedAt":"2026-05-14" } ``` | `200 OK`, `404 Not Found` |
| POST | `/api/v1/bills` | Body: `houseHoldId`, `description`, `amount`, `createdBy`, `paymentDate` | ```json { "houseHoldId":"HH001","description":"Electricity bill","amount":120.0,"createdBy":1,"paymentDate":"2026-05-20" } ``` | `201 Created`, `400 Bad Request` |
| GET | `/api/v1/bills/byhousehold/{householdId}` | Path: `householdId` | ```json [ { "id":"B001","houseHoldId":"HH001","description":"Electricity bill","amount":120.0,"createdBy":1,"paymentDate":"2026-05-20","createdAt":"2026-05-14","updatedAt":"2026-05-14" } ] ``` | `200 OK`, `404 Not Found` |
| PUT | `/api/v1/bills/byid/{id}` | Path: `id`, Body: `description`, `amount`, `paymentDate` | ```json { "description":"Updated bill","amount":150.0,"paymentDate":"2026-05-25" } ``` | `200 OK`, `400 Bad Request`, `404 Not Found` |
| DELETE | `/api/v1/bills/{id}` | Path: `id` | ```json { "id":"B001","houseHoldId":"HH001","description":"Electricity bill","amount":120.0,"createdBy":1,"paymentDate":"2026-05-20","createdAt":"2026-05-14","updatedAt":"2026-05-14" } ``` | `200 OK`, `404 Not Found` |


### HouseHold

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/house_hold/{id}` | Obtener household por ID | GET | `/api/v1/house_hold/{id}` | Path Parameter: `id` | Retorna la información del household asociado al identificador especificado. |
| `/api/v1/house_hold/{id}` | Actualizar household | PUT | `/api/v1/house_hold/{id}` | Path Parameter: `id`, Body JSON: `name`, `description`, `memberCount`, `currency`, `startDate` | Actualiza la información del household especificado. |
| `/api/v1/house_hold` | Crear household | POST | `/api/v1/house_hold` | Body JSON: `id`, `name`, `representativeId`, `currency`, `description`, `memberCount`, `startDate` | Registra un nuevo household en el sistema. |
| `/api/v1/house_hold/representative/{representativeId}` | Obtener households por representante | GET | `/api/v1/house_hold/representative/{representativeId}` | Path Parameter: `representativeId` | Retorna los households asociados al representante especificado. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/house_hold/{id}` | Path: `id` | ```json { "id":"HH001","name":"Family House","description":"Main household","memberCount":4,"representativeId":1,"currency":"USD","startDate":"2026-05-01","createdAt":"2026-05-14","updatedAt":"2026-05-14" } ``` | `200 OK`, `404 Not Found` |
| PUT | `/api/v1/house_hold/{id}` | Path: `id`, Body: `name`, `description`, `memberCount`, `currency`, `startDate` | ```json { "name":"Updated House","description":"Updated description","memberCount":5,"currency":"USD","startDate":"2026-05-01" } ``` | `200 OK`, `404 Not Found` |
| POST | `/api/v1/house_hold` | Body: `id`, `name`, `representativeId`, `currency`, `description`, `memberCount`, `startDate` | ```json { "id":"HH001","name":"Family House","representativeId":1,"currency":"USD","description":"Main household","memberCount":4,"startDate":"2026-05-01" } ``` | `201 Created`, `400 Bad Request` |
| GET | `/api/v1/house_hold/representative/{representativeId}` | Path: `representativeId` | ```json [ { "id":"HH001","name":"Family House","description":"Main household","memberCount":4,"representativeId":1,"currency":"USD","startDate":"2026-05-01","createdAt":"2026-05-14","updatedAt":"2026-05-14" } ] ``` | `200 OK` |


### HouseholdMember

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/household_member` | Crear household member | POST | `/api/v1/household_member` | Body JSON: `householdId`, `userId`, `isRepresentative`, `income` | Registra un nuevo miembro en un household. |
| `/api/v1/household_member` | Obtener todos los household members | GET | `/api/v1/household_member` | No requiere parámetros | Retorna la lista de miembros registrados. |
| `/api/v1/household_member/{id}` | Obtener household member por ID | GET | `/api/v1/household_member/{id}` | Path Parameter: `id` | Retorna la información del miembro especificado. |
| `/api/v1/household_member/{id}` | Actualizar household member | PUT | `/api/v1/household_member/{id}` | Path Parameter: `id`, Body JSON: `householdId`, `userId`, `isRepresentative`, `income`, `allocations` | Actualiza la información del miembro especificado. |
| `/api/v1/household_member/{id}` | Eliminar household member | DELETE | `/api/v1/household_member/{id}` | Path Parameter: `id` | Elimina el miembro especificado. |
| `/api/v1/household_member/household/{householdId}` | Obtener miembros por household | GET | `/api/v1/household_member/household/{householdId}` | Path Parameter: `householdId` | Retorna los miembros asociados al household indicado. |
| `/api/v1/household_member/household/{householdId}/detailed` | Obtener miembros detallados | GET | `/api/v1/household_member/household/{householdId}/detailed` | Path Parameter: `householdId` | Retorna miembros con información detallada de usuario y contribuciones. |
| `/api/v1/household_member/user/{userId}` | Obtener households por usuario | GET | `/api/v1/household_member/user/{userId}` | Path Parameter: `userId` | Retorna los households asociados al usuario indicado. |
| `/api/v1/household_member/{id}/promote-representative` | Promover representante | POST | `/api/v1/household_member/{id}/promote-representative` | Path Parameter: `id` | Promueve un miembro a representante del household. |
| `/api/v1/household_member/{id}/demote-representative` | Degradar representante | POST | `/api/v1/household_member/{id}/demote-representative` | Path Parameter: `id` | Remueve el rol de representante del miembro indicado. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| POST | `/api/v1/household_member` | Body: `householdId`, `userId`, `isRepresentative`, `income` | ```json { "householdId":"HH001","userId":1,"isRepresentative":true,"income":2500.0 } ``` | `201 Created`, `400 Bad Request` |
| GET | `/api/v1/household_member` | Ninguno | ```json [ { "id":"HM001","householdId":"HH001","userId":1 } ] ``` | `200 OK` |
| GET | `/api/v1/household_member/{id}` | Path: `id` | ```json { "id":"HM001","householdId":"HH001","userId":1,"isRepresentative":true,"income":2500.0 } ``` | `200 OK`, `404 Not Found` |
| PUT | `/api/v1/household_member/{id}` | Path: `id`, Body: `householdId`, `userId`, `isRepresentative`, `income`, `allocations` | ```json { "householdId":"HH001","userId":1,"isRepresentative":false,"income":3000.0 } ``` | `200 OK`, `404 Not Found` |
| DELETE | `/api/v1/household_member/{id}` | Path: `id` | ```json { "message":"Household member deleted" } ``` | `200 OK`, `404 Not Found` |
| GET | `/api/v1/household_member/household/{householdId}` | Path: `householdId` | ```json [ { "id":"HM001","householdId":"HH001","userId":1 } ] ``` | `200 OK` |
| GET | `/api/v1/household_member/household/{householdId}/detailed` | Path: `householdId` | ```json [ { "id":"HM001","userId":1,"income":2500.0,"contributions":[] } ] ``` | `200 OK` |
| GET | `/api/v1/household_member/user/{userId}` | Path: `userId` | ```json [ { "householdId":"HH001","userId":1 } ] ``` | `200 OK` |
| POST | `/api/v1/household_member/{id}/promote-representative` | Path: `id` | ```json { "message":"Representative promoted successfully" } ``` | `200 OK`, `404 Not Found` |
| POST | `/api/v1/household_member/{id}/demote-representative` | Path: `id` | ```json { "message":"Representative demoted successfully" } ``` | `200 OK`, `404 Not Found` |

### IncomeAllocation

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/income_allocation/byhousehold/{householdId}` | Obtener allocations por household | GET | `/api/v1/income_allocation/byhousehold/{householdId}` | Path Parameter: `householdId` | Retorna las asignaciones de ingreso asociadas al household indicado. |
| `/api/v1/income_allocation/byuserid/{userId}` | Obtener allocations por usuario | GET | `/api/v1/income_allocation/byuserid/{userId}` | Path Parameter: `userId` | Retorna las asignaciones de ingreso asociadas al usuario indicado. |
| `/api/v1/income_allocation` | Crear income allocation | POST | `/api/v1/income_allocation` | Body JSON: `userId`, `householdId`, `percentage` | Registra una nueva asignación de ingreso. |
| `/api/v1/income_allocation/byid/{id}` | Actualizar income allocation | PUT | `/api/v1/income_allocation/byid/{id}` | Path Parameter: `id`, Body JSON: `id`, `userId`, `householdId`, `percentage` | Actualiza la asignación de ingreso especificada. |
| `/api/v1/income_allocation/{id}` | Eliminar income allocation | DELETE | `/api/v1/income_allocation/{id}` | Path Parameter: `id` | Elimina la asignación de ingreso especificada. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/income_allocation/byhousehold/{householdId}` | Path: `householdId` | ```json { "id":"IA001","userId":1,"householdId":"HH001","percentage":50.0 } ``` | `200 OK`, `404 Not Found` |
| GET | `/api/v1/income_allocation/byuserid/{userId}` | Path: `userId` | ```json { "id":"IA001","userId":1,"householdId":"HH001","percentage":50.0 } ``` | `200 OK`, `404 Not Found` |
| POST | `/api/v1/income_allocation` | Body: `userId`, `householdId`, `percentage` | ```json { "userId":1,"householdId":"HH001","percentage":50.0 } ``` | `201 Created`, `400 Bad Request` |
| PUT | `/api/v1/income_allocation/byid/{id}` | Path: `id`, Body: `id`, `userId`, `householdId`, `percentage` | ```json { "id":"IA001","userId":1,"householdId":"HH001","percentage":60.0 } ``` | `200 OK`, `400 Bad Request` |
| DELETE | `/api/v1/income_allocation/{id}` | Path: `id` | ```json { "id":"IA001","userId":1,"householdId":"HH001","percentage":50.0 } ``` | `200 OK`, `404 Not Found` |

### Settings

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/settings` | Obtener settings por usuario | GET | `/api/v1/settings?userId={userId}` | Query Parameter: `userId` | Retorna la configuración asociada al usuario especificado. |
| `/api/v1/settings` | Crear settings | POST | `/api/v1/settings` | Body JSON: `userId`, `language`, `darkMode`, `notificationEnabled` | Registra la configuración de un usuario o retorna la existente. |
| `/api/v1/settings/{id}` | Actualizar settings | PUT | `/api/v1/settings/{id}` | Path Parameter: `id`, Body JSON: `userId`, `language`, `darkMode`, `notificationEnabled` | Actualiza la configuración asociada al identificador especificado. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/settings?userId={userId}` | Query: `userId` | ```json { "id":1,"userId":1,"language":"EN","darkMode":true,"notificationEnabled":true,"createdAt":"2026-05-15","updatedAt":"2026-05-15" } ``` | `200 OK`, `404 Not Found` |
| POST | `/api/v1/settings` | Body: `userId`, `language`, `darkMode`, `notificationEnabled` | ```json { "userId":1,"language":"EN","darkMode":true,"notificationEnabled":true } ``` | `200 OK`, `201 Created` |
| PUT | `/api/v1/settings/{id}` | Path: `id`, Body: `userId`, `language`, `darkMode`, `notificationEnabled` | ```json { "userId":1,"language":"ES","darkMode":false,"notificationEnabled":true } ``` | `200 OK`, `404 Not Found` |


### Settings

| Endpoint | Acción Implementada | Método HTTP | Sintaxis de Llamada | Parámetros | Descripción del Response |
|---|---|---|---|---|---|
| `/api/v1/settings` | Obtener settings por usuario | GET | `/api/v1/settings?userId={userId}` | Query Parameter: `userId` | Retorna la configuración asociada al usuario especificado. |
| `/api/v1/settings` | Crear settings | POST | `/api/v1/settings` | Body JSON: `userId`, `language`, `darkMode`, `notificationEnabled` | Registra la configuración de un usuario o retorna la existente. |
| `/api/v1/settings/{id}` | Actualizar settings | PUT | `/api/v1/settings/{id}` | Path Parameter: `id`, Body JSON: `userId`, `language`, `darkMode`, `notificationEnabled` | Actualiza la configuración asociada al identificador especificado. |

| Método | Endpoint | Parámetros | Ejemplo Request/Response | Códigos HTTP |
|---|---|---|---|---|
| GET | `/api/v1/settings?userId={userId}` | Query: `userId` | ```json { "id":1,"userId":1,"language":"EN","darkMode":true,"notificationEnabled":true,"createdAt":"2026-05-15","updatedAt":"2026-05-15" } ``` | `200 OK`, `404 Not Found` |
| POST | `/api/v1/settings` | Body: `userId`, `language`, `darkMode`, `notificationEnabled` | ```json { "userId":1,"language":"EN","darkMode":true,"notificationEnabled":true } ``` | `200 OK`, `201 Created` |
| PUT | `/api/v1/settings/{id}` | Path: `id`, Body: `userId`, `language`, `darkMode`, `notificationEnabled` | ```json { "userId":1,"language":"ES","darkMode":false,"notificationEnabled":true } ``` | `200 OK`, `404 Not Found` |

##### 4.2.1.7. Software Deployment Evidence for Sprint Review

**Landing Page - Deploy:**

https://1acc0238-2610-3667.github.io/Landing-Page/

<br>
<img src="assets/landing_deploy1.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_deploy2.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_deploy3.jpg" alt="CandidateContextDiscovery">
<br>

<br>
<img src="assets/landing_deploy4.jpg" alt="CandidateContextDiscovery">
<br>



**Backend - Deploy:**

https://backend-harmonix.onrender.com/swagger

<br>
<img src="assets/backend_deploy.jpg" alt="CandidateContextDiscovery">
<br>


##### 4.2.1.8. Team Collaboration Insights during Sprint

<br>
<img src="assets/insights_backend.jpg" alt="CandidateContextDiscovery">
<br>


#### 4.2.2. Sprint 2

A continuación, se presenta el Sprint Planning 2, donde se incluyen las evidencias de planificación e implementación del Landing Page, Mobile App y Backend. También se registran los avances del proyecto e insights de colaboración del equipo a través de GitHub.

##### 4.2.2.1. Sprint Planning 2

| **Campo**                              | **Descripción**                                                                                                                                                                                                                                                                                                    |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Sprint #**                           | Sprint 1                                                                                                                                                                                                                                                                                                           |
| **Sprint Planning Background**         |                                                                                                                                                                                                                                                                                                                    |
| **Date**                               | 2026-06-11                                                                                                                                                                                                                                                                                                         |
| **Time**                               | 03:00 PM (GMT -5)                                                                                                                                                                                                                                                                                                  |
| **Location**                           | Modalidad remota por Google Meet                                                                                                                                                                                                                                                                                   |
| **Prepared By**                        | Testigos de Splitly                                                                                                                                                                                                                                                                                              |
| **Attendees (to planning meeting)**    | Equipo Splitly                                                                                                                                                                                                                                                            |
| **Sprint 0 Review Summary**        | Este es el segundo sprint. Del Sprint anterior concluimos que nos falta pulir un pequeño porcentaje del backend y estamos listos para implementar la aplicación.                                                                                                                                                                                                                                   |
| **Sprint 0 Retrospective Summary** | Al estar en una face intermedia del proyecto, se identificaron aspectos técnicos por aprender, como el uso kotlin y Flutter para el desarrollo movil de nuestras pantallas previamente diseñadas en figma. Se discutió el contenido a incluir y se definió el objetivo principal: Implementar una primera versión de la aplicación Splitly al final del sprint. |
| **Sprint Goal & User Stories**         |                                                                                                                                                                                                                                                                                                                    |
| **Sprint 1 Goal**                      | Completar el Backend de la aplicación al 100% e implementar una primera versión de la aplición móvil Splitly.                                                                                                                                                                                        |
| **Sprint 1 Velocity**                  | 20                                                                                                                                                                                                                                                                                                                  |
| **Sum of Story Points**                | 10                                                                                                                                                                                                                                                                                                                  |


##### 4.2.2.2. Sprint Backlog 2

El Sprint Backlog 2 corresponde al desarrollo de la primera versión de la aplicación Splitly. En este sprint nos enfocaremos en conectar el frontend con el backend, asegurar la aplicación mediante autenticación y roles, y cerrar los flujos centrales de gastos y pagos.

Adicionalmente, se incluyeron tareas técnicas relacionadas con la documentación del despliegue y la configuración de monitoreo básico, asegurando que el proyecto cuente con una base sólida para futuras iteraciones.

El trabajo colaborativo del equipo se gestionó en la herramienta Trello, lo que permitió organizar, priorizar y dar seguimiento a cada tarea de manera eficiente.
Link al tablero de Trello: https://trello.com/invite/b/6a04a4676f2c78852edaeb1a/ATTI85b6ff75c99bfbde325e6f171ad6e8b4E226ADCE/splitly-sprint-backlog


| User Story Id | Title | Task Id | Task Title | Description | Estimation (Hours) | Assigned To | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **TS01** | Implementar autenticación JWT | T1 | Configuración JWT | Generación y validación de tokens en el backend | 4 | Héctor Ríos | To-do |
| **TS02** | Cifrar contraseñas | T1 | Hashing de passwords | Integración de Bcrypt antes de guardar en BD | 3 | Walter Ramirez | To-do |
| **TS03** | Validar roles backend | T1 | Middleware roles | Proteger rutas según rol (administrador/miembro) | 4 | Joaquin Cuentas | To-do |
| **TS05** | Conectar formularios con endpoints | T1 | Integración Auth | Conectar UI de login y registro con API | 4 | Jose Luis Martinez Validivia | To-do |
| **TS05** | Conectar formularios con endpoints | T2 | Integración Gastos | Conectar UI de creación de gastos y pagos con API | 5 | Rodrigo Miraval | To-do |
| **TS06** | Validar respuestas del backend | T1 | Interceptores HTTP | Manejo centralizado de respuestas y códigos de estado | 3 | Walter Ramirez | To-do |
| **US37** | Manejo de estados de carga | T1 | UI Loaders | Implementar spinners y mensajes de éxito en la app | 4 | Héctor Ríos | To-do |
| **TS04** | Actualización de perfil API | T1 | UI Update Perfil | Conectar pantalla de edición con el endpoint de perfil | 3 | Jose Luis Martinez Validivia | To-do |
| **US09** | Visualizar reportes mensuales | T1 | Reporte básico | Consolidar ingresos y gastos del mes en una vista | 5 | Rodrigo Miraval | To-do |
| **TS09** | Update/Delete gastos | T1 | Endpoints mutación | Lógica para editar o eliminar un gasto ya registrado | 4 | Joaquin Cuentas | To-do |
| **TS10** | Integración de gastos | T1 | Testing flujo gastos | Pruebas end-to-end de registro, vista y cálculo de gastos | 3 | Walter Ramirez | To-do |


##### 4.2.2.3. Development Evidence for Sprint Review

| Repository Branch | Commit Id     | Commit Message                               | Commit Message Body | Commited on (Date) |
|------------------|--------------|-----------------------------------------------|---------------------|-------------------|
| Mobile App - develop | 3861935 | chore(): add sharedPreferences                 |                     | 11/05/2026 |
| Mobile App - develop | b151bf1 | chore(): add drawer and navigation bar        |                     | 11/05/2026 |
| Mobile App - develop | fc52f52 | chore(): add working login flow               |                     | 11/05/2026 |
| Mobile App - develop | bdb50ad | chore(): add entities models                  |                     | 10/05/2026 |
| Mobile App - develop | 023ad09 | chore(): add initial signup screen            |                     | 10/05/2026 |
| Mobile App - develop | fe8c024 | chore(): add new login screen styles          |                     | 10/05/2026 |
| Mobile App - develop | 3312219 | initial commit                                |                     | 10/05/2026 |

##### 4.2.2.4. Testing Suite Evidence for Sprint Review

Tal como se estableció en la planificación y retrospectiva del Sprint 1, durante este segundo sprint se procedió con la implementación de la suite de pruebas automatizadas, aprovechando que el backend alcanzó su etapa de completitud y la estructura de la aplicación móvil en Flutter se encontraba consolidada.

El objetivo principal en esta fase fue garantizar la estabilidad de los flujos críticos del sistema (autenticación y gestión de gastos) mediante herramientas nativas del ecosistema de Flutter (`flutter_test` e `integration_test`).

**1. Tipos de Pruebas Implementadas**

Para asegurar la calidad del producto, la estrategia de pruebas abarcó los siguientes niveles:

* **Unit Tests (Pruebas Unitarias):** Se evaluó la lógica de negocio aislada de la interfaz gráfica. Esto incluyó la validación de los modelos de datos, la correcta serialización/deserialización de las respuestas JSON provenientes del backend, y las utilidades matemáticas encargadas del cálculo proporcional de las cuotas.
* **Widget Tests (Pruebas de Componentes):** Se verificó el correcto renderizado y comportamiento de los componentes individuales de la UI en Flutter. Se comprobó que los formularios de registro e inicio de sesión muestren las validaciones de estado correctas (ej. campos obligatorios vacíos o formatos de correo inválidos) sin necesidad de levantar un emulador completo.
* **Integration Tests (Pruebas de Integración y Aceptación):** Cumpliendo con lo reprogramado en el Sprint 1, se implementaron pruebas End-to-End (E2E) corriendo en dispositivos simulados. Estas pruebas validaron la comunicación real entre la aplicación móvil y los endpoints del backend desplegados, confirmando flujos completos como el inicio de sesión seguro (JWT) y el registro de un nuevo gasto.

**2. Resumen de Ejecución de Pruebas**

La siguiente tabla detalla un subconjunto representativo de los casos de prueba ejecutados exitosamente durante el cierre del Sprint 2:

| ID Prueba | Tipo de Prueba | Módulo / Historia de Usuario | Descripción de la Validación | Resultado |
| :--- | :--- | :--- | :--- | :---: |
| TS-01 | Unit Test | Identity and Access Management | Serialización correcta del modelo `User` y extracción del JWT. | Exitoso |
| TS-02 | Unit Test | Contributions Distribution | Validación del algoritmo de cálculo proporcional de un gasto entre `n` miembros. | Exitoso |
| TS-03 | Widget Test | Interfaz de Usuario (UI) | Renderizado del formulario de Login y validación visual de campos vacíos. | Exitoso |
| TS-04 | Widget Test | Interfaz de Usuario (UI) | Visualización correcta de estados de carga (Spinners) al procesar peticiones. | Exitoso |
| TS-05 | Integration Test | Flujo End-to-End | Inicio de sesión exitoso con credenciales reales y redirección al Dashboard. | Exitoso |

**3. Evidencias de Ejecución**

La ejecución de la suite automatizada se realizó directamente desde el entorno de desarrollo mediante los comandos de testing de Flutter. Todas las aserciones (*expects*) diseñadas para los módulos de IAM y Contributions Distribution pasaron satisfactoriamente.

<p align="center">
  <img src="./assets/testeo prueba.jpg" alt="Ejecución de pruebas en Flutter" width="100%">
  <br>
  <em>Figura 1. Consola de comandos mostrando la ejecución exitosa de la suite de pruebas unitarias y de widgets en Flutter.</em>
</p>

**Conclusión del Sprint en Testing:**
Con la integración de esta suite, se mitiga la deuda técnica del sprint anterior y se establece una base sólida de integración continua, asegurando que las futuras actualizaciones de los flujos de Splitly no rompan las funcionalidades ya validadas.

##### 4.2.2.5. Execution Evidence for Sprint Review

Durante la realización de este segundo sprint se implementó con éxito la primera versión funcional de la aplicación móvil (Mobile App) en Flutter, logrando la integración completa con los servicios web para los flujos críticos como autenticación, gestión de hogares y control de gastos.



**Mobile App:**

<br>
<img src="assets/app1.jpg" alt="Pantalla de Login / Registro">
<br>

<br>
<img src="assets/app2.jpg" alt="Pantalla de Login / Registro">
<br>

<br>
<img src="assets/app3.jpg" alt="Pantalla de Login / Registro">
<br>

<br>
<img src="assets/app4.jpg" alt="Pantalla de Login / Registro">
<br>

<br>
<img src="assets/app5.jpg" alt="Pantalla de Login / Registro">
<br>

<br>
<img src="assets/app6.jpg" alt="Pantalla de Login / Registro">
<br>

<br>
<img src="assets/app7.jpg" alt="Pantalla de Login / Registro">
<br>

##### 4.2.2.6. Services Documentation Evidence for Sprint Review

Durante el Sprint 1 se estableció la estructura base de la documentación de la API. Para este segundo sprint, la documentación en OpenAPI/Swagger fue actualizada en su totalidad para reflejar la culminación del 100% de los endpoints del backend.

El avance más significativo en esta iteración documentada fue la integración del esquema de seguridad **JWT (JSON Web Token)** en los contratos de la API. A continuación, se presentan las tablas de los endpoints finales actualizados, donde se especifica claramente la restricción de autorización. Se documentó que todos los módulos críticos exigen un token Bearer válido, a excepción de las rutas de autenticación inicial.

### 1. Identity and Access Management (Autenticación y Usuarios)

Este módulo fue documentado para diferenciar claramente las rutas públicas de las operaciones privadas que requieren validación del usuario en sesión.

| Endpoint | Acción Implementada | Método | Parámetros Principales | Seguridad (JWT) | Códigos HTTP |
| :--- | :--- | :---: | :--- | :---: | :--- |
| `/api/v1/authentication/sign-up` | Registrar nuevo usuario | POST | Body: `email`, `password`, `name`, `role`, `householdId` | Acceso Público | `200 OK`, `400 Bad Request` |
| `/api/v1/authentication/sign-in` | Iniciar sesión y obtener token | POST | Body: `email`, `password` | Acceso Público | `200 OK`, `401 Unauthorized` |
| `/api/v1/user/user/{id}` | Consultar perfil por ID | GET | Path: `id` | Requiere Token | `200 OK`, `401 Unauthorized` |
| `/api/v1/user/byemail/{emailAddress}`| Actualizar perfil de usuario | PUT | Path: `emailAddress`, Body: `personName`, `password`| Requiere Token | `200 OK`, `403 Forbidden` |
| `/api/v1/user-income` | Registrar ingresos del usuario | POST | Body: `userId`, `income` | Requiere Token | `201 Created`, `400 Bad Request` |

### 2. Contributions Distribution (Gastos y Cuotas)

La documentación de este módulo fue actualizada para incluir los flujos de creación de facturas (Bills) y el cálculo de la distribución (Contributions), asegurando que solo usuarios autenticados del hogar puedan modificarlos.

| Endpoint | Acción Implementada | Método | Parámetros Principales | Seguridad (JWT) | Códigos HTTP |
| :--- | :--- | :---: | :--- | :---: | :--- |
| `/api/v1/bills` | Registrar nuevo gasto central | POST | Body: `houseHoldId`, `amount`, `description`, `paymentDate`| Requiere Token | `201 Created`, `401 Unauthorized` |
| `/api/v1/bills/byhousehold/{id}` | Listar gastos del hogar | GET | Path: `id` (Household ID) | Requiere Token | `200 OK`, `404 Not Found` |
| `/api/v1/contribution` | Generar distribución de pago | POST | Body: `billId`, `strategy`, `deadlineForMembers` | Requiere Token | `201 Created`, `400 Bad Request` |
| `/api/v1/member_contribution` | Registrar pago de cuota individual| POST | Body: `contributionId`, `memberId`, `amount` | Requiere Token | `201 Created`, `403 Forbidden` |
| `/api/v1/member_contribution/{id}` | Eliminar registro de pago | DELETE | Path: `id` (Member Contribution ID) | Requiere Token | `200 OK`, `401 Unauthorized` |

### 3. Household Management (Gestión de Hogares e Invitaciones)

Documentación finalizada para el ciclo de vida de los grupos. Se detallaron las respuestas esperadas al interactuar con las invitaciones y los roles internos.

| Endpoint | Acción Implementada | Método | Parámetros Principales | Seguridad (JWT) | Códigos HTTP |
| :--- | :--- | :---: | :--- | :---: | :--- |
| `/api/v1/house_hold` | Crear un nuevo hogar | POST | Body: `name`, `representativeId`, `currency`, `startDate`| Requiere Token | `201 Created`, `401 Unauthorized` |
| `/api/v1/house_hold/{id}` | Actualizar datos del hogar | PUT | Path: `id`, Body: `name`, `currency`, `memberCount` | Requiere Token | `200 OK`, `404 Not Found` |
| `/api/v1/household_member` | Añadir miembro al hogar | POST | Body: `householdId`, `userId`, `income` | Requiere Token | `201 Created`, `400 Bad Request` |
| `/api/v1/invitations` | Generar invitación por correo | POST | Body: `email`, `householdId`, `description` | Requiere Token | `200 OK`, `401 Unauthorized` |
| `/api/v1/invitations/pending` | Validar invitación pendiente | GET | Query: `email`, `householdId` | Requiere Token | `200 OK`, `404 Not Found` |

### 4. App Management (Configuraciones)

Se agregaron a Swagger los endpoints transversales para manejar las preferencias de la aplicación, garantizando que un usuario solo pueda alterar sus propios ajustes mediante el token.

| Endpoint | Acción Implementada | Método | Parámetros Principales | Seguridad (JWT) | Códigos HTTP |
| :--- | :--- | :---: | :--- | :---: | :--- |
| `/api/v1/settings` | Crear preferencias de usuario | POST | Body: `userId`, `language`, `darkMode`, `notificationEnabled` | Requiere Token | `201 Created`, `400 Bad Request` |
| `/api/v1/settings?userId={id}` | Consultar preferencias | GET | Query: `userId` | Requiere Token | `200 OK`, `404 Not Found` |
| `/api/v1/settings/{id}` | Actualizar preferencias | PUT | Path: `id`, Body: `language`, `darkMode`, `notification` | Requiere Token | `200 OK`, `403 Forbidden` |


##### 4.2.2.7. Software Deployment Evidence for Sprint Review

Durante el Sprint 2, se desplegó el backend al 100% de Splitly en el servicio RENDER, asegurando su disponibilidad y persistencia de datos. Se validó el funcionamiento de los endpoints por medio de Swagger y pruebas de integración, y se dejó preparada la arquitectura para futuros desarrollos. Aquí las evidencias principales:

**Backend:**

<br>
<img src="assets/render1.png" alt="Swagger Backend Sprint 2">
<br>

<br>
<img src="assets/render2.png" alt="Swagger Backend Sprint 2">
<br>

<br>
<img src="assets/render3.png" alt="Swagger Backend Sprint 2">
<br>

<br>
<img src="assets/render4.png" alt="Swagger Backend Sprint 2">
<br>

<br>
<img src="assets/render5.png" alt="Swagger Backend Sprint 2">
<br>

<br>
<img src="assets/render6.png" alt="Swagger Backend Sprint 2">
<br>


##### 4.2.2.8. Team Collaboration Insights during Sprint

Evidencias de los insighs del sprint 2:

<br>
<img src="assets/insights2.1" alt="Swagger Backend Sprint 2">
<br>

<br>
<img src="assets/insights2.2" alt="Swagger Backend Sprint 2">
<br>

<br>
<img src="assets/insights2.3" alt="Swagger Backend Sprint 2">
<br>


### 4.3. Validation Interviews
#### 4.3.1. Diseño de Entrevistas

Durante el proceso de entrevistas con los usuarios finales, se identificaron diversos requerimientos relevantes para la experiencia en base a las siguientes preguntas:

**Para el Segmento 1: Miembros del hogar**

1. Primera impresión sobre la interfaz:

- ¿Qué opinas del diseño de la landing page? ¿Te resulta fácil de entender?

- ¿Hay algún elemento visual que te llame la atención o que encuentres confuso?

2. Facilidad de uso:

- ¿Fue fácil encontrar dónde se registran los gastos o contribuciones?

- ¿Hubo algún momento en el que te sentiste perdido o no supieras qué hacer en la página?

3. Navegación y funcionalidades:

- ¿La navegación entre secciones (como ver tus aportes, revisar los gastos) fue clara?

- ¿Te resultó sencillo agregar un gasto o una contribución? ¿Qué mejoras sugerirías?

4. Transparencia y confianza:

- ¿Qué piensas sobre la transparencia de la herramienta? ¿Te resultó útil ver las contribuciones de los demás miembros del hogar?

- ¿Sientes que la aplicación te ayuda a comprender mejor la distribución de los gastos en el hogar?

5. Gráficos y reportes:

- ¿Qué opinas de los gráficos o reportes que muestra la página? ¿Son claros y fáciles de entender?

- ¿Te gustaría tener más detalles en los reportes, o consideras que la información mostrada es suficiente?

6. Experiencia general:

- ¿Te parece que esta herramienta puede ayudarte a gestionar los gastos del hogar de manera más equitativa?

- ¿Usarías esta aplicación de manera regular? ¿Qué haría que la usaras más seguido?


**Para el Segmento 2: Representantes del hogar**

1. Gestión de finanzas en el panel:

- ¿Qué opinas del panel de control donde puedes gestionar los gastos y contribuciones? ¿Lo encuentras útil?

- ¿Fue fácil aprobar o modificar los gastos? ¿Hubo algo que te resultó confuso en el proceso?

2. Visibilidad y control:

- ¿Te pareció que tienes suficiente visibilidad sobre las contribuciones de los miembros del hogar?

- ¿Qué tan útil encuentras la capacidad de ver los reportes mensuales y las contribuciones de todos los miembros del hogar?

3. Personalización y ajustes:

- ¿Te gustaría poder personalizar más aspectos de la herramienta, como las categorías de gastos o las reglas de división?

- ¿Fue fácil ajustar los porcentajes de contribución o cambiar cualquier configuración?

4. Usabilidad y eficiencia:

- ¿Te resultó fácil realizar tareas como agregar miembros al hogar o asignar contribuciones?

- ¿Hubo algún momento en que pensaste que la aplicación podía hacer algo más para facilitar la gestión de los gastos?

5. Confianza en el sistema:

- ¿Confías en que la aplicación divide los gastos de manera justa? ¿Te gustaría que el sistema explique de manera más clara cómo se calculan los porcentajes?

- ¿Hay alguna parte del proceso donde te gustaría tener más detalles o explicaciones sobre cómo funcionan los cálculos?

6. Satisfacción general y recomendaciones:

- ¿Crees que esta app facilitaría la convivencia en términos de finanzas? ¿Por qué?

- ¿Qué cambios harías para mejorar la experiencia como representante del hogar?


#### 4.3.2. Registro de Entrevistas

En esta sección se presentan los registros de las entrevistas realizadas para validar los productos de software enfocados a los representantes y miembros del hogar. Cada entrevista incluye información sobre el entrevistado, el entrevistador, el tiempo de la entrevista, un resumen de la misma

**Entrevista 1**

| Entrevista                                                         | Registro                                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <p align="center"><img src="./assets/melisa-vi.jpeg"/></p> | **Distrito:** Magdalena <br>**Entrevistado:** Melisa Sulca                                                                                                                                                                                                                                                                       |
| [Enlace al video de validación](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20201f788_upc_edu_pe/IQAWtLL35_1RTJ8ARHXxQwr7ASAayhCOSOgCbG8H7l69KWw?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=rqnxCq)                                | **Entrevistador:** Joaquin Cuentas                                                                                                                                                                                                                                                                                               |
|                                         | **Resumen:** La entrevistada comentó que al inicio se confundió un poco, pero tras explorar la interfaz entendió rápido cómo usar la aplicación web. Consideró que la navegación es clara una vez familiarizado, los gráficos son suficientes y que la herramienta sí ayuda a comprender y gestionar mejor los gastos del hogar. |


**Entrevista 2**

| Entrevista                                                         | Registro                                                                                                                                                                                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <p align="center"><img src="./assets/walter-vi.jpeg"/></p> | **Distrito:** San Miguel <br>**Entrevistado:**  Walter Fajardo                                                                                                                                                                                                                                                                                                                                                                       |
| [Enlace al video de validación](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20201f788_upc_edu_pe/IQD0Lb8dbu__S4Cj2bW3_BiEActS_rI2Ffp4gPIkN_bvnb4?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=MYv6Z2)                                | **Entrevistador:**    Joaquin Cuentas                                                                                                                                                                                                                                                                                                                                                                                                |
|                                        | **Resumen:** El entrevistado indicó que no tuvo ningún problema al usar el panel de control y que todas las funciones —gestión de gastos, visibilidad de contribuciones, reportes y ajustes— le parecieron claras y suficientes. Señaló que todo estuvo en orden, que la herramienta funciona como espera un representante del hogar y que considera que puede facilitar la gestión financiera sin necesidad de cambios adicionales. |


**Entrevista 3**

| Entrevista                                                         | Registro                                                                                                                                                                                                                                                                                                                                                                                                                             |
|--------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <p align="center"><img src="./assets/diego-vi.jpeg"/></p> | **Distrito:** San Miguel <br>**Entrevistado:**  Diego Ávalos                                                                                                                                                                                                                                                                                                                                                                         |
| [Enlace al video de validación](https://upcedupe-my.sharepoint.com/:v:/g/personal/u20201f788_upc_edu_pe/IQCnL77pZNIxQ7IfQ5ZGXYnYAaCW8LKC-rpNBGOayP7NYXU?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=eWygIB)                                | **Entrevistador:**    Joaquin Cuentas                                                                                                                                                                                                                                                                                                                                                                                                |
|                                     | **Resumen:** El entrevistado indicó que no tuvo ningún problema de usabilidad ni de navegación de la aplicación. Todas las secciones estuvieron claras.

**Entrevista 4**

| Entrevista                                                         | Registro                                                                                                                                                                                             |
|--------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <p align="center"><img src="./assets/andrea-vi.jpeg"/></p> | **Distrito:** Los Olivos <br>**Entrevistado:** Andrea Santur                                                                                                                                         |
| [Entrevista de Validación - Andrea](https://upcedupe-my.sharepoint.com/personal/u20201f788_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu20201f788%5Fupc%5Fedu%5Fpe%2FDocuments%2FAndrea%2Dvalidation%20interviews%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E8c76d770%2Dc34a%2D48fb%2Db1db%2Dc0359abb5c42)                                | **Entrevistador:** Joaquin Cuentas                                                                                                                                                                   |
|                               | **Resumen:**  Andrea, menciono que tuvo facilidad para entender la plataforma, funcionalidades y como usrala en el dia dia. Destaca que esto le ayudara mucho en su dia a dia, en los gastos hormiga |


**Entrevista 5**

| Entrevista                                                         | Registro                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|--------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <p align="center"><img src="../images/Entrevista 4.png"/></p> | **Distrito:** Chorrillos <br>**Entrevistado:** Eduardo Chareo                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| [Link](bit.ly/444Hopn)                                | **Entrevistador:** Jose Martinez                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
|                            | **Resumen:**  Eduardo, representante del hogar de 23 años, consideró la plataforma clara, intuitiva y útil para organizar gastos y aportes entre los miembros. Destacó que el dashboard es fácil de entender, la gestión de gastos es sencilla y los reportes mensuales serían muy valiosos. Sugirió únicamente añadir un calendario y una explicación más transparente de cómo se calculan los porcentajes de contribución. En general, afirmó que la herramienta facilitaría la convivencia financiera y no hizo más cambios adicionales. |


**Entrevista 6**

| Entrevista                                                         | Registro                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|--------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <p align="center"><img src="https://imgur.com/hwh99wf.png"/></p> | **Distrito:** Chorrillos<br>**Entrevistada:** Jessica Castillo                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| [Link](bit.ly/4hYUwlD)                                | **Entrevistador:** Joaquin Cuentas                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | 
|                                       | **Resumen:**  Jessica Castillo, de 47 años, consideró que la herramienta es interesante y útil porque le permitiría medir y organizar sus gastos mensuales, mantener sus pagos al día y controlar mejor el dinero disponible en su hogar, especialmente porque a veces se desfasa en sus compras y termina quedándose ajustada. Durante la demostración, comprendió y validó las funciones principales como la creación y edición del hogar, el registro de miembros, la carga de facturas, la visualización de contribuciones y el uso de ajustes, confirmando que estas características responden a sus necesidades de orden y seguimiento. Además, resaltó que la aplicación la ayudaría a ahorrar un poco al tener claro qué debe pagar y cuándo, y como única mejora sugirió incorporar la opción de realizar pagos directamente desde la plataforma, lo cual reforzaría aún más su utilidad como herramienta de gestión financiera.|




#### 4.3.3. Evaluaciones según heurísticas

# Evaluación según Heurísticas (Evaluación propia)

- **CARRERA:** Ingeniería de Software
- **CURSO:** 1acc0238 Aplicaciones para dispositivos móviles
- **SECCIÓN:** Todos
- **AUDITOR:** Grupo 2
- **CLIENTE(S):** Grupo 3
---
## SITE o APP A EVALUAR:

Spitly

## 1. Tareas a Evaluar
El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas tanto en la Landing Page como en la aplicación móvil:

1. Identificación de la propuesta de valor y misión.
2. Navegación por el catálogo de servicios y funcionamiento por roles.
3. Comparación y selección de planes de pago.
4. Registro de un usuario nuevo e inicio de sesión.
5. Creación de un "Hogar" (Household) y unión mediante ID.
6. Gestión de miembros de la comunidad.
7. Registro de contribuciones económicas y visualización de gastos.
8. Seguimiento del cumplimiento de metas grupales.

---

2. Escala de Severidad
   Los problemas detectados se puntúan bajo la siguiente métrica:

* **1. Problema superficial:** Ocurre con muy poca frecuencia; no necesita ser arreglado a menos que exista disponibilidad de tiempo.
* **2. Problema menor:** Se le debería asignar una prioridad baja de cara al siguiente release.
* **3. Problema mayor:** Ocurre frecuentemente; es importante que sean corregidos con prioridad alta.
* **4. Problema muy grave:** Impide al usuario continuar con el uso de la herramienta; imperativo corregir antes del lanzamiento.

---

## 3. Tabla Resumen

| #   | Problema                                                  | Severidad | Heurística/Principio Violada(o)                        |
| :-- | :-------------------------------------------------------- | :-------: | :----------------------------------------------------- |
| 1   | Sección de testimonios sin contenido visible              |   **4**   | Information Architecture: Is it usable?                |
| 2   | Inconsistencia de idioma (Inglés/Español)                 |   **1**   | Usability: Consistencia y estándares                   |
| 3   | Duplicidad de encabezados de sección                      |   **2**   | Usability: Consistencia y estándares                   |
| 4   | Superposición de texto sobre mapa interactivo             |   **2**   | Inclusive Design: Proporciona experiencias comparables |
| 5   | Falta de indicadores de campos obligatorios               |   **2**   | Usability: Prevención de errores                       |
| 6   | Iconos de redes sociales sin etiquetas descriptivas       |   **3**   | Inclusive Design: Diseño accesible                     |
| 7   | Ambigüedad visual en el toggle de ahorro anual            |   **2**   | Information Architecture: Is it findable?              |
| 8   | Contraste insuficiente en selector de rol inactivo        |   **2**   | Usability: Visibilidad del estado del sistema          |
| 9   | Inconsistencia monetaria (S/ frente a $)                  |   **3**   | Usability: Consistencia y estándares                   |
| 10  | Menú de navegación inferior (Tab Bar) volátil             |   **4**   | Usability: Consistencia y estándares                   |
| 11  | Componente de fecha con lógica de botones inusual         |   **3**   | Usability: Libertad y control del usuario              |
| 12  | Variación de etiquetas de retroceso ("Back" vs "Go back") |   **1**   | Usability: Consistencia y estándares                   |
| 13  | Botones de sistema incrustados dentro de inputs de texto  |   **2**   | Usability: Estética y diseño minimalista               |
| 14  | Contraste crítico de accesibilidad en el Login            |   **3**   | Inclusive Design: Proporciona experiencias comparables |

---

## 4. Descripción de Problemas

### **PROBLEMA #1: Sección de testimonios sin contenido visible**
* **Severidad:** 4
* **Heurística violada:** Arquitectura de Información - ¿Es usable?
* **Problema:** En la landing page, el menú de navegación incluye el enlace "Opiniones", pero al dirigirse a dicha sección, solo se muestra el título sin ningún testimonio o reseña de usuario. Esto genera una percepción de producto incompleto y resta credibilidad a la marca.
* **Recomendación:** Integrar al menos tres testimonios reales con fotografía y nombre, o en su defecto, ocultar la sección y el acceso desde el menú hasta que se cuente con contenido validado.
### **PROBLEMA #2: Inconsistencia de idioma (Inglés/Español)**
* **Severidad:** 1
* **Heurística violada:** Usabilidad - Consistencia y estándares
* **Problema:** Se detectan elementos en inglés dentro de una interfaz configurada en español. Específicamente, los placeholders de los videos ("VIDEO ABOUT THE PRODUCT") y etiquetas de navegación móvil ("Back") rompen la armonía idiomática del sitio.
* **Recomendación:** Traducir todos los recursos gráficos y etiquetas de navegación al español para mantener la consistencia en la experiencia del usuario local.

### **PROBLEMA #3: Duplicidad de encabezados de sección**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Consistencia y estándares
* **Problema:** El título "Nuestros Servicios" aparece repetido en dos secciones consecutivas de la landing page. Esto puede confundir al usuario sobre la jerarquía de la información y hace que la navegación se sienta redundante.
* **Recomendación:** Unificar ambas secciones bajo un solo encabezado o renombrar la primera como "Introducción a Splitly" y la segunda como "Características principales".

### **PROBLEMA #4: Superposición de texto sobre mapa interactivo**
* **Severidad:** 2
* **Heurística violada:** Diseño Inclusivo - Proporciona experiencias comparables
* **Problema:** En la sección de contacto, las instrucciones de uso del mapa ("Utiliza la tecla Ctrl...") aparecen superpuestas directamente sobre la cartografía. Dependiendo del color del mapa en esa zona, el texto puede volverse ilegible.
* **Recomendación:** Colocar las instrucciones de interacción en un cintillo informativo debajo del mapa o dentro de un contenedor con fondo sólido para garantizar el contraste.

### **PROBLEMA #5: Falta de indicadores de campos obligatorios**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Prevención de errores
* **Problema:** Los formularios de la landing page y de la aplicación móvil (como el de registro) no especifican qué campos son obligatorios. Esto obliga al usuario a adivinar y puede generar frustración tras intentos fallidos de envío.
* **Recomendación:** Añadir el asterisco estándar (*) en los campos obligatorios y un mensaje aclaratorio al inicio del formulario.

### **PROBLEMA #6: Iconos de redes sociales sin etiquetas descriptivas**
* **Severidad:** 3
* **Heurística violada:** Diseño Inclusivo - Diseño accesible
* **Problema:** Los iconos de redes sociales en el footer carecen de etiquetas de texto o atributos "aria-label". Esto hace que la sección sea inaccesible para usuarios que dependen de lectores de pantalla.
* **Recomendación:** Implementar etiquetas descriptivas invisibles (como aria-label="Síguenos en Instagram") para cada enlace social.

### **PROBLEMA #7: Ambigüedad visual en el toggle de ahorro anual**
* **Severidad:** 2
* **Heurística violada:** Arquitectura de Información - ¿Es fácil de encontrar?
* **Problema:** En la sección de precios, el beneficio "Ahorra 2 meses" es visualmente pequeño. Al activar el modo anual, el sistema no resalta con suficiente fuerza el cambio en el costo total, diluyendo la percepción de valor de la oferta.
* **Recomendación:** Utilizar un color de contraste más llamativo para el distintivo de ahorro y mostrar el cálculo del precio mensual anterior tachado.

### **PROBLEMA #8: Contraste insuficiente en selector de rol inactivo**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Visibilidad del estado del sistema
* **Problema:** En el flujo de "¿Cómo funciona?", el botón del rol no seleccionado tiene un color tan claro que parece estar deshabilitado en lugar de simplemente "no activo". El usuario podría pensar que la opción no está disponible.
* **Recomendación:** Aplicar un borde definido o un tono gris más oscuro al estado inactivo para comunicar que el elemento es interactivo pero no está seleccionado.

### **PROBLEMA #9: Inconsistencia monetaria (S/ frente a $)**
* **Severidad:** 3
* **Heurística violada:** Usabilidad - Consistencia y estándares
* **Problema:** Existe una contradicción en el uso de divisas dentro de la aplicación móvil. Mientras la mayoría de pantallas usan Soles (S/), la vista de detalles de gastos utiliza el signo de Dólares ($). Esto genera incertidumbre financiera crítica en una app de gestión de gastos.
* **Recomendación:** Configurar una variable global de moneda que se aplique a toda la interfaz según la preferencia del hogar, asegurando que el símbolo sea idéntico en todas las pantallas.
### PROBLEMA #10: Navegación inferior (Tab Bar) inconsistente
* **Severidad:** 4
* **Heurística violada:** Usabilidad - Consistencia y estándares
* **Problema:** El menú inferior (Tab Bar) no mantiene una estructura fija. En la pantalla de gastos aparece la opción "Bills", mientras que en la de invitaciones es reemplazada por "Members", y en el seguimiento por "Contributions". Esto desorienta al usuario al cambiarle las rutas principales de navegación según la pantalla en la que se encuentre.
* Recomendación:** Definir un set de 4 o 5 iconos globales que representen las secciones más importantes del sistema y mantenerlos estáticos en toda la aplicación móvil.

### PROBLEMA #11: Control de fecha con botones internos confusos
* **Severidad:** 3
* **Heurística violada:** Usabilidad - Libertad y control del usuario
* **Problema:** El componente de selección de fecha incluye botones de "Set" y "Cancel" como parte de la misma fila de entrada. Esto rompe el flujo natural de introducción de datos y puede causar que el usuario cancele el proceso por error al intentar ajustar el día o el mes.
* **Recomendación:** Implementar un Date Picker nativo del sistema operativo (iOS/Android) que se despliegue en un modal o menú inferior independiente.

### PROBLEMA #12: Variación de etiquetas de retroceso ("Back" vs "Go back")
* **Severidad:** 1
* **Heurística violada:** Usabilidad - Consistencia y estándares
* **Problema:** Existe una falta de consistencia en las etiquetas textuales asignadas a los botones de navegación de retorno en la barra superior de la interfaz móvil. En ciertas vistas se utiliza el texto "< Back", mientras que en otras pantallas de la misma aplicación se visualiza como "< Go back". Esta variabilidad rompe con el principio de uniformidad y previsibilidad del sistema.
* **Recomendación:** Estandarizar un único formato de botón de retroceso para todas las pantallas de la aplicación móvil (se sugiere adoptar la etiqueta estándar "< Back" o emplear únicamente un icono de flecha limpia) para unificar la experiencia de navegación.

### PROBLEMA #13: Botones de sistema incrustados dentro de inputs de texto
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Estética y diseño minimalista
* **Problema:** Los botones de acción interactivos del sistema, tales como "Search" y "Generate ID", se encuentran posicionados directamente dentro del contenedor interno del campo de texto de entrada. Este patrón de diseño compromete el espacio útil horizontal para la introducción y lectura de datos por parte del usuario, además de saturar la jerarquía visual dentro de los formularios.
* **Recomendación:** Extraer los botones de acción fuera de las cajas de texto y reubicarlos de manera externa (ya sea al lado derecho como un elemento adyacente o debajo del campo correspondiente) para asegurar un área de entrada limpia, espaciosa y legible.

### PROBLEMA #14: Contraste crítico de accesibilidad en el Login
* **Severidad:** 3
* **Heurística violada:** Diseño Inclusivo - Experiencias comparables
* **Problema:** En la pantalla de inicio de sesión, las etiquetas de los campos ("Email", "Password") utilizan un color azul oscuro sobre un fondo negro. Esta combinación no cumple con los estándares mínimos de contraste de la WCAG, dificultando severamente la lectura para personas con visión reducida o en entornos con mucha luz.
* Recomendación:** Cambiar el color de las etiquetas a blanco o un gris de alta luminancia para asegurar una legibilidad universal.

----------------------------------------------------------------------------
----------------------------------------------------------------------------
# Evaluación según Heurísticas (Evaluación a otro grupo)

- **CARRERA:** Ingeniería de Software
- **CURSO:** 1acc0238 Aplicaciones para dispositivos móviles
- **SECCIÓN:** Todos
- **AUDITOR:** Grupo 3
- **CLIENTE(S):** Grupo 2

---
## SITE o APP A EVALUAR:

SoftWork    

## 1. Tareas a Evaluar 
El alcance de esta evaluación incluye la revisión de la usabilidad de las siguientes tareas tanto en la Landing Page como en la aplicación móvil (flujos de Empleado y RRHH):

1. Identificación de la propuesta de valor.
2. Registro de un usuario nuevo con validación de correo corporativo.
3. Inicio de sesión seguro.
4. Selección de planes de membresía y registro de método de pago.
5. Configuración de preferencias de privacidad en el perfil.
6. Interacción comunitaria: lectura, publicación y votación en foros anónimos.
7. Cumplimentación de encuestas diarias de clima laboral y bienestar.
8. Gestión y visualización de reportes de clima por equipos (Rol RRHH).
9. Revisión del centro de notificaciones y alertas.

---

## 2. Escala de Severidad
Los problemas detectados se puntúan bajo la siguiente métrica:

* **1. Problema superficial:** Ocurre con muy poca frecuencia; no necesita ser arreglado a menos que exista disponibilidad de tiempo.
* **2. Problema menor:** Se le debería asignar una prioridad baja de cara al siguiente release.
* **3. Problema mayor:** Ocurre frecuentemente; es importante que sean corregidos con prioridad alta.
* **4. Problema muy grave:** Impide al usuario continuar con el uso de la herramienta; imperativo corregir antes del lanzamiento.

---

## 3. Tabla Resumen

| #   | Problema                                                | Severidad | Heurística/Principio Violada(o)                        |
| :-- |:--------------------------------------------------------| :-------: | :----------------------------------------------------- |
| 1   | Desorden ilógico en el eje Y del gráfico de reportes    |   **4** | Usability: Prevención de errores / Consistencia        |
| 2   | Enlaces inoperativos en la Landing Page                 |   **3** | Information Architecture: Is it usable?                |
| 3   | Inconsistencia de idioma en formulario de tarjeta       |   **1** | Usability: Consistencia y estándares                   |
| 4   | Botón principal de "Iniciar sesión" en web sin ruta     |   **4** | Usability: Control y libertad del usuario              |
| 5   | Formato de fecha extranjero en el dashboard de RRHH     |   **2** | Usability: Relación entre el sistema y el mundo real   |
| 6   | Contraste insuficiente en enlaces de login/registro     |   **3** | Inclusive Design: Diseño accesible                     |
| 7   | Pantallas de éxito carentes de contexto o resumen       |   **2** | Usability: Visibilidad del estado del sistema          |
| 8   | Ausencia de fechas explícitas en notificaciones de pago |   **2** | Usability: Reconocimiento antes que recuerdo           |
| 9   | Semántica de colores confusa en tarjetas del dashboard  |   **3** | Usability: Consistencia y estándares                   |
| 10  | Estados vacíos sin orientación a la acción              |   **2** | Usability: Ayudar a los usuarios a reconocer errores   |
| 11  | Ambigüedad visual en el estado por defecto del dropdown |   **2** | Usability: Estética y diseño minimalista               |
| 12  | Duplicidad de acceso a "Métodos de pago" para RRHH      |   **1** | Information Architecture: Is it findable?              |
| 13  | Botón flotante en el foro sin etiqueta descriptiva      |   **2** | Usability: Reconocimiento antes que recuerdo           |
| 14  | Falta de botón de cancelación en el modal de encuesta   |   **3** | Usability: Control y libertad del usuario              |

---

## 4. Descripción de Problemas

### **PROBLEMA #1: Desorden ilógico en el eje Y del gráfico de reportes**
* **Severidad:** 4
* **Heurística violada:** Usabilidad - Prevención de errores / Consistencia
* **Problema:** En la pantalla de "Reportes" (vista RRHH), el gráfico de líneas presenta un eje Y completamente desordenado numéricamente ("10, 0, 80, 50, 20, 10"). Esto hace que la visualización de datos de clima laboral sea totalmente inútil, impidiendo al analista interpretar la evolución del equipo.
* **Recomendación:** Corregir la lógica de renderizado del componente del gráfico para que el eje Y mantenga un orden ascendente estricto (ej. 0, 20, 40, 60, 80, 100).

### **PROBLEMA #2: Enlaces inoperativos (anclas `#`) en la Landing Page**
* **Severidad:** 3
* **Heurística violada:** Arquitectura de Información - ¿Es usable?
* **Problema:** En el *footer* y en la navegación principal de la página web promocional, varios enlaces clave (como "Hablar con ventas", "Integraciones" y todas las políticas legales) apuntan a un ancla vacía (`#`). El usuario hace clic esperando información vital y no ocurre ninguna acción.
* **Recomendación:** Deshabilitar y ocultar estos enlaces si las páginas aún no existen en esta fase del proyecto, o enlazar a un modal de "Próximamente" para no romper el flujo de navegación.

### **PROBLEMA #3: Inconsistencia de idioma en formulario de tarjeta**
* **Severidad:** 1
* **Heurística violada:** Usabilidad - Consistencia y estándares
* **Problema:** En la pantalla "Agregar método de pago" de la aplicación móvil, los *placeholders* de los campos de texto están en inglés ("Name on the card", "Card number", "Month / Year"), a pesar de que toda la interfaz y los títulos de la app están en español.
* **Recomendación:** Traducir los atributos de marcador de posición (placeholders) al español ("Nombre en la tarjeta", "Número de tarjeta", "Mes / Año") para mantener la cohesión del idioma.

### **PROBLEMA #4: Botón principal de "Iniciar sesión" en web sin ruta**
* **Severidad:** 4
* **Heurística violada:** Usabilidad - Control y libertad del usuario
* **Problema:** En la cabecera de la *landing page*, el botón primario de "Iniciar sesión" apunta a `#`. Esto bloquea completamente a los usuarios existentes que intentan ingresar a la plataforma web desde la página principal.
* **Recomendación:** Enlazar inmediatamente el botón al subdominio de la aplicación (ej. `app.softwork.com/login`) o a la vista web de autenticación.

### **PROBLEMA #5: Formato de fecha extranjero en el dashboard de RRHH**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Relación entre el sistema y el mundo real
* **Problema:** En el eje X del gráfico de reportes, las fechas están formateadas en el estándar estadounidense "Mes/Día" (ej. "3/19", "3/20"). Para usuarios en Latinoamérica o España, esto resulta antinatural y puede causar confusión temporal.
* **Recomendación:** Adaptar el formato de fecha a la configuración regional del usuario, utilizando el estándar "Día/Mes" (ej. "19/03", "20/03").

### **PROBLEMA #6: Contraste insuficiente en enlaces de login/registro**
* **Severidad:** 3
* **Heurística violada:** Diseño Inclusivo - Diseño accesible
* **Problema:** En las pantallas de autenticación de la app móvil, textos como "¿Olvidaste tu contraseña?" y "Registrate" utilizan un tono de azul claro sobre fondo blanco que no alcanza el ratio mínimo de contraste de la WCAG (4.5:1). Esto dificulta la lectura para personas con baja visión.
* **Recomendación:** Oscurecer el código hexadecimal del color azul en estos enlaces de texto para cumplir con los estándares de accesibilidad visual.

### **PROBLEMA #7: Pantallas de éxito carentes de contexto o resumen**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Visibilidad del estado del sistema
* **Problema:** Tras realizar una compra o registrarse, la app muestra una pantalla blanca dominada casi por completo por un *check* gigante y el texto "Membresía adquirida" o "Usuario registrado". No se ofrece un recibo rápido, el correo registrado, ni el tipo de plan comprado, lo que genera dudas sobre si la transacción fue correcta.
* **Recomendación:** Incluir una pequeña tarjeta de resumen debajo del check (ej. "Plan Pro - S/. 99 cobrados a tu tarjeta terminada en 4521") antes del botón de "Menú inicial".

### **PROBLEMA #8: Ausencia de fechas explícitas en notificaciones de pago**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Reconocimiento antes que recuerdo
* **Problema:** En la pestaña de Notificaciones, la alerta de pago indica "Tu plan vencerá pronto". Al no especificar la fecha exacta de vencimiento en la misma tarjeta, obliga al usuario a recordar la fecha de facturación o a hacer clics innecesarios para averiguarlo.
* **Recomendación:** Dinamizar el texto para que incluya la fecha concreta: "Tu plan vencerá el 27 de Mayo. Actualiza tu método de pago".

### **PROBLEMA #9: Semántica de colores confusa en tarjetas del dashboard**
* **Severidad:** 3
* **Heurística violada:** Usabilidad - Consistencia y estándares
* **Problema:** En la pantalla de Reportes (vista RRHH), las tarjetas superiores utilizan colores pastel de fondo (celeste, verde, rojo, morado) que parecen ser meramente decorativos. Sin embargo, el rojo en "Reportes en foro: 1" transmite una alerta de error grave instintivamente, mientras que el verde en "Integrantes: 5" no representa un estado de éxito real.
* **Recomendación:** Utilizar un esquema de colores neutro (blanco/gris) para los contenedores y reservar los colores semánticos (rojo, amarillo, verde) únicamente para los iconos o indicadores numéricos que representen cambios positivos o críticos.

### **PROBLEMA #10: Estados vacíos sin orientación a la acción**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Ayudar a los usuarios a reconocer, diagnosticar y recuperarse de errores
* **Problema:** En la pantalla "Historial de pagos", si no hay registros, solo se lee el texto "No ha realizado ningún pago" flotando en el espacio en blanco. No hay ilustración, ni un botón que sugiera la siguiente acción lógica (como "Adquirir un plan").
* **Recomendación:** Diseñar estados vacíos amigables que incluyan un gráfico ligero y un Call to Action (CTA) que dirija al usuario a resolver esa "ausencia" de datos.

### **PROBLEMA #11: Ambigüedad visual en el estado por defecto del dropdown**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Estética y diseño minimalista
* **Problema:** En la pantalla inicial de "Reportes", el selector de equipos dice "Ninguno" por defecto, dejando casi el 90% de la pantalla en un blanco absoluto sin instrucciones. Da la sensación de ser un error de carga o una pantalla inacabada.
* **Recomendación:** Cambiar el texto "Ninguno" por un placeholder instruccional como "Selecciona un equipo" y colocar un gráfico tenue de fondo con el texto "Elige un equipo de la lista para visualizar sus métricas de clima".

### **PROBLEMA #12: Duplicidad de acceso a "Métodos de pago" para RRHH**
* **Severidad:** 1
* **Heurística violada:** Arquitectura de Información - ¿Es fácil de encontrar?
* **Problema:** Para los perfiles de pago, la opción para gestionar o ver la facturación parece estar distribuida tanto en el "Perfil" del usuario como directamente expuesta en el "Menú inicial" mediante botones grandes. Esto infla la carga cognitiva sin necesidad.
* **Recomendación:** Consolidar todo lo relacionado a facturación y pagos bajo una única ruta (preferiblemente dentro de "Mi Perfil" o "Configuración") para limpiar el dashboard principal.

### **PROBLEMA #13: Botón flotante en el foro sin etiqueta descriptiva**
* **Severidad:** 2
* **Heurística violada:** Usabilidad - Reconocimiento antes que recuerdo
* **Problema:** En la pantalla del Foro, hay un Floating Action Button (FAB) en la esquina inferior derecha con un simple ícono de suma (+). Aunque es un patrón común, en contextos laborales complejos, un ícono solitario puede dejar dudas sobre si es para "Crear post", "Invitar persona" o "Crear encuesta".
* **Recomendación:** Al hacer scroll hacia arriba, expandir momentáneamente el FAB para mostrar el texto "Nueva publicación" junto al ícono (+), asegurando la claridad de la acción.

### **PROBLEMA #14: Falta de botón de cancelación en el modal de encuesta**
* **Severidad:** 3
* **Heurística violada:** Usabilidad - Control y libertad del usuario
* **Problema:** Una vez que el usuario ingresa a la pantalla de "Encuesta" (¿Cómo te sientes hoy?), no existe una "X" visible o un botón de "Cancelar" claro en la parte superior. El usuario podría sentirse atrapado y obligado a enviar la encuesta para poder regresar al menú.
* **Recomendación:** Añadir un ícono de "X" o una flecha de retroceso explícita en la esquina superior izquierda de la vista de la encuesta para garantizar una salida segura sin enviar datos.



# Conclusiones y recomendaciones

## Conclusiones
- Las sesiones de validación confirmaron nuestra hipótesis principal respecto a la equidad financiera: la automatización del cálculo proporcional de gastos basado en los ingresos reales disminuye significativamente las tensiones domésticas. Los resultados demostraron que la aplicación móvil resuelve de forma efectiva la problemática planteada en los Problem Statements, logrando que tanto los representantes del hogar como los convivientes confíen en el algoritmo de distribución y perciban un alto valor en la transparencia de la información compartida.

- Frente a los assumptions de riesgo iniciales sobre una posible resistencia tecnológica o desconfianza al registrar datos financieros personales, las validaciones evidenciaron una rápida curva de adopción. Esto se logró gracias a la usabilidad de la interfaz y a la integración ágil de los recursos del dispositivo (como el uso de la cámara para registrar recibos). Se concluye que la solución, apoyada por una propuesta de valor clara desde el Landing Page, supera las barreras de entrada y cumple satisfactoriamente con los criterios de éxito definidos en el ciclo Lean UX.

## Recomendaciones

- Dentro del roadmap a corto y mediano plazo de la aplicación móvil, se sugiere priorizar la expansión de las integraciones con billeteras digitales locales y pasarelas de pago externas. Las validaciones indicaron que los usuarios buscan liquidar sus deudas con la menor cantidad de fricción posible, por lo que agilizar el flujo de pago directo in-app será vital para la retención y la reducción de la morosidad.


## Video About the Product

<br>
<img src="assets/VideoAboutTheProduct.jpg" alt="videabouttheproduct">
<br>

- Duración: 6:12 mins

- Youtube: https://www.youtube.com/watch?v=NVFVIfCgTQ4
- Microsoft: https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231c540_upc_edu_pe/IQBxWyY8_jhcQILuW-XuEOtQAR76RRQ-3nte36kfHOY16HU?e=cgvTo8&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D



## Video App Validation

<br>
<img src="assets/videoAppValidation.jpg" alt="videabouttheproduct">
<br>

- Youtube: https://youtu.be/AKwF7MdLJfs

- Microsoft:https://upcedupe-my.sharepoint.com/:v:/g/personal/u20231c540_upc_edu_pe/IQDKI97wfxZsT6ojQ84-Z26DAcRBgbcwj5sN4bSOb-4Na9U?e=wSybbE&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0%3D

