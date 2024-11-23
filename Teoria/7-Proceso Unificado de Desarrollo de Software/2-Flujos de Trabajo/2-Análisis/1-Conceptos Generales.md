## ANALISIS

La fase de análisis en el desarrollo de software tiene como objetivo refinar y estructurar los requisitos capturados previamente, permitiendo una comprensión más precisa y detallada del sistema.

### Importancia del Análisis

1. Refinamiento de Requisitos: El análisis busca resolver los aspectos no tratados durante la captura de requisitos, los cuales, debido al uso del lenguaje natural del cliente, pueden haber quedado imprecisos o incompletos. Se utiliza un lenguaje más formal y técnico, adecuado para desarrolladores, para aclarar estos detalles. COMPRENSIÓN DETALLADA 
    
2. Estructuración y Mantenibilidad: El análisis permite estructurar los requisitos de manera que sean más fáciles de comprender, modificar y mantener. Esta estructura, que se basa en clases de análisis y paquetes, no depende de la estructura definida en los casos de uso, pero existe una trazabilidad directa entre ambas. Esto asegura que las diferentes descripciones de un mismo requisito se mantengan consistentes a lo largo del tiempo.
    

### Problemas no Resueltos en la Captura de Requisitos

1. Interferencia, Concurrencia y Conflictos entre Casos de Uso:
    

- Pueden surgir conflictos cuando varios casos de uso compiten por recursos compartidos del sistema. Por ejemplo, "Ingresar Dinero" y "Sacar Dinero" pueden acceder a la misma cuenta bancaria, lo que puede generar problemas de concurrencia. El análisis permite resolver estos conflictos.
    

3. Lenguaje del Cliente:
    

- El análisis permite introducir un lenguaje más formal (diagramas de estado, actividad, interacción, etc.) para detallar con mayor precisión los aspectos funcionales y no funcionales del sistema.
    

5. Redundancias y Descomposición de Casos de Uso:
    

- En el análisis, se puede encontrar un equilibrio entre la comprensibilidad y la mantenibilidad, descomponiendo los requisitos de manera que faciliten el diseño e implementación del sistema.
    

### Propósito del Análisis

El propósito del análisis es resolver los problemas y ambigüedades que puedan haber surgido en la captura de requisitos, utilizando un enfoque más formal y técnico. Además, el análisis permite estructurar los requisitos de forma que sean más manejables a largo plazo, preparando el terreno para las fases de diseño y desarrollo del sistema.

  

  

Cuadro comparativo del modelo de casos de uso con el modelo de análisis![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXclcRXUWs63HZ23wNA47nrmFPe-KJJ4JnqgEzpXUcl9Z7wt1IgvHH57AImoz9HSCazNraZdh669MTAhoWZt3_3lbxaSCppDW-g4c1RKrBTnijnoXT2Q03rzMVDIBnG0SlSz8rAxjDAZTFjSSmG7zZe6ub6e?key=VReuh94fGGpJZLGsXsGdUQ)

Análisis y el Ciclo de Vida:

Se tienen variantes en diferentes proyectos (se analiza el costo/beneficio):

- Usar el modelo de análisis y mantenerlo. Costoso, pero es lo que más detalle da
    
- Usarlo y no mantenerlo. Durante las primeras etapas, usualmente la elección
    
- No usarlo. Se puede saltar directamente al modelo de diseño
    

  

  

  

  

  

  

  

  

### TRABAJADORES Y ARTEFACTOS![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfmDrmu2V2iZbFxCAVnY7oFF2jsjf3c_P0gcmHCWOW3uGEAJJKGbezeeQd3gFj_Rul1DhFzL4466-qeLkPM3Oa_Z3ej9_6cneh-dTtt7PJD2HwLHlnX_YChR_eibVvkYlA-qTUCdDMgvC_m2CyBdAgyzhUT?key=VReuh94fGGpJZLGsXsGdUQ)

El análisis es fundamental para poder afinar y estructurar los CU de la etapa anterior, y el cómo se hace todo eso se deja para los flujos de diseño e implementación. 

En este flujo que ocurre durante las primeras iteraciones de la fase de elaboración vamos obteniendo una arquitectura más estable y requisitos más definidos.

#### ARTEFACTOS

