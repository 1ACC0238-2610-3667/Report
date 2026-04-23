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
9. ¿Cree que una aplicación como Harmonix podría ayudar a mejorar la convivencia y la organización en su hogar?

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
7. ¿Qué funcionalidades le gustaría que tenga una app como SplitEasy?
8. ¿Qué tan importante considera la transparencia financiera dentro del hogar?
9. ¿Estaría dispuesto(a) a registrar los ingresos de cada miembro para que la aplicación calcule automáticamente cuánto debe aportar cada uno?
10. ¿Qué beneficios cree que traería una solución como Harmonix en la convivencia familiar?


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

