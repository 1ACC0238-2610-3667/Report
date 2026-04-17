## 1.1 Startup Profile

### 1.1.1 Descripción de la Startup

**SymmetriQ** es una empresa emergente del sector tecnológico dedicada a desarrollar soluciones innovadoras para la gestión financiera en entornos de convivencia. Su producto principal, **Harmonix**, está diseñado para facilitar la organización y distribución equitativa de los gastos compartidos del hogar, considerando los ingresos de cada miembro.  

A través de un sistema digital automatizado, claro y accesible, Harmonix fomenta la responsabilidad económica, la comunicación eficaz y la adecuada gestión del presupuesto común, reduciendo conflictos y fortaleciendo una cultura de colaboración dentro del hogar.

**Título:** Harmonix  

**Misión:** Brindar un manejo eficiente de las finanzas compartidas mediante una solución orientada a dispositivos móviles que distribuye los gastos de forma proporcional a los ingresos de cada integrante, fomentando la equidad, la claridad y una convivencia armoniosa.

**Visión:** Convertirse en la plataforma líder en la gestión financiera compartida en los hogares, reconocida por empoderar a las personas para tomar decisiones económicas justas, responsables y colaborativas. 

**Principios:** Transparencia, justicia y colaboración. 

### 1.1.2 Perfiles de integrantes del equipo

| Integrante | Descripción Personal | Conocimientos Técnicos |
|-------------|----------------------|-------------------------|
| **José Luis Martínez Valdivia - u202213989** <br> |       |         |
| **Héctor Javier Rios Pacheco - u20231c540**<br> <img src="assets/integrantes/FotoHector.png" alt="foto-hector" width="170px"/>   |  Soy responsable, me gusta involucrarme activamente en los proyectos, aportar ideas útiles y cumplir con mis tareas a tiempo. Siempre estoy dispuesto a colaborar y ayudar al equipo a avanzar de la mejor manera posible.     |  Cuento con formación en desarrollo de software, incluyendo estructuras de datos, algoritmos y arquitecturas orientadas a servicios. Trabajo con lenguajes como Java, TypeScript, JavaScript, HTML5 y CSS3, y utilizo herramientas y frameworks como Angular, Spring Boot, Git/GitHub, Swagger y bases de datos relacionales.       |
| **JoaquinAlberto Cuentas Peña - u20201f788**<br>|       |         |
| **Walter Luis Fajardo Monrroy - u202221632**<br>   |       |         |
| **Rodrigo Jesús Miraval Pomalaya**<br>    |       |         |


## 1.2. Solution Profile

**Harmonix**, producto desarrollado por **SymmetriQ**, es una solución integral compuesta por una aplicación móvil (nativa/multiplataforma) y un sitio web estático (Landing Page)l diseñada para facilitar la distribución equitativa de los gastos del hogar entre sus miembros, considerando los ingresos personales de cada individuo. La plataforma calcula automáticamente el aporte correspondiente de cada integrante, basándose en su situación económica, y garantiza así una distribución justa de los gastos compartidos como alquiler, servicios esenciales y alimentos.  

Técnicamente, la aplicación móvil aprovecha las capacidades del dispositivo para optimizar la experiencia del usuario: soporte de almacenamiento local, y acceso a recursos internos del dispositivo (como la cámara para registrar recibos y pagos realizados). Además, toda la lógica de negocio se integra de forma segura con un servicio RESTful de desarrollo interno, y se conecta a un servicio externo de terceros (pasarela de pagos) para procesar y validar las transferencias directamente desde la app.

Los usuarios pueden registrar sus ingresos, conocer cuánto deben contribuir y monitorear sus pagos, mientras que la persona responsable de la gestión del hogar obtiene una visión integral del proceso. Además, Harmonix ofrece monitoreo en tiempo real, informes mensuales claros y alertas de pagos pendientes mediante notificaciones push en sus dispositivos.

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

