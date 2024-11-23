## DISEÑO

En el diseño, modelamos el sistema y su arquitectura para cumplir con todos los requisitos, incluidos los no funcionales. La entrada esencial para este proceso es el modelo de análisis, que ofrece una comprensión detallada de los requisitos y establece una estructura que debemos conservar.

### Propósitos del Diseño

- Comprensión de Requisitos No Funcionales: Profundizar en aspectos como lenguajes de programación, componentes reutilizables, sistemas operativos y tecnologías de interfaz.
    
- Punto de Partida para Implementación: Capturar requisitos, subsistemas, interfaces y clases para facilitar la implementación.
    
- Descomposición de Tareas: Dividir la implementación en partes manejables para diferentes equipos, considerando la concurrencia.
    
- Captura de Interfaces: Identificar interfaces entre subsistemas temprano en el ciclo de vida del software para mejorar la arquitectura y la sincronización entre equipos.
    
- Visualización del Diseño: Utilizar notaciones comunes para reflexionar sobre el diseño.
    
- Abstracción de la Implementación: Asegurar que la implementación sea un refinamiento directo del diseño, permitiendo tecnologías como generación de código y ingeniería de ida y vuelta.
    

  
  
  
  
  
  
  
  
  
  
  
  

Comparación entre Modelo de Análisis y Diseño:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcrEmpKHvxsvoQOQeGseRLaGNFIUN0alihaPabt4uigG6Z2g1WlCIHELnnz1SVEfmIAlOTK13ZY2qUb9f3P7U5SqJ--dMHsgD3na2v-4BdwqgVFlKaK-x6lr97A0VPalA1o4ddYa8OoneiYmhD6aenDpgPd?key=VReuh94fGGpJZLGsXsGdUQ)

### TRABAJADORES Y ARTEFACTOS

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcqlkQr0eRocOd6VK5wu9GNnchPQP-wQggjbmXRPhrqEbMLw50dQ6LbxMOfkGBVnP1YVs8ki9p37wPeJ9Zg5FHfExtwP9c1XtGKiNBr4VBJ35FfOOLufRUEm_IstnfMAF_gp_oeK5t4f1r2GHzQopZS44Cp?key=VReuh94fGGpJZLGsXsGdUQ)  

### ARTEFACTOS

- ARTEFACTO: MODELO DE DISEÑO
    

El modelo de diseño es un modelo de objetos que describe la implementación física de los casos de uso, enfocándose en cómo los requisitos funcionales y no funcionales, así como otras restricciones del entorno de implementación, afectan al sistema. Este modelo actúa como una abstracción de la implementación y es fundamental para las actividades de implementación.

Estructura del Modelo de Diseño:

- Jerarquía: Representa el subsistema de nivel más alto y organiza el modelo en porciones manejables.
    
- Subsistemas y Clases de Diseño: Representan abstracciones directas que muestran una correspondencia sencilla entre el diseño y la implementación.
    

Realización de Casos de Uso:

Los casos de uso son implementados por las clases de diseño y sus objetos, lo que se denota a través de colaboraciones en el modelo.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXczsgxuFIHG_5I2wtbwMnzxnLA5HFarLEIW3Du0BwHulYODJZd3sz9k2eFwHF1HKH1vlLgV-JB6PxfOeFFLtOcgMd5ihW71BAbzcPT9D5KoCli9-AFnr0LXUgrmbKs_La-M65xEiQRF8oMw3BVdGJfdCaQl?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  

- ARTEFACTO: CLASE DE DISEÑO
    

Es una abstracción que refleja de manera directa una clase o construcción en la implementación del sistema. Esta abstracción se caracteriza por ser "sin costuras", lo que implica varias características clave:

Características de una Clase de Diseño:

- Lenguaje Consistente: El lenguaje para especificar la clase de diseño es el mismo que el del lenguaje de programación, usando su sintaxis para operaciones, parámetros, atributos, etc.
    
- Visibilidad de Atributos y Operaciones: Se especifica la visibilidad (público, protegido, privado) de manera clara, como en C++.
    
- Relaciones Directas: Las relaciones entre clases de diseño tienen un significado directo en la implementación, como la herencia y las asociaciones, que se corresponden con atributos en la implementación.
    
- Correspondencia de Métodos: Los métodos en la clase de diseño tienen una correspondencia directa con los métodos en la implementación, y se pueden especificar en lenguaje natural o pseudocódigo.
    
- Postergación de Requisitos: Se pueden postergar algunos requisitos para las actividades de implementación, indicando requisitos de implementación en la clase.
    
- Estereotipos Correspondientes: La clase de diseño se puede estereotipar según construcciones del lenguaje de programación (por ejemplo, "class module" en Visual Basic).
    
- Interfaces: Puede proporcionar interfaces si es apropiado en el lenguaje de programación.
    
- Activación de Clases: Puede implicar que los objetos mantengan su propio hilo de control y se ejecuten concurrentemente, aunque normalmente no son activas. Las clases activas deberían residir en su propio modelo de proceso en lugar de en el modelo de diseño.
    

