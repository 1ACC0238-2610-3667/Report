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
| **José Luis Martínez Valdivia - u202213989** <br> |       |         |
| **Héctor Javier Rios Pacheco - u20231c540**<br> <img src="assets/integrantes/FotoHector.png" alt="foto-hector" width="170px"/>   |  Soy responsable, me gusta involucrarme activamente en los proyectos, aportar ideas útiles y cumplir con mis tareas a tiempo. Siempre estoy dispuesto a colaborar y ayudar al equipo a avanzar de la mejor manera posible.     |  Cuento con formación en desarrollo de software, incluyendo estructuras de datos, algoritmos y arquitecturas orientadas a servicios. Trabajo con lenguajes como Java, TypeScript, JavaScript, HTML5 y CSS3, y utilizo herramientas y frameworks como Angular, Spring Boot, Git/GitHub, Swagger y bases de datos relacionales.       |
| **JoaquinAlberto Cuentas Peña - u20201f788**<br>|       |         |
| **Walter Luis Fajardo Monrroy - u202221632**<br>   |       |         |
| **Rodrigo Jesús Miraval Pomalaya**<br>    |       |         |


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