- MODELO DE ANÁLISIS![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUExzjy09MphNwxPfXrN2jEYsAghrpedNz6qeY7_N5rO8mUTJvufYQtR3bPOz_SfAJ66UTVmswtAx1Hq5aFTDQTqr5_mzR5Lyzp2QoixvLjDjPwCo2wKhI8s7ma4HqV0MdlqtgzWrwqE4H7Z6fm1zNvAjM?key=VReuh94fGGpJZLGsXsGdUQ)
    

Se estructura jerárquicamente mediante un sistema de análisis en el nivel más alto, subdividido en paquetes que representan subsistemas o capas del diseño.

Paquetes de análisis: Agrupan partes manejables del sistema, facilitando la comprensión y manejo de la complejidad.

Clases de análisis: Son abstracciones de clases del diseño, representando componentes del sistema que se refinan desde los requisitos.

Realizaciones de casos de uso: Describen cómo los casos de uso interactúan mediante colaboraciones entre clases de análisis.

- CLASES DE ANÁLISIS![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeynIrWzra1wlq0ruTE9fEFrLDqhIFd86cpI-YyF4nDYL16KEYovDFeRPR6xkZNdSB7jNp0CD7W_b8QqVgvUIWry1jDRSooKDicq_AdL8AzZcJYlhd_ZgKAVcKJnjQZwwtsJyTDlfDBGi_m-3e5QsJ3Psk?key=VReuh94fGGpJZLGsXsGdUQ)
    

Abstracción: Representan una abstracción de clases o subsistemas del diseño, centradas en los requisitos funcionales.

Nivel conceptual: Son más conceptuales y de mayor granularidad que las clases de diseño, enfocándose en el dominio del problema.

Responsabilidades: En lugar de definir operaciones, describen el comportamiento mediante responsabilidades de manera textual.

Atributos: Los atributos son de alto nivel y se basan en conceptos del dominio del problema. Algunos atributos pueden convertirse en clases durante el diseño.

Relaciones conceptuales: Las relaciones entre clases de análisis son menos formales y la navegabilidad no es crucial como en el diseño.

Estereotipos: Las clases de análisis se dividen en tres tipos: 

Clases de Interfaz:

- Modelan la interacción entre el sistema y los actores (usuarios o sistemas externos).
    
- Abstracciones de interfaces como ventanas, formularios, API, etc.
    
- Describen qué información se intercambia, sin entrar en detalles de implementación.
    
- Aisladas para facilitar cambios en interfaces.
    

Clases de Entidad:

- Modelan información persistente y de larga duración (personas, objetos, sucesos).
    
- Derivadas de clases del dominio del negocio.
    
- Reflejan la información de manera que beneficie el diseño y la implementación, aislando cambios.
    
- Pueden tener comportamiento complejo relacionado con la información que manejan.
    

Clases de Control:

- Encapsulan la lógica de control, secuencia, transacciones y coordinación de otros objetos.
    
- Usadas para manejar la lógica de negocio o casos de uso complejos.
    
- Aíslan cambios en el control y la lógica, delegando trabajo a otras clases (interfaz o entidad).
    
- REALIZACIÓN DE CASO DE USO-ANÁLISIS![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcm3ekxyn5eKLgTa0NTwIc4iFwuA_xOuw1jbS8lgb2L7smscIxCBeuuKc9oG8WLL-t2_sVCo4YlX_ecuRhYUq6qqZJw8tjTeoUKPSN9GXa4mo3EKH9nM0GOJizz9BO3dHXgxhtsX8_ohFh7n_1pIwdXyTmi?key=VReuh94fGGpJZLGsXsGdUQ)
    

Describe cómo se ejecuta un caso de uso en términos de clases y objetos de análisis. Incluye una traza hacia el modelo de casos de uso.  
Componentes:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeaZAH2V3lAOKy4tvU6nh8VtvHYRSkTExr4ZY6GgoNw8kagxEbN4xvKUn0a_fqGOjKwP2L9_GoHcZEKrkZpXUnNfnYWxPOImmvY8QjvR6fwkYlRiLHueb0JwQa20eXXiS9oApp1t9qvLxiD2cnbzz5gKd9g?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeXBoukZ2uyGFYFPV74_0lqMK_vQKnBDP8be8JRtYITcRY7_aaK3SbB4nkuvqebeoUB2f0m_kpgeRvmVN-MGfIS8tPZsAhLuPmdG-ezmRcHtwWEZHg1FnEPq5g1OZDjEPa9saQIxdjQkj-q8ulSKzk7ruU8?key=VReuh94fGGpJZLGsXsGdUQ)

- Descripción textual del flujo de sucesos.
    
- Diagramas de clases y de interacción para representar la ejecución del caso de uso.
    

Enfoque: Se centra en los requisitos funcionales, dejando los no funcionales (requisitos especiales) para las fases de diseño e implementación.

  

  

  

  

  

Diagramas de Clases: Muestran las clases participantes en un caso de uso y sus relaciones. Se usan para coordinar los requisitos de diferentes casos de uso sobre una clase.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeBB90pSQEKh6EYFn2W-DjEZkgfet94jm_pVPch3LPeAegbdhvbHXpniO1WjHxOqda_snE4wy9ptROPIJiqvkUy8cw2hR509rUvugXkOnAS-_yjMvBOFkKZXpA5AVX1PKJEVXdrfr10UmpXbCloMMPfIS1P?key=VReuh94fGGpJZLGsXsGdUQ)

Diagramas de Interacción: Muestran cómo interactúan los objetos para llevar a cabo el caso de uso. Se prefieren los diagramas de colaboración en el análisis para identificar responsabilidades de los objetos ante qué sucesos en orden cronológico.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXewzt8w8xMspPNvLnjEmXPjVclnSUuagvRqGxAL7ZymBnR5_3oDULdciVzEhveFIzjAB7Y2ppxVFyj1O38QTpXSZJr_Jr8HnLAb-_46LQNU5I2PHe-hbKBgNH7oUe2Cp1lREKrIJllK6TEbyk3BMdyWocoi?key=VReuh94fGGpJZLGsXsGdUQ)

Ciclo de vida de objetos:

- Objetos de interfaz: Pueden crearse y destruirse en una sola realización de caso de uso.
    
- Objetos de entidad: Tienen una vida larga y participan en varias realizaciones de casos de uso.
    
- Objetos de control: Se crean al inicio del caso de uso y se destruyen al finalizar, aunque hay excepciones.
    

Flujo de sucesos: Descripción textual de un diagrama de colaboración, sin entrar en detalles de atributos, responsabilidades, asociaciones, etc.  
  
Requisitos especiales: Textos que recogen requisitos no funcionales, algunos capturados previamente y otros derivados durante el análisis.

- PAQUETES DE ANÁLISIS
    

Es una herramienta que permite organizar los artefactos del modelo de análisis en unidades más manejables. Es un concepto clave en la estructura de los sistemas, especialmente en proyectos grandes, ya que facilita la separación de responsabilidades y permite el trabajo concurrente entre distintos equipos. Un paquete de análisis puede incluir clases de análisis, realizaciones de casos de uso y otros paquetes.

Las características clave de los paquetes de análisis son:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdBa6ZXQM-4uMcjeZ1hzJmk7yVPI_xJON_9U6hXkkJ3EXpuwOwuiG_RRzVRtQww6dvjiw6TpWuIevrROLAHpIRjs-8xyiSdpEAK0TDPeM_5NJ1VmUHhEBf31v7B1LI93Z2in-sGGZk-tqyO29o127ZfLQxT?key=VReuh94fGGpJZLGsXsGdUQ)

1. Cohesión: Los elementos dentro de un paquete deben estar fuertemente relacionados, lo que significa que las clases y casos de uso que contiene deben tener objetivos comunes.
    
2. Bajo acoplamiento: Las dependencias entre diferentes paquetes deben ser mínimas, lo que facilita el mantenimiento y la evolución del sistema.
    
3. Particionamientos funcionales del sistema: Los paquetes pueden representar diferentes áreas del sistema, que pueden ser trabajadas de manera independiente por diferentes equipos de desarrollo.
    
4. Basados en el dominio del problema: Se estructuran en torno a los requisitos funcionales y las necesidades del negocio, no en los requisitos técnicos o no funcionales.
    

Paquetes de servicio

Representan una agrupación de funcionalidad relacionada que puede ser utilizada en varios casos de uso. Son fundamentales para estructurar sistemas en términos de los servicios que proporcionan, y su diseño es clave para lograr una alta cohesión y bajo acoplamiento.

Características importantes de los paquetes de servicio:

- Indivisibilidad: Un cliente del sistema obtiene un paquete de servicio completo o no obtiene nada. Los paquetes de servicio no se pueden dividir en partes menores.
    
- Relevancia para varios casos de uso: Puede ser utilizado por múltiples casos de uso y suele ser relevante para uno o pocos actores del sistema.
    
- Mutuamente excluyentes o variantes: Pueden ser excluyentes o pueden representar variantes de un mismo servicio (por ejemplo, diferentes versiones de una funcionalidad).
    
- Reutilizables: Debido a su cohesión y bajo acoplamiento, los paquetes de servicio son reutilizables tanto dentro del mismo sistema como en otros sistemas relacionados. Esto es especialmente cierto para aquellos centrados en clases de entidad, que representan objetos del dominio del negocio.
    
- Evolución del sistema: Estructurar el sistema en torno a paquetes de servicio facilita la localización de cambios, lo que contribuye a que el sistema sea más robusto y resistente a los cambios.
    
- DESCRIPCIÓN DE LA ARQUITECTURA (VISTA MODELO ANÁLISIS)
    

La descripción de la arquitectura resalta los artefactos clave del modelo de análisis que influyen en el diseño e implementación:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfkkmG-AQxvcBApeeTbomeyZIAJd-uTVBRR4TS4YNSo8mQE6yefJWfJNJXPkB04a3koRrkA1YY9TeDZEVcPB7hetIU8_IMxauyZr_pw_Ety4hbsOvMHPtsfpAZmBic_j4r97AtAT8lSLv3tuYLxPnIkpIhE?key=VReuh94fGGpJZLGsXsGdUQ)

1. Paquetes de análisis y dependencias: La descomposición del sistema en paquetes afecta directamente la estructura de los subsistemas y sus interacciones.
    
2. Clases fundamentales:
    

- Clases de entidad: Encapsulan fenómenos clave del dominio.
    
- Clases de interfaz: Gestionan las interacciones del usuario.
    
- Clases de control: Coordinan secuencias críticas.
    

4. Realizaciones de casos de uso: Describen funcionalidad crítica, cubren múltiples clases y paquetes, y son clave para el desarrollo temprano.
    

#### TRABAJADORES

Arquitecto:

- Responsable de la integridad del modelo de análisis, asegurando su corrección, consistencia y legibilidad.
    
- Mantiene las partes significativas para la arquitectura.
    
- Puede delegar tareas rutinarias a otros trabajadores, pero sigue siendo responsable de la descripción de la arquitectura.
    
- No gestiona el desarrollo continuo de artefactos del modelo de análisis.
    

Ingeniero de casos de uso:

- Responsable de la realización de casos de uso, asegurando que cumplen los requisitos y se ajustan a sus descripciones.
    
- No es responsable de las clases o relaciones del análisis.
    
- También diseña las realizaciones de casos de uso, facilitando una transición suave entre análisis y diseño.
    

Ingeniero de componentes:

- Mantiene las clases de análisis y sus atributos, relaciones y responsabilidades.
    
- Responsable de paquetes de análisis, asegurando que sus dependencias son mínimas y correctas.
    
- Si es posible, también se encarga de los subsistemas de diseño asociados al paquete de análisis.
    

  

### FLUJO DE TRABAJO - ACTIVIDADES

Comienza con los arquitectos, quienes crean el modelo de análisis identificando los paquetes principales, clases de entidad y requisitos comunes. Luego, los ingenieros de casos de uso desarrollan cada caso de uso con base en estas clases, detallando los comportamientos requeridos. Después, los ingenieros de componentes definen y consolidan estos requisitos, asignando responsabilidades, atributos y relaciones a las clases. A medida que el análisis avanza, se identifican nuevos paquetes, clases y requisitos, que los ingenieros de componentes refinan y mantienen continuamente para ajustar el modelo.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdFgMvP4-8r_bKvGAvDcEYq6lYMxw-E6Q2xT4_sSOxOlytthbDW4_j0bg_cNFjMgSkcT2qJsKVFaHTpKrs2ZudIMOu_QAuq16ocihJMVKxBOMV9V2bPifQFf_OpYQBhOxEh9iTPEJGPf-vt-D0KeMgbg2E?key=VReuh94fGGpJZLGsXsGdUQ)

#### Actividad: Análisis de la Arquitectura

Su objetivo es esbozar el modelo y la arquitectura mediante la identificación de paquetes de análisis, clases del análisis evidentes y requisitos especiales comunes.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfnyd5sFSzrLS-m-eGk7PBsh6Giny1D1Tr6rD-CWLhx61nKzup78XjvjIuWTE__7IH5cLxOfMUjavBy-f0WPYQ4bOq9u6XUjObnfz1TyfBqKINtrtz6vMroir21LPTAhK8xvVTn26CWapB5-or9Dm_KbLI?key=VReuh94fGGpJZLGsXsGdUQ)

Identificación de paquetes del análisis:

- Los paquetes organizan el modelo en partes más manejables y pueden definirse al inicio o conforme evoluciona el modelo.
    
- Se identifican basándose en los requisitos funcionales y el dominio del problema. Una forma común es asignar casos de uso a un paquete, como:
    

- Soporte a un proceso de negocio.
    
- Soporte a un actor del sistema.
    
- Casos de uso relacionados por generalización o extensión.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcdRfOLPLiNMUiCPB3sdCNF7c0kKV6O-U5R-pbNHLrKyPxBHvmquDVgCBcrvBQf0er0e5pGr2M8kYSvBYSp6vuWXOkLY_7dI2DCtXTJm6aRa4KtLdkK-97WIuHjna0vgz5MPyUk3Nf-zDXTLZspNdo_-0Gr?key=VReuh94fGGpJZLGsXsGdUQ)
    

- Gestión de aspectos comunes: Cuando varios paquetes necesitan compartir clases, se extraen esas clases en un paquete propio o simplemente fuera de cualquier otro paquete, y después los otros paquetes serán dependientes de este paquete o clase más general. Estas suelen ser clases de entidad, de las cuales se puede hacer una traza hasta clases del dominio o clases de entidad del negocio.
    
- Identificación de paquetes de servicio: Estos paquetes se definen más adelante en el análisis, cuando los requisitos están claros. Cada paquete agrupa clases que contribuyen a un mismo servicio. Al identificar paquetes de servicio, debemos hacer lo siguiente:
    

- Identificar un paquete de servicio por cada servicio opcional. El paquete de servicio será una unidad de compra. Ejemplo:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfWZ2PI9F6hNTDi2Ne0pbaiNfd9hV-WbplARyM8wX2lEfB-XKUPqAqx2JfVnMorxDl2cy7LeT9JK3mpRuABebMB2KCVgrFZPEN6ceLVt-b0kGnuuU29FDMJMLwWGs4ibMapzqbZ9mlI7fkH2zRtqEED4Nvz?key=VReuh94fGGpJZLGsXsGdUQ)
    

Se describe el caso de uso opcional Enviar Aviso. Algunos vendedores quieren avisos automáticos cuando se dé una factura atrasada, mientras que otros prefieren que se les avise cuando haya una factura atrasada, y ellos mismos decidirán después si mandan un aviso.

Esta variabilidad se representa mediante dos paquetes de servicio opcionales y mutuamente exclusivos Avisos Automáticos se utiliza para los avisos automáticos, y Avisos Manuales notifica al vendedor, el cual decide si contacta con el comprador. 

Cuando un vendedor no quiere este servicio, no se entrega ninguno de los paquetes con el sistema.

- Identificar un paquete de servicio por cada servicio que podría hacerse opcional, incluso aunque todos los clientes siempre lo quieran. Debido a que los paquetes de servicio contienen clases relacionadas funcionalmente, obtendremos con ellos una estructura de paquetes que aísla la mayoría de los cambios en paquetes individuales. 
    

Una clase A y una clase B están relacionadas funcionalmente cuando:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfXfr3-UR9Le-PXPrRN_3I41qq35St-O75e6X3e6smTt2gBc9AqOjxVkbdbDswDdxvyYtHZaUnR-aw0ROVF89m3Dosw-Vg5gAeYd9wt2G7n_sHy-Jn-AroyWtlft5NuEQ2u1pEwryy_hS8X8nnO9sLxa3hr?key=VReuh94fGGpJZLGsXsGdUQ)

- Un cambio en A requerirá un cambio en B.
    
- La eliminación de A hace que B sea superflua.
    
- Los objetos de A interactúan intensamente con objetos de B, posiblemente a través de varios mensajes diferentes.
    

- Dependencias entre paquetes: Se definen dependencias si los paquetes están relacionados, el objetivo es conseguir paquetes que sean relativamente independientes y débilmente acoplados pero que posean cohesión interna alta. Esto es ideal, ya que facilita el mantenimiento y reduce las dependencias entre paquetes.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfs4S79JfATUkBY9V5t5aGm9t0q7LvzjIgfyBE0kUJVAzJLoH9RgDXdTFCtsZGx5h-1qYk021yIN3PBOeHmR5LQiGIlIm2JztJ0L9_tA5u6_I8hCfuCW_gO2V7CEuDvYY5VuQE73GGWluipmbxzyBJXJ7lI?key=VReuh94fGGpJZLGsXsGdUQ)
    

Identificación de clases de entidad obvias:

- Se proponen preliminarmente las clases de entidad más importantes (10 o 20) basadas en las clases del dominio o en las entidades del negocio que se identificaron en la etapa anterior. Es esencial no sobrecargarse con detalles en esta etapa, ya que la mayoría de clases surgirán al realizar casos de uso.
    

Identificación de requisitos especiales comunes:

- Estos surgen durante el análisis y es importante anotar para que sean tratados en las siguientes actividades (diseño e implementación). Estos deben ser identificados y documentados por el arquitecto para facilitar el trabajo posterior. Ejemplos:
    

- Persistencia.
    
- Distribución y concurrencia.
    
- Características de seguridad.
    
- Tolerancia a fallos.
    
- Gestión de transacciones.
    

#### Actividad: Analizar un caso de uso

Refinamiento de casos de uso usando clases de analisis![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXePaJ60vf7ZFBhnA6zA9vGYk8yGIZMv3DrlsudggYvIsYmom2ckHpB_ah-oSMdIh7H2UKEwH6yMmyKKQB9Sr9Tc4M1OmOX1ma14c24cbxweLQSBuJjfPMLUFJXtdkj3j63YgvVN3z7KKCXw4v61wk6fzP9P?key=VReuh94fGGpJZLGsXsGdUQ)

1 Identificacion clases de análisis

Aquellas clases que intervienen en la realizacion. Casi todo lo anterior (flujo de requisitos) muchas veces no esta del todo detallado

Normas generales para identificar las clases del análisis:

- Clases de entidad mediante el modelo de dominio y la descripción de CU. Hay casos donde la información es mejor tratarla como atributo.
    
- Clase de interfaz central por cada ACTOR humano. Interfaz de usuario. Es una refinación de la interfaz primitiva.
    
- Clase de interfaz primitiva por cada clase entidad, estas clases representan objetos lógicos con los que el actor interactúa durante la realización.
    
- Clase de interfaz por cada actor sistema externo (software o hardware), sería un medio de comunicación.
    
- Clase de control, tratamiento y coordinación de la realización. Cuando es muy simple el control, se lo manda todo a una clase interfaz(el actor se encarga de hacer el control), en situaciones complejas se usan clases de control.
    

Aparte se tiene el modelo de análisis, del cual se extraen clases también.

Se puede representar mediante un diagrama de clases

  

Descripción de interacciones entre objetos del análisis:

Objetivo: Describir cómo interactúan los objetos del análisis en un caso de uso mediante diagramas de colaboración.

- Diagramas de Colaboración:
    

- Representan instancias de actores y objetos del análisis.
    
- Se recomienda crear un diagrama por cada flujo o subflujo del caso de uso para mayor claridad.
    

- Creación del Diagrama:
    

- Comienza desde el inicio del flujo del caso de uso, avanzando paso a paso.
    
- Las interacciones entre objetos y actores son esenciales para la realización del caso de uso.
    

- Características de los Diagramas:
    

- El caso de uso se inicia con un mensaje de un actor a un objeto de interfaz.
    
- Cada clase del análisis debe tener al menos un objeto en el diagrama; de lo contrario, es superflua.
    
- Los mensajes reflejan el propósito del objeto que los envía, no operaciones específicas.
    
- Los enlaces representan asociaciones entre clases del análisis; deben ser evidentes en el diagrama de clases asociado.
    
- La secuencia de interacciones no es el objetivo principal; se debe priorizar las relaciones y requisitos.
    

- Relaciones entre Casos de Uso:
    

- El diagrama debe incluir todas las relaciones relevantes; por ejemplo, especializaciones de otros casos de uso.
    

- Complemento Textual:
    

- En casos complejos, es útil añadir descripciones textuales que se incluyan en el artefacto de flujo de sucesos-análisis del caso de uso.
    

Captura de Requisitos Especiales

Recoger requisitos no funcionales relevantes para la realización de un caso de uso que deben ser tratados en las fases de diseño e implementación.

  

  

  

  

  

#### Actividad: Analizar una clase![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfaYe7xGyEI2P6vuBcN-CyK_-KCmm53OJB-o7GUvhm8yIj13NRaHQv2K-B9JGER3Rn7nVkLUuDRUKRqBbyJVricMfhw6kfVB_R39BYDXyyOoMMBSiJ8OwguBefKS38lGBHG_64pmr4XUFyv2CNQPyqOoJc?key=VReuh94fGGpJZLGsXsGdUQ)

Objetivos: Identificar responsabilidades, atributos, relaciones y requisitos especiales.

Identificación de Responsabilidades:

- Combinar todos los roles que cumple la clase en diferentes realizaciones de casos de uso.
    
- Estudiar diagramas de clases e interacción para identificar en cuáles casos de uso participa la clase.
    
- Consultar el artefacto de flujo de sucesos - análisis para obtener requisitos textuales.
    
- Técnica de Recopilación:
    

- Extraer las responsabilidades de cada rol de manera secuencial.
    
- Añadir o modificar responsabilidades basadas en las realizaciones de casos de uso.
    

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdxQ1bscHWkvV3SD98s0aGNRiYESJwzXzUtQMIbI6Fx8Vl4hazxOI3U-gltc745FPMH_EOtVW_RzLL8UOU_0yjmTib7T0JE335TBuVCbb4HALjECrnapZKBrCDeL9c25U0ky-NM1iZ4Xj5snRxlxmfOm9Gn?key=VReuh94fGGpJZLGsXsGdUQ)  
  

Identificación de Atributos:

Un atributo especifica una propiedad de una clase de análisis y es fundamental para cumplir con las responsabilidades de dicha clase.

Normas Generales para Identificar Atributos:

- Nomenclatura: El nombre de un atributo debe ser claro y conciso, siguiendo el formato [1,2].
    
- Tipo Conceptual: El tipo de los atributos debe ser conceptual en el análisis, sin estar restringido por el entorno de implementación. Por ejemplo, "cantidad" es adecuado en análisis, mientras que en diseño podría ser "entero".
    
- Reutilización de Tipos: Al decidir el tipo de un atributo, se debe intentar reutilizar tipos ya existentes para mantener coherencia.
    
- Instancias Únicas: Una instancia de un atributo no puede ser compartida por varios objetos. Si se requiere, el atributo debe definirse en su propia clase.
    
- Claridad: Si los atributos de una clase hacen difícil su comprensión, se pueden separar en clases independientes.
    
- Clases de Entidad: Los atributos son evidentes en clases de entidad. Las trazas con clases del dominio o de negocio son útiles para identificar atributos.
    
- Clases de Interfaz: Los atributos en clases de interfaz que interactúan con actores humanos suelen ser elementos de información (ej. campos de texto). En clases de interfaz que interactúan con sistemas, representan propiedades de la comunicación.
    
- Clases de Control: Aunque son poco frecuentes, pueden tener atributos que representan valores acumulados o calculados durante la realización de un caso de uso.
    

- Atributos Formales: No siempre son necesarios; a veces, una explicación simple de una propiedad es suficiente y puede añadirse a la descripción de responsabilidades.
    

- Diagrama de Clases: Si una clase tiene muchos atributos o atributos complejos, se puede crear un diagrama de clases separado que muestre solo la sección de atributos.
    

Identificación de Asociaciones y Agregaciones:

Los objetos del análisis interactúan mediante enlaces en los diagramas de colaboración, que suelen representar instancias de asociaciones entre clases.

- Proceso de Identificación:
    

- Estudio de enlaces: Analizar los enlaces en los diagramas de colaboración para determinar las asociaciones necesarias.
    
- Identificar referencias y agregaciones entre objetos.
    
- Minimización de relaciones: Reducir el número de relaciones entre clases.
    
- Modelar sólo aquellas relaciones que son necesarias para satisfacer las demandas de las realizaciones de casos de uso.
    

- Enfoque en el Análisis: El análisis no debe centrarse en modelar rutas de búsqueda óptimas a través de asociaciones o agregaciones; esto se debe abordar en las fases de diseño e implementación.
    

- Definición de Asociaciones: El ingeniero de componentes define:
    

- Multiplicidad de las asociaciones
    
- Nombres de los roles
    
- Auto-asociaciones
    
- Clases de asociación
    
- Roles ordenados
    
- Roles cualificados
    
- Asociaciones n-arias
    

- Ejemplos de Uso de Agregaciones: Las agregaciones son apropiadas cuando los objetos representan:
    

- Contenidos Físicos: Ejemplo: Un coche que contiene al conductor y a los pasajeros.
    
- Composición: Un coche que consta de un motor y ruedas.
    
- Colecciones Conceptuales: Una familia que incluye un padre, una madre y los niños.
    

Identificación de Generalizaciones:

Las generalizaciones se utilizan para extraer comportamientos compartidos y comunes entre varias clases del análisis, simplificando el modelo y mejorando su comprensión.

- Deben mantener un nivel alto y conceptual: Mantener las generalizaciones en un nivel alto, evitando detalles específicos que puedan complicar el modelo.
    
- Facilitación de Comprensión: El objetivo principal es hacer el modelo de análisis más fácil de entender, resaltando similitudes entre clases.
    

Captura de Requisitos Especiales:

Este paso implica recoger todos los requisitos de una clase del análisis que se han identificado, pero que deben ser tratados en las fases de diseño e implementación, especialmente los requisitos no funcionales.

  

  

  

  

#### Actividad Analizar un paquete

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdoYTt_zAKM5EFqKr02VDf8wxedfQvE11D3FFp5CW01cSJ3E_OjDrdjWP8W2phM6lIYcCrVGdQVQKd3BAV5jsVrxNgau60YGo8IHZyIVMhWyrHVAFpcNEZJYDLipKInfOmZrWxZBZ9lfsfLgsh0-gwy9gkg?key=VReuh94fGGpJZLGsXsGdUQ)

Objetivos clave:

- Independencia de Otros Paquetes: Asegurar que el paquete sea lo más independiente posible de otros paquetes, lo que facilita su mantenimiento y reutilización. BAJO ACOPLAMIENTO.
    

- Cumplimiento de Objetivos: Verificar que el paquete cumple su propósito, ya sea implementando clases del dominio o satisfaciendo casos de uso específicos.
    

- Descripción de Dependencias: Documentar las dependencias del paquete para estimar el impacto de futuros cambios, lo que ayuda en la planificación y gestión de riesgos.
    

Normas Generales para el Análisis de Paquetes

- Definir relaciones entre paquetes
    
- Cohesión del Paquete: Elementos altamente cohesivos
    
- Limitación de Dependencias: bajo acoplamiento entre paquetes
    

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXealp_LY4FRxGDHHL33fddjhxb3xFNVMMLJxLds7a3ZkvBwFU-bxnIPyMyj2Oc3WXyNE-nYApqwkkwLlRCbaeLTAh60DHDEL0br40oKwncYlPOXuRR6C0qdZ2R-KmSS620FKqZq9C4A-lkzXq7GCjSzO3YA?key=VReuh94fGGpJZLGsXsGdUQ)

  

  

  

  

  

  

  

  

  

  

### Resumen del Análisis

El flujo de trabajo del análisis culmina en el modelo de análisis, que refina y estructura los requisitos. Incluye:

- Paquetes del Análisis: Aíslan cambios en procesos del negocio y casos de uso.
    
- Paquetes de Servicio: Aíslan cambios en servicios específicos, promoviendo la reutilización.
    
- Clases del Análisis: Definen responsabilidades y relaciones.
    

- Clases de Control: Coordinan la lógica del negocio.
    
- Clases de Entidad: Gestionan información persistente.
    
- Clases de Interfaz: Manejan interacciones de usuario.
    

- Realizaciones de Casos de Uso-Análisis: Refinan casos de uso y aislan cambios.
    
- Vista de la Arquitectura: Ayuda a identificar cambios arquitectónicos.
    

Influencia en el Diseño: El modelo de análisis influye en el diseño al:

- Relacionar paquetes de análisis con subsistemas de diseño.
    
- Guiar el diseño de clases, abordando requisitos especiales.
    
- Servir como base para especificaciones de casos de uso.
    
- Proveer una vista arquitectónica que asegura trazas relevantes entre modelos.
    

Este enfoque sistemático facilita un desarrollo de software coherente y estructurado.