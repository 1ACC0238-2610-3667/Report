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


### 2.4. Ubiquitous Language

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