Estas características permiten que las clases de diseño sirvan como un puente efectivo entre el diseño y la implementación, asegurando que las decisiones tomadas en la fase de diseño se traduzcan de manera efectiva en el código final.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfCFSRDc4xW0Ce2Ea3en0v91oo2puCboi-uGeA0evLEP_saGb32LhkrL2MdEfwFiK8-rNVg8jDxYkpIb4mMOCUOECkQNI_gP8Wm_1iRmLnngwD0gzEuDCNQC-9H2XZRGAD9BEydHEIQ8L5rPLlI14UJmes?key=VReuh94fGGpJZLGsXsGdUQ)

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfEeKvUv9FnQGLh64pC1YDbg47WsvNyiYflGxHCbbFgUZWPjjq8HIDYmRow5XEhV-zilxRJiR15xCVDz9hm9fwWR0nJMYPrAHVj3hN6NB3K31gWKDHbN2n70xmgKY6cEG5KNFR0ePcubZNRN9_VQiSTpNoo?key=VReuh94fGGpJZLGsXsGdUQ)

- ARTEFACTO: REALIZACIÓN DE CASO DE USO - DISEÑO![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXetvPyiczzN8lAeFgkB5s4vNFG4ziSLvPZqsC2j7Tiks8fSTVb9i5uk26N_mtwv6BtqVdubrv3yVmaUqpcnW6aLZUoUdMG9YM1ppYJ6UW52iReISSTyOc9YLMqgH66-Hv_3ckkmaIvQPP4zZ_G_7pECqbDX?key=VReuh94fGGpJZLGsXsGdUQ)
    

Es una colaboración en el modelo de diseño que describe cómo se realiza un caso de uso específico, utilizando clases de diseño y sus objetos. Este tipo de realización proporciona una traza directa a una realización de caso de uso-análisis en el modelo de análisis.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXftWqSVFLwUJ6h_RsTAyg6FlFGYkXYvfsjPj5OAIugeTS_yyaxLB3gPYBHrXUpYyV47wzzp47-glCuK45iUATH-cZpkpZWPI7oOzh9IGwDxiPV0PJBos627MtvWl-3LPzC6JRQGfLsMDkmhgZcAxA9gWlXq?key=VReuh94fGGpJZLGsXsGdUQ)

Cuando el modelo de análisis no se mantiene a lo largo del ciclo de vida del software, la dependencia de traza de una realización de caso de uso-diseño irá directamente hasta el caso de uso en el modelo de casos de uso.

Componentes de una Realización de Caso de Uso - Diseño:

- Diagramas de Clases: Los diagramas de clases conectados a una realización de caso de uso permiten coordinar requisitos que diferentes realizaciones imponen a una clase y sus objetos. Muestran las clases de diseño participantes y sus relaciones.
    
- Diagramas de Interacción: Los diagramas de secuencia son preferidos para representar las interacciones entre objetos, mostrando la transferencia de mensajes entre ellos. Esto permite identificar las interfaces de los subsistemas en fases tempranas del ciclo de vida del software. Representan el flujo o escenario de un caso de uso en términos de interacción entre objetos del diseño.
    
- Flujo de Sucesos - Diseñó: Este artefacto es una descripción textual que complementa los diagramas, explicando las interacciones sin detallar atributos u operaciones específicas, lo que facilita el mantenimiento. Explica cómo se lleva a cabo el caso de uso.
    
- Requisitos de Implementación: Son descripciones textuales que recogen requisitos no funcionales y otros que deben ser tratados en la fase de implementación.
    

  

- ARTEFACTO: SUBSISTEMA DE DISEÑO
    

Son una forma de organizar los artefactos del modelo de diseño en piezas más manejables. Un subsistema puede incluir clases de diseño, realizaciones de caso de uso, interfaces y otros subsistemas.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcj8rlGj1b6o9e8M1HFQ20NG3YUbACuUtJs3zlE2VKYo5qeCvf0FSUYTAToyNIfVeUYZ_VyCUIl0CuitFdaWnDvcvhUZVBYzeetPa-BELy-gH03XeLe8QvYCGMeJS8bncn1Dug3iG3UeZdtw-eR4m0GQNo?key=VReuh94fGGpJZLGsXsGdUQ)

Características de los Subsistemas de Diseño:

- Cohesión: Los contenidos de un subsistema deben estar fuertemente asociados.
    
- Acoplamiento: Las dependencias entre subsistemas deben ser mínimas.
    
- Separación de aspectos: Permiten que diferentes equipos desarrollen subsistemas de manera independiente.
    
- Trazas directas: Los subsistemas suelen tener trazas directas hacia paquetes y/o clases del análisis.
    
- Componentes de grano grueso: Representan componentes que proporcionan varios interfaces compuestos.
    
- Reutilización de software: Pueden encapsular productos de software reutilizados.
    
- Sistemas heredados: Pueden incluir sistemas heredados en el modelo de diseño.
    

Subsistemas de Servicio: Se utilizan en un nivel inferior de la jerarquía de subsistemas de diseño para preparar cambios en servicios individuales, aislando los cambios en los subsistemas de servicio.

- Identificación de Subsistemas de Servicio: Se basa en los paquetes de servicio del modelo de análisis, con una traza uno-a-uno entre ambos. Los subsistemas de servicio deben tratar más aspectos que sus correspondientes paquetes de servicio:
    

- Ofrecen servicios en términos de interfaces y operaciones.
    
- Contienen clases de diseño, enfrentándose a requisitos no funcionales y restricciones del entorno de implementación.
    
- Pueden dar lugar a componentes ejecutables o binarios en la implementación.
    

Organización de Artefactos: La organización de los artefactos del modelo de diseño utiliza subsistemas de diseño normales, pero se introduce un estereotipo «service subsystem» para diferenciar explícitamente los subsistemas que representan servicios, lo cual es crucial en sistemas grandes.

- ARTEFACTO: INTERFAZ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcrcBDaVukiDVEgwnl2IeUbzxE4KeSbuihRuEm6l1KpHQqs_N1kN6uBnsm7HWtxYn4cLMu1rXx2H-3CRWL2efVmdYAHFbZm6_tgMgtaDTRzhHONfIoExozChAhM-deVGIOqeeAJUwi50SsIyn9uq0R6quU?key=VReuh94fGGpJZLGsXsGdUQ)
    

Especifican las operaciones que ofrecen las clases y subsistemas del diseño. Son clave en el diseño de sistemas, asegurando flexibilidad y modularidad.

Las interfaces permiten que los clientes sean independientes de la implementación concreta, facilitando la sustitución de implementaciones sin cambios en los clientes.

- Definen interacciones entre subsistemas, relevantes para la arquitectura.
    
- Permiten diseñar interfaces estables desde etapas tempranas del desarrollo.
    
- Sirven como herramientas de sincronización entre equipos de desarrollo.
    

  
  
  

- ARTEFACTO: DESCRIPCIÓN DE LA ARQUITECTURA (MODELO DE DISEÑO)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe8iJRA55_Y1hWE6A-PlhYGq-fsuYRmvcDMPW771998uHTFA5hBR9hyw0Q3YfF1Y4--B4lQeC10Rel8i-hX4NVDqXE76iVp083sTtJrvObuCUBLisUwvDpwpmF3C4wePtSSTZ8Pb-Sri0faBCTeNzBQrG1H?key=VReuh94fGGpJZLGsXsGdUQ)
    

La descripción de la arquitectura presenta una vista del modelo de diseño, destacando los artefactos relevantes para la arquitectura.

- Descomposición en Subsistemas: Incluye subsistemas, sus interfaces y dependencias, formando la estructura fundamental del sistema.
    
- Clases del Diseño Fundamentales: Clases que tienen trazas con clases del análisis significativas, clases activas y clases generales que representan mecanismos de diseño genéricos.
    
- Realizaciones de Caso de Uso-Diseño: Describen funcionalidades críticas que deben desarrollarse pronto, implicando muchas clases del diseño y abarcando varios subsistemas.
    

Estos artefactos son esenciales para entender la arquitectura del sistema y su desarrollo a lo largo del ciclo de vida del software.

- ARTEFACTO: MODELO DE DESPLIEGUE
    

Describe la distribución física del sistema, mostrando cómo se distribuye la funcionalidad entre los nodos de cómputo.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeXAo88deLtCH8nOVCLea8vtsoPTpJbACyvbvVN-9uKaPFkOwUwuONyaLR1dMx7f6TlafbIdK0wU5dK9XEOqEFC-ru_DywrGe1JBbf1edbA3jEqmEHsGKZnrRDq2lZjt7K2xv_NotVjZ-8ASecVMbAbF3A?key=VReuh94fGGpJZLGsXsGdUQ)

- Nodos: Cada nodo representa un recurso de cómputo, como un procesador o dispositivo hardware.
    
- Relaciones: Los nodos tienen relaciones que representan medios de comunicación, como Internet o intranet.
    
- Configuraciones de Red: Puede describir diferentes configuraciones, incluidas pruebas y simulaciones.
    
- Funcionalidad: Los procesos de un nodo se definen por los componentes distribuidos sobre él.
    
- Correspondencia Arquitectónica: Representa la relación entre la arquitectura software y la del sistema (hardware).
    
- ARTEFACTO: DESCRIPCIÓN DE LA ARQUITECTURA (VISTA DEL MODELO DE DESPLIEGUE)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcYdNRLWipUD9npeOKM3fS50yyDcngI_9ORWdBjQTusjb_a0AWGzgWHjtbrTdwcbsZGko2yRcZ98QCVm8XseQU0mWbBYDI1Eo02BfK5bFr0ngBlI8Hc0OpVqFNSl846c1OGwN65pcuNkJX2WiJTgwerVS_5?key=VReuh94fGGpJZLGsXsGdUQ)
    

  
La descripción arquitectónica incluye todos los aspectos del modelo de despliegue, mostrando la correspondencia de los componentes sobre los nodos tal como se identificó durante la implementación.

Este modelo es fundamental para las actividades de diseño e implementación, ya que la distribución del sistema influye en su diseño.

  
  
  
  
  

### TRABAJADORES

- TRABAJADOR: ARQUITECTO
    

Es responsable de la integridad de los modelos de diseño y de despliegue, garantizando que sean correctos, consistentes y legibles. Para sistemas grandes y complejos, puede incluirse un trabajador adicional para asumir las responsabilidades del subsistema de más alto nivel del modelo de diseño.

Los modelos son correctos cuando realizan la funcionalidad descrita en el modelo de casos de uso y en los requisitos adicionales. El arquitecto también es responsable de la arquitectura de los modelos, asegurando la existencia de partes significativas en las vistas arquitectónicas.

Es importante notar que el arquitecto no se encarga del desarrollo y mantenimiento continuo de los artefactos del modelo de diseño; esa responsabilidad recae en los ingenieros de casos de uso y de componentes.

- TRABAJADOR: INGENIERO DE CASOS DE USO
    

Es responsable de la integridad de una o más realizaciones de casos de uso-diseño, garantizando que cumplen con los requisitos esperados. Cada realización debe reflejar correctamente el comportamiento de su correspondiente realización de caso de uso-análisis y el caso de uso del modelo de casos de uso.

Esto incluye hacer legibles y adecuadas todas las descripciones textuales y diagramas que describen la realización del caso de uso. Sin embargo, el ingeniero de casos de uso no es responsable de las clases, subsistemas, interfaces y relaciones de diseño utilizados en la realización del caso de uso; esa es responsabilidad del ingeniero de componentes.

- TRABAJADOR: INGENIERO DE COMPONENTES
    

Define y mantiene las operaciones, métodos, atributos, relaciones y requisitos de implementación de una o más clases del diseño, asegurando que cada clase cumple con los requisitos esperados según las realizaciones de caso de uso en las que participa.

Este ingeniero puede mantener la integridad de uno o más subsistemas, garantizando que sus contenidos y dependencias son correctos y que realizan correctamente las interfaces que ofrecen. Es común que el ingeniero de componentes responsable de un subsistema también sea responsable de los elementos del modelo que contiene, promoviendo un desarrollo uniforme y sin discontinuidades.

  

### Flujo de Trabajo de Diseño

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfn4kxzzU7an0t6JWIGi1oJkuVBEQKUZFbQ-C8ui1j0CiUHjm61cW7FM26wlDbUqzCywk5FbfpxqoIm-zLG5cqlgUK4I_94FiSG6dbvMy0EgK9i_D3G3Xg0DJYHW5A7MI4L_CfJkOFXJRF4oWSDOMaUYmxc?key=VReuh94fGGpJZLGsXsGdUQ)

- Los arquitectos crean los modelos de diseño y despliegue, definiendo nodos, subsistemas, interfaces y clases importantes.
    
- Los Ingenieros de Casos de Uso realizan cada caso de uso en términos de clases y subsistemas, estableciendo requisitos de comportamiento.
    
- Los Ingenieros de Componentes especifican e integran requisitos en las clases mediante operaciones, atributos y relaciones.
    
- Los desarrolladores identifican nuevos candidatos para subsistemas y clases, y los ingenieros de componentes los refinan.
    

  

#### Actividad: Diseño de la arquitectura![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf7CnS5iplAVdnsiktm5rruxS-imJcaHTa7dCEukKxDvbPvyMXvFxt1mAPTtoTiW4-5GbSD8gD0jH1lVGG7HIgHuprB4R2E_prFr-9ShBJEd7VNnIfhsjwJLjmMh2FF9idTZyIpFZqyQ3y9Lf4aWiMfPkFg?key=VReuh94fGGpJZLGsXsGdUQ)

El objetivo es esbozar los modelos de diseño y despliegue, identificando los siguientes elementos:

- Nodos y configuraciones de red.
    
- Subsistemas y sus interfaces.
    
- Clases del diseño significativas, como las clases activas.
    
- Mecanismos de diseño genéricos para requisitos no funcionales.
    

A lo largo de esta actividad, los arquitectos consideran posibilidades de reutilización, como partes de sistemas similares o productos de software generales.

Los subsistemas, interfaces y otros elementos resultantes se añadirán al modelo de diseño. Además, el arquitecto mantiene, refina y actualiza la descripción de la arquitectura y sus vistas arquitectónicas.

Identificación de nodos y configuraciones de red

Las configuraciones físicas de red influyen en la arquitectura del software, afectando las clases activas y la distribución de la funcionalidad. Un patrón común es el de tres capas:

- Clientes (interacciones de los usuarios).
    
- Funcionalidad de base de datos.
    
- Lógica del negocio o de la aplicación.
    

El patrón cliente/servidor es un caso especial donde la lógica de negocio se ubica en una de las otras capas.

Aspectos Clave de las Configuraciones de Red:

- Identificación de nodos necesarios y su capacidad (potencia de proceso y tamaño de memoria).
    
- Tipos de conexiones entre nodos y protocolos de comunicación a utilizar.
    
- Características de las conexiones y protocolos (ancho de banda, disponibilidad, calidad).
    
- Necesidad de redundancia, modos de fallo, migración de procesos y copias de seguridad.
    

Con este conocimiento, el arquitecto puede incorporar tecnologías como brokers de solicitudes de objetos y servicios de replicación de datos para facilitar la distribución del sistema.

Cada configuración de red, incluidas las de pruebas y simulación, debe mostrarse en un diagrama de despliegue separado.

Identificación de subsistemas y de sus interfaces

Los subsistemas organizan el modelo de diseño en piezas manejables. Pueden identificarse al inicio para dividir el trabajo de diseño o surgir a medida que el modelo evoluciona.

No todos los subsistemas se desarrollan internamente; algunos son productos reutilizados o recursos existentes en la empresa. Incluir estos subsistemas permite analizar alternativas de reutilización.

Identificación de Subsistemas de Aplicación

En este paso, se identifican los subsistemas en las capas específica y general de la aplicación. Si se realizó una descomposición adecuada en paquetes durante el análisis, se pueden utilizar estos paquetes para identificar subsistemas dentro del modelo de diseño.

Es crucial identificar subsistemas de servicio que mantengan la estructuración del sistema según los servicios que ofrecen. Esta identificación puede refinarse durante el diseño para abordar temas relacionados con la implementación y distribución del sistema.

Refinamiento de la Descomposición Inicial

Puede ser necesario refinar la descomposición inicial en subsistemas en los siguientes casos:

- Si una parte de un paquete de análisis se corresponde con un subsistema por sí misma, permitiendo su uso compartido por otros subsistemas.
    
- Si algunas partes del paquete se realizan mediante productos software reutilizados, que podrían asignarse a capas intermedias o subsistemas.
    
- Si los paquetes del análisis no representan una división del trabajo adecuada.
    
- Si los paquetes no incorporan un sistema heredado, que puede encapsularse mediante un subsistema independiente.
    
- Si los paquetes no están preparados para una distribución directa sobre los nodos, lo que puede requerir descomponer algunos subsistemas en otros más pequeños.
    

Identificación de Subsistemas Intermedios y de Software del Sistema

El software del sistema y la capa intermedia constituyen los cimientos de un sistema. La selección e integración de productos software son objetivos fundamentales durante las fases de inicio y elaboración.

Es importante mantener una adecuada libertad de acción al adquirir middleware y software del sistema, evitando depender totalmente de un producto o fabricante. Cada producto debe considerarse como un subsistema independiente con interfaces explícitas.

Definición de Dependencias entre Subsistemas

Las dependencias entre subsistemas deben definirse si sus contenidos tienen relaciones. La dirección de la dependencia debe coincidir con la dirección de la relación. Si se esbozan dependencias antes de conocer los contenidos, se deben considerar las dependencias entre los paquetes del análisis.

Identificación de Interfaces entre Subsistemas

Las interfaces proporcionadas por un subsistema definen operaciones accesibles "desde fuera". Para esbozar las interfaces, se deben considerar las dependencias identificadas previamente. Cuando un subsistema tiene una dependencia, es probable que deba proporcionar una interfaz.

Las interfaces de las capas intermedias y de software del sistema son más sencillas de identificar, ya que encapsulan productos software con interfaces predefinidas. Además de identificar las interfaces, es necesario definir las operaciones sobre ellas mediante el diseño de casos de uso.

Identificación de clases del diseño relevantes para la arquitectura

Suele ser práctico identificar las clases del diseño relevantes para la arquitectura pronto dentro del ciclo de vida del software, para comenzar el trabajo de diseño. Sin embargo, la mayoría de las clases se identificarán al diseñar las clases dentro de la actividad de diseño de clases, y se refinarán según los resultados obtenidos en la actividad de diseño de casos de uso.

Por este motivo, los desarrolladores deberían evitar identificar demasiadas clases en esta etapa o quedar atrapados en demasiados detalles. Un esbozo inicial de las clases significativas para la arquitectura es suficiente.

Identificación de Clases del Diseño a partir de Clases del Análisis

Podemos esbozar inicialmente algunas clases del diseño a partir de las clases del análisis significativas para la arquitectura que encontramos en el análisis. Además, podemos utilizar las relaciones entre esas clases del análisis para identificar un conjunto tentativo de relaciones entre las correspondientes clases del diseño.

  

Identificación de Clases Activas

Son clases que representan la ejecución de procesos concurrentes, estas clases toman la información de las clases de análisis o subsistemas (conjunto de clases). Ejemplos: UI, Ctrl, Procesamiento de pagos, etc.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfaWfc1-b4iBCt8Ikq9GmQFdm04qvwv5TZTrmtnwTaj0Xg-_BGSCEdghNjLxkNhB8C2NwxhOrSA8UiSAm5AOOmO6w75UpfjF-hYQKU554JR5-T0TT5nMYlfTVh8LjDxY3rZaVDONyQwWkKweM6pRQMhznLl?key=VReuh94fGGpJZLGsXsGdUQ)

El arquitecto identifica las clases activas necesarias en el sistema considerando los requisitos de concurrencia. Algunos aspectos a considerar incluyen:

- Los requisitos de rendimiento, tiempo de respuesta y disponibilidad que tienen los diferentes actores en su interacción con el sistema.
    
- La distribución del sistema sobre los nodos, donde los objetos activos deben soportar la distribución sobre varios nodos.
    
- Otros requisitos como arranque y terminación del sistema, progresión, evitación del interbloqueo, y capacidad de los nodos.
    

Cada clase activa se esboza considerando el ciclo de vida de sus objetos y cómo deberían comunicarse, sincronizarse y compartir información. Luego, se asignan los objetos activos a los nodos del modelo de despliegue, teniendo en cuenta la capacidad de los nodos y las características de las conexiones.

Esbozo de Clases Activas

Para esbozar las clases activas inicialmente, se pueden utilizar los resultados del análisis y el modelo de despliegue como entradas. Otra posibilidad es utilizar los subsistemas identificados previamente y asignar esos subsistemas a nodos particulares.

Cualquier clase activa que represente un proceso pesado es candidata para ser identificada como un componente ejecutable durante la implementación. La asignación de clases activas a los nodos es una entrada importante para la asignación de componentes (ejecutables) a los nodos durante la implementación.

Identificación de mecanismos genéricos de diseño

En este paso, estudiamos requisitos comunes, como los requisitos especiales identificados durante el análisis en las realizaciones de caso de uso y en las clases del análisis. Decidimos cómo tratarlos, teniendo en cuenta las tecnologías de diseño e implementación disponibles. El resultado es un conjunto de mecanismos genéricos de diseño que pueden manifestarse como clases, colaboraciones o incluso subsistemas.

Requisitos:

- Persistencia.
    
- Distribución transparente de objetos.
    
- Características de seguridad.
    
- Detección y recuperación de errores.
    
- Gestión de transacciones.
    

Colaboraciones Genéricas: El arquitecto también debería identificar colaboraciones genéricas que puedan servir como patrones utilizados por varias realizaciones de caso de uso dentro del modelo de diseño. Los patrones que son colaboraciones parametrizadas (con clases parametrizadas) también son genéricos y pueden utilizarse asociando clases concretas con los parámetros.

  
  
  
  
  
  
  
  
  
  
  
  
  
  

#### Actividad: Diseño de un Caso de Uso![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfWoiaKa2ka-i4AvhWPvCWuZaEenbWazo2FzusVVc3KxSeA1uzkv_E5xUS9A6NmZ1pq3-lZL4biM3MHpkB4EqZ8qaL5eMHfKzGhCNmU_bgSDdr75nGUn2UjuEzzFssKzNJyQ2IEhsk06Gbcvutq6w4Vp0ZG?key=VReuh94fGGpJZLGsXsGdUQ)

  

Los objetivos del diseño de un caso de uso son:

- Identificar las clases del diseño y/o los subsistemas cuyas instancias son necesarias para llevar a cabo el flujo de sucesos del caso de uso.
    
- Distribuir el comportamiento del caso de uso entre los objetos del diseño que interactúan y/o entre los subsistemas participantes.
    
- Definir los requisitos sobre las operaciones de las clases del diseño y/o sobre los subsistemas y sus interfaces.
    
- Capturar los requisitos de implementación del caso de uso.
    

  

1. Identificación de Clases del Diseño
    

Objetivo: Identificar las clases del diseño necesarias para un caso de uso.

Pasos:

- Estudiar clases de análisis vinculadas al caso de uso.
    
- Identificar requisitos especiales y las clases que los satisfacen.
    
- Asignar responsabilidades a ingenieros de componentes para el detalle de las clases
    
- Comunicar cualquier clase faltante a los arquitectos. Clases faltantes
    

  

2. Descripción de Interacciones entre Objetos![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpGUVDOz-yWKoEpA4V8YRTwOfC_EnLzJDSznI6tR8ptw7yTpOYFY81xuNLYPWjUXJs5KmokEEZwYfKasFwXrsNKZMbcnNahupbTupF6TYy3-cIKyyIZTs9bmc8qA3HK0w70XptVQoEjeU-Ao3e3hjTvP8?key=VReuh94fGGpJZLGsXsGdUQ)
    

Objetivo: Describir cómo interactúan los objetos del diseño.

Herramienta: Diagramas de secuencia que muestran actores, objetos y mensajes.

Pasos:

- Estudiar la realización del caso de uso-análisis.
    
- Crear diagramas de secuencia para flujos y subflujos.
    
- Identificar interacciones y asegurar que cada clase tenga un objeto en el diagrama.
    
- Documentar excepciones y caminos alternativos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdJTyllbSF5RNHWbnUd0LMf4LRPNqyLEQMi9qOTJQgKBfzII3RNb3osmuYWCNg-YljtNWZ9bUeKgnkhUIuKCkul6Wo7QKof3_0-HgmAA9--1PxwVJfZkpPtB75FpGTqcu4uAhuGezkJ9RVShsL5txU0zss?key=VReuh94fGGpJZLGsXsGdUQ)
    

Puede pasar que existan más caminos alternativos, e incluso el ingeniero de componentes puede detectar más caminos no descubiertos![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXev7X8EnYVSb5t90cw_fwl6dW0d6YwN-ZwCKQgFLWlMJ5V3g05SCq069FtwD52Uxq5d-t2Ox_r-UThD0oz0Tl5H1RMrQpV5JUlaZdBzmYF-Puht-VPJaFQ7acH_98UarJuFKb5Xvn4jGHdcK0Ib0-bwyZM?key=VReuh94fGGpJZLGsXsGdUQ)

  

3. Identificación de Subsistemas e Interfaces
    

Objetivo: Diseñar el caso de uso considerando subsistemas e interfaces.

Pasos:

- Identificar subsistemas necesarios analizando las clases y paquetes del análisis.
    
- Recoger subsistemas en un diagrama de clases que muestre dependencias e interfaces.
    
- Requisitos especiales mediante subsistemas![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdXTYnJh91Tg4-GxRLpa7JUeVCiEcxTyFyJrAHhV_9X-8dw90WuPFrHtJEjZqbjhLDUiygp0ySOdrDNpHGd5Nup5C5zTauC0IY0tJjKlnDdPTY9aUyfVhqasp8uOL9K1lVnh8rVoCJm1JnXAD1W6NCXsbWH?key=VReuh94fGGpJZLGsXsGdUQ)
    

  
  
  
  

4. Descripción de Interacciones entre Subsistemas
    

Objetivo: Describir interacciones a nivel de subsistema.

Herramienta: Diagramas de secuencia con líneas de vida representando subsistemas.

Pasos:

- Asegurar que cada subsistema tenga al menos una línea de vida en el diagrama.
    
- Cualificar mensajes con las interfaces correspondientes.
    

  

5. Captura de Requisitos de Implementación
    

Objetivo: Incluir en la realización del caso de uso requisitos identificados durante el diseño para la implementación del caso de uso, como los requisitos no funcionales.

  
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

#### Actividad: Diseño de una Clase![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc1Fun3HalY-4Eiqd5XOsH9GajfDnZAK_z9zmNulpnosMVC7fP8DTMSWkwPR2fm8QZnAiX-uVgtt1awR4wrqdLYfUpl5MaqmAHDssSN2llKTJdEHjDnFdfKirwdCYLPiJluqX_j5Vvn4AJikkKxhwpU_Iaf?key=VReuh94fGGpJZLGsXsGdUQ)

El propósito de diseñar una clase es crear una clase del diseño que cumpla su papel en las realizaciones de los casos de uso y los requisitos no funcionales que se aplican a estos. Esto incluye el mantenimiento del diseño de clases en sí mismo y los siguientes aspectos de éste:

- Sus operaciones.
    
- Sus atributos.
    
- Las relaciones en las que participa.
    
- Sus métodos (que realizan sus operaciones).
    
- Los estados impuestos.
    
- Sus dependencias con cualquier mecanismo de diseño genérico.
    
- Los requisitos relevantes a su implementación.
    
- La correcta realización de cualquier interfaz requerida
    

  

1. Esbozar la Clase del Diseño
    

Objetivo: Crear un esbozo de clases de diseño a partir de clases de análisis o interfaces.

Consideraciones:

Cuando tomamos una interfaz como entrada, suele ser simple y directo el asignar a una clase de diseño para que proporcione esa interfaz.

Cuando se dan como entrada una o varias clases del análisis, dependen del estereotipo:

- Clases de interfaz dependen de la tecnología utilizada (ej. Visual Basic).
    
- Clases de entidad deben reflejar información persistente, a menudo vinculadas a bases de datos.
    
- Clases de control deben considerar distribución, rendimiento y manejo de transacciones.
    

Resultado: Identificación de clases de diseño que deben trazarse a las clases de análisis correspondientes.

  

2. Identificar Operaciones (sintaxis de lenguaje de programación)
    

Objetivo: Definir operaciones necesarias para las clases de diseño.

Entradas Clave:

- Responsabilidades de clases de análisis relacionadas.
    
- Requisitos especiales de clases de análisis.
    
- Interfaces que la clase debe proporcionar.
    
- Realizaciones de casos de uso donde participa la clase.
    

Nota: Clases con comportamiento dependiente del estado se describen mejor con diagramas de estado.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSz_GtXp2U8OgSw9MPC458vBLDHOnOHon5TzXE0TuUctvmxk8cRvYQqU52Jmc4RyRvcY1-jSbzoXjSJt1MdXQFAjlb6gnJNrr0tw_Z3zxCWmnlr-mOTFy6Anrh6eVGTJjj6bGIFYbkFKv8gFGSM_amqzv3?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  

3. Identificar Atributos
    

Objetivo: Identificar y describir atributos de la clase de diseño.

Normas Generales:

- Considerar atributos de clases de análisis relacionadas.
    
- Respetar restricciones del lenguaje de programación.
    
- Reutilizar atributos existentes cuando sea posible.
    
- Evitar compartir instancias de atributos entre objetos.
    
- Simplificar atributos complejos en clases independientes si es necesario.
    

  

4. Identificar Asociaciones y Agregaciones
    

Objetivo: Definir interacciones entre objetos mediante asociaciones y agregaciones. Estas asociaciones luego se ven en la realización de caso de uso

Directrices:

- Estudiar relaciones de clases de análisis que puedan requerir asociaciones en el diseño.
    
- Refinar multiplicidad, nombres de rol y navegabilidad de asociaciones. En base al lenguaje elegido
    
- Minimizar el número de relaciones innecesarias.
    

  

5. Identificar Generalizaciones
    

Objetivo: Usar generalizaciones según la semántica del lenguaje de programación.

Alternativa: Usar asociaciones o agregaciones si no se admite herencia.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUOfRK7vmi56AGMzNz9Ye5GkGHjuX4VEEVm18lFWIhDkyIMX32-Lw1-cAHW0UeqZfNq3BpWFXWsTS_UnxyQ39hkvh6UAQw4mp2iw9BuwMp8xbDk0zRLZaquIz3vxusd7gKxi1BmF9dS3lhGCB9IRWCc-0?key=VReuh94fGGpJZLGsXsGdUQ)

6. Describir Métodos
    

Objetivo: Especificar cómo se realizarán las operaciones.

Nota: Los métodos suelen ser creados durante la implementación, pero pueden especificarse en herramientas de diseño si se soporta generación de código.

  

7. Describir Estados
    

Objetivo: Utilizar diagramas de estado para objetos cuyo comportamiento depende de su estado.

Resultado: Diagramas de estado como entrada para la implementación de la clase.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXepk0cCOhDlG0zTrFj0SWvVNPYIgamduCiRODB2KsemubDX1ZPgsMRVsuwmN29jB1s0x-WG-4ntKUXD0FJsyKrVm_x4YOlIYQ0y-9iYLTmF8s6unRqBTaXjZxlGy4eU2qvO8PoRlr-qrOOpRpr-1JudiM9B?key=VReuh94fGGpJZLGsXsGdUQ)

  

8. Tratar Requisitos Especiales
    

Objetivo: Abordar requisitos no considerados previamente, incluyendo requisitos no funcionales.

Consideraciones:

- Estudiar requisitos en realizaciones de casos de uso.
    
- Utilizar mecanismos de diseño recomendados por el arquitecto.
    
- Posponer el tratamiento de algunos requisitos hasta la implementación si es necesario.
    

#### Actividad: Diseño de un Subsistema

Los objetivos del diseño de un subsistema son (véase la Figura 9.44):

- Garantizar que el subsistema es tan independiente como sea posible de otros subsistemas y/o de sus interfaces.
    
- Garantizar que el subsistema proporciona las interfaces correctas.
    
- Garantizar que el subsistema cumple su propósito de ofrecer una realización correcta de las operaciones tal y como se definen en las interfaces que proporciona.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXevRAxTp2JVf-1stnbwKqT3gHuohzcK2RexddFlPRRNkxm-4lRuE3ldLJAbEw-ZVPUj9XG4tGC7QF3JJNe7UiXkonszBCiX6vIIjcjP5NS8faeih0bKCBJ_HpZdhIMfDMxHXMGeeg0E9zpJRfpLqjrl-MI9?key=VReuh94fGGpJZLGsXsGdUQ)
    

  
  

1. Mantenimiento de las Dependencias entre Subsistemas
    

Objetivo: Definir y mantener adecuadamente las dependencias entre subsistemas.

Consideraciones:

- Las dependencias deben establecerse en función de la asociación de elementos entre subsistemas.
    
- Si un subsistema proporciona interfaces, las dependencias deben declararse hacia esas interfaces, no hacia el subsistema en sí.
    
- Preferir la dependencia de interfaces, ya que permite mayor flexibilidad al cambiar subsistemas sin afectar la interfaz.
    
- Minimizar las dependencias entre subsistemas y/o interfaces, reubicando clases que sean excesivamente dependientes.
    

  

2. Mantenimiento de Interfaces Proporcionadas por el Subsistema
    

Objetivo: Asegurar que las operaciones de las interfaces de un subsistema cumplan con todos los roles en diferentes realizaciones de casos de uso.

Refinamiento:

- Los ingenieros de componentes pueden necesitar refinar las interfaces a medida que el modelo de diseño evoluciona.
    
- Las mismas interfaces pueden ser utilizadas en varias realizaciones de casos de uso, aumentando así los requisitos sobre ellas.
    

Técnica: El mantenimiento de interfaces es similar al de las clases de diseño y sus operaciones.

  

3. Mantenimiento de los Contenidos de los Subsistemas
    

Objetivo: Asegurar que un subsistema cumpla correctamente con las operaciones descritas por sus interfaces.

Aspectos Generales:

- Por cada interfaz que proporciona un subsistema, debe haber clases de diseño u otros subsistemas que también ofrezcan esa interfaz.
    
- Para clarificar cómo se realizan las interfaces o casos de uso dentro de un subsistema, se pueden crear colaboraciones que justifiquen los elementos contenidos en él.
    

  

### Resumen del Diseño

El diseño de un sistema culmina en un modelo que preserva la estructura establecida por el modelo de análisis, sirviendo como guía para la implementación. Este modelo de diseño comprende varios elementos clave:

1. Subsistemas del Diseño
    

Elementos: Incluye subsistemas de diseño, subsistemas de servicio, sus dependencias, interfaces y contenidos.

Origen: Los subsistemas se derivan de los paquetes del análisis, y las dependencias se basan en las del análisis.

Interfaces: Se generan a partir de las clases del análisis.

  

2. Clases del Diseño
    

Componentes: Incluye clases activas, operaciones, atributos y requisitos de implementación.

Derivación: Las clases del diseño se obtienen de las clases del análisis relevantes para la arquitectura.

  

3. Realizaciones de Caso de Uso-Diseño
    

Descripción: Detallan cómo se diseñan los casos de uso mediante colaboraciones en el modelo de diseño.

Especificaciones: Se basan en las realizaciones de caso de uso-análisis.

  

4. Vista Arquitectónica
    

Elementos Significativos: Identificación de elementos relevantes para la arquitectura del modelo de diseño, basados en el modelo de análisis.

  

5. Modelo de Despliegue
    

Descripción: Detalla las configuraciones de red para la implementación del sistema.

Componentes: Incluye nodos, sus características y conexiones, así como la correspondencia inicial de clases activas sobre los nodos.