
### QUE ES?

Es el proceso de averiguar lo que se debe construir. De hecho, es tan difícil que todavía no es poco común para los equipos de proyecto el comenzar a escribir código (lo cual es bastante fácil) antes de que hayan firmado simplemente lo que se supone que debe hacer el código (lo cual es difícil de determinar).

Objeto: Guiar el desarrollo a un sistema correcto.

Se puede basar en el modelo de negocios o dominio. (Modelo de negocios es lo que quiere el cliente (actor de negocio) y modelo de dominio es que se va a almacenar desde el punto de vista del sistema)

Modelo de negocios = actividades de negocio

Usuarios:

- Visión incompleta de sus necesidades.
    
- No comprenden el alcance del sistema hasta el final (retrasos).
  
### Visión general de la captura de requisitos

Cada proyecto de software es diferente. Esta singularidad proviene de las diferencias en el tipo de sistema, en el cliente, en la organización de desarrollo, en la tecnología, etc. De igual forma, hay diferentes puntos de partida para la captura de requisitos.

- En algunas ocasiones, comenzamos haciendo un modelo del negocio, o comenzamos con un modelo del negocio que ya está en desarrollo por parte de alguna otra empresa.
    
- Y en otros casos, el cliente incluso puede haber ya desarrollado una especificación de requisitos completa y detallada que no esté basada en un modelo de objetos, a partir de la cual podemos comenzar y negociar los cambios.
    

El objetivo del modelado del dominio es comprender y describir las clases más importantes dentro del contexto del sistema. Los dominios de tamaño moderado normalmente requieren entre I O y 50 de esas clases. Los dominios más grandes pueden requerir muchas más. Los restantes cientos de clases candidatas que los analistas pueden extraer del dominio se guardan como definiciones en un glosario de términos: de otra manera, el modelo del dominio se haría demasiado grande y requeriría más esfuerzo del necesario para esta parte del proceso.

El glosario y el modelo del dominio ayudan a los usuarios, clientes, desarrolladores y otros interesados a utilizar un vocabulario común.

### Flujo de Trabajo de la Captura de Requisitos![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcHYQiSUoKQ8iPc6mNw5fPJKhENud1yiyWUJdS6xwlaId-dkfROofJSxTXyRplz5XA8wmFa59FFODYjUck-H_o_sFENM1ClbPmE-QyLYoE2PiyNZDa5FeLuoHfEl-xMTDAQy4AKgCvex44ClhIORC6PLfOe?key=VReuh94fGGpJZLGsXsGdUQ)

1. Listar los requisitos candidatos.
    

La lista de características deseadas del sistema constituye los requisitos candidatos. Fundamentalmente para planear.

De cada característica se registra:

- Nombre corto.
    
- Descripción.
    
- Estado (propuesto, aprobado, incluido o validado).
    
- Coste estimado de implementación (en términos de tipos de recursos y horas-hombre).
    
- Prioridad (crítico, importante o secundario).
    
- Nivel de riesgo asociado a la implementación de la característica (crítico, significativo u ordinario).
    

Relaciones de traza con caso de uso

Es bajar a papel lo que se espera del sistema. Escuchar al cliente y anotar frases. Hacer preguntas para especificar bien lo que nos piden. Nombres cortos de características junto con una breve descripción. 

Hablar en términos muy resumidos y tratar de planificar en líneas generales.

2. Comprender el contexto del sistema (MÁS IMPORTANTE)
    

Modelo de Dominio:

Comprender, describir y capturar las clases más importantes de objetos en el contexto del sistema.

Cosas que existen o eventos que suceden en el entorno del sistema

Tres formas típica:

- Objetos del negocio que representan cosas que se manipulan en el negocio, como pedidos, cuentas, contratos, etc.
    
- Objetos del mundo real y conceptos de los que el sistema debe hacer seguimiento como aviación enemiga, misiles, trayectorias, etc.
    
- Sucesos que ocurrirán o han ocurrido, como llegada de un avión, su salida, hora de la comida, etc.
    

El MD se representa por diagramas de clases.

Permite usar un vocabulario común.

Modelo de dominio = Modelo de clases conceptuales 

Modelo del Negocio:

En resumen, procesos del negocio. Sistema desde la perspectiva de uso, ofrece valor

- Una entidad del negocio representa algo que los trabajadores toman, manipulan, inspeccionan, producen o utilizan en un negocio.
    
- Una unidad de trabajo es un conjunto de esas entidades que conforman un todo reconocible para el usuario final.
    
- La técnica de modelado de negocio identifica entidades y trabajadores que participan en la realización de los casos de uso del negocio.
    
- Los trabajadores identificados en el modelo de negocio se utilizan como punto de partida para derivar un primer conjunto de actores y casos de uso del sistema.
    

Un modelo de objetos del negocio es un modelo interno a un negocio. Describe cómo cada caso de uso de negocio es llevado a cabo por parte de un conjunto de trabajadores que utilizan un conjunto de entidades del negocio y de unidades de trabajo. 

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKtS3C_7sRiudv1QB633uvFPFulcFxz4bLERFB_riVX6NcMn4tRoAWRaDccNhymucdcHLiiYB3ZDbN1zFYqIOQrhRA83BVuXUMyUBQZ-OAYw-fcG3PvgHZsRvwFJYvKv9CKk8NxxIXB7qptoulhkTj9m03?key=VReuh94fGGpJZLGsXsGdUQ)

Se puede recurrir a distintos enfoques: modelo de dominio, modelo de negocio o ninguna de las dos. Idealmente se debe utilizar alguna y reflejar el diagrama de clases.

Incluye modelo de negocio y modelo de objetos del negocio.

¿Cuáles son los diagramas del modelo de negocio? Diagrama de interacción y diagrama de actividades.

3. Capturar requisitos funcionales
    

Cosas que hace el sistema. De valor

Identificar requisitos de sistema a través de casos de uso.

Capturar los requisitos funcionales y no funcionales que son específicos de los casos de uso individuales.

Búsqueda de CU a partir de un Modelo del Negocio

- Se identifica un actor por cada trabajador y por cada actor del negocio que vaya a ser usuario del sistema.
    
- Por cada rol de un trabajador / actor del negocio, asignamos un CU candidato.
    

  

  

4. Capturar requisitos no funcionales
    

Los requisitos no funcionales especifican las propiedades del sistema, como:

- Requisitos de interfaz: formatos, tiempos, u otros factores de relevancia en esa interacción.
    
- Requisitos físicos: material, forma, tamaño o peso.
    
- Restricciones de implementación: Las restricciones ambientales y de implementación,
    
- Restricciones de diseño: El rendimiento, Las dependencias de la plataforma, La capacidad de mantenimiento, La extensibilidad y La confiabilidad.
    

Algunos requisitos no funcionales son más genéricos y no se pueden conectar a un caso de uso particular o a una clase particular del mundo real. Lista de requisitos suplementarios.

### CAPTURA DE REQUISITOS COMO CASOS DE USO

- Forma apropiada de crear un modelo de sistemas.
    
- Los requisitos funcionales se estructuran naturalmente como casos de uso.
    
- Los casos de uso ofrecen una forma sistemática e intuitiva de capturar los requisitos funcionales.
    
- Con especial atención al valor agregado a cada usuario individual o a cada sistema externo.
    
- Obligan a pensar en términos de quiénes son los usuarios y que necesidades comerciales o de misión se pueden satisfacer a través de ellos.
    

TRABAJADORES Y ARTEFACTOS![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXehLPxHf-RuKLPW-OjjN2wNif1lYEkImpPUaR0jZrQ52Z-DJa6fHFQKVpgDbklo-UAHmNJO5uW6rW5ub7e96aVUVxn4f2dhdUOZ_XBRM-zRxSSIvDe3w1pZ8YxARqglaW_vzTnRSZpa_0HpeVHTMqnvdxSo?key=VReuh94fGGpJZLGsXsGdUQ)

  

ARTEFACTOS

![Imagen que contiene Diagrama Descripción generada automáticamente](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZhxKakRt-LVhASW78zDLys3elvsw_h-qqKMb1r609iFL5W_XfJ6-kmRsqHfUqDwPONnyakJPEYG3RZQi5Vhqliz2nTbN5TOqFJgAXC88Xm_7DpFPhm6w_gkBAB4TV_me1YesxHTJiIe3qCmkuLisTuvUR?key=VReuh94fGGpJZLGsXsGdUQ)

- Modelo de Casos de Uso: Es un modelo del sistema que contiene: paquetes (para más entendible o subsistemas), actores, casos de uso y sus relaciones. La totalidad de los casos de uso constituyen el modelo.
    
- Actor: Representa un tipo de usuario externo al sistema. Se corresponden con trabajadores o actores del negocio. Un actor juega un papel por cada caso de uso con el que colabora.
    
- Caso de Uso: Son fragmentos de funcionalidad que el sistema ofrece para aportar un resultado de valor para sus actores. Una instancia de caso de uso es la realización (o ejecución) de un caso de uso. Pueden tener atributos a nivel instancia que representan los valores que una instancia de un caso de uso utiliza y manipula durante la ejecución de su caso de uso. Estos valores son locales a la instancia del caso de uso, es decir, no pueden ser utilizados por otras instancias del caso de uso. Por ejemplo, puede considerarse que el caso de uso Sacar Dinero posee atributos como la contraseña, la cuenta, y la cantidad a retirar.
    
- Descripción de la Arquitectura (vista del modelo de casos de uso): Representa los CU significativos para la arquitectura. CU críticos.
    
- Glosario: Para definir términos comunes importantes que los analistas utilizan para describir el sistema. También se pueden usar los modelos de negocio y dominio.
    
- Prototipo de interfaz de usuario: Ayudan a comprender y especificar las interacciones entre actores humanos y el sistema durante la captura de requisitos. BOCETO VISUAL
    

TRABAJADORES

- Analista de Sistemas: Es responsable de mantener la consistencia inter-caso de uso. Encontrar funcionalidad, pero no especificarla
    

- Responsable de:
    

- Modelo de casos de uso.
    
- Actores que contiene.
    
- Glosario.
    

- Especificador de Casos de Uso: Asistencia al analista de sistema en la descripción detallada de cada caso de uso. Se para en cada CU en particular para detallarlo.
    

- Responsable de:
    

- Caso de uso.
    

- Diseñador de Interfaz de Usuario: Realiza bocetos, no la implementación. 
    

- Responsable de:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcFBdax1L1mwm83K9lq6eGPVTRLH6tUD1F-3NYTN2r6ePpZnPeZx7zFxq0oaALB2aVav_mW9FrtmH8MPFDp3PRXVXFp9TBojFtRJBbuIn1awvka8ojdSUEV3dW65SYRqOA1LDIPLJ8i9aejC16e6AWY-7o?key=VReuh94fGGpJZLGsXsGdUQ)
    

- Prototipo de interfaz de usuario.
    

- Arquitecto: Arquitecto prioriza CU.
    

- Responsable de:
    

- Descripción de la arquitectura (vista del modelo de casos de uso).
    

  

### FLUJO DE TRABAJO - ACTIVIDADES![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeOl0hjp7P_Sgn9Q41xxJAxihBEwznyu2PwW1H-0nzGyywa8tsIy8K4X7isEW_HJChTM-sLVY1PqINzcfSfwPHkDXy4dFiYO4DqZyY_30KQPwBam0OfuNYfAxDPYZMRfr3cTd0ZFwM6sz3bliBSA9_Co-fy?key=VReuh94fGGpJZLGsXsGdUQ)

  

#### Actividad: Buscar actores y casos de uso![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdHt_NyrAXxgIvf-zHBQA7-wle1cPOzvMndSv5HbaV0BQQbrzGbgn9sRVMPrpKHKISKOhSFEeyI_oZayD3sAqX34p93frLzXnDN0BvdjnSsZ8XqKjaeBBdMMkuT5390wuYT1pxKQTalD_CiGUhiTZhGxKlX?key=VReuh94fGGpJZLGsXsGdUQ)

Identificamos los actores y los casos de uso para: 

- Delimitar el sistema de su entorno.
    
- Esbozar quién y qué (actores) interactuarán con el sistema, y qué funcionalidad (casos de uso) se espera del sistema. 
    
- Capturar y definir un glosario de términos comunes esenciales para la creación de descripciones detalladas de las funcionalidades del sistema (es decir, de los casos de uso).
    

PASOS PARA ENCONTRAR ACTORES Y CU

- Encontrar los actores.
    

- Mediante los modelos
    
- Con el cliente
    

- Encontrar los casos de uso.
    

- Modelo de negocio
    
- Por actor
    
- Mediante reunión con el cliente
    
- Seguir criterios útiles:
    

- Resultado de valor: Cada ejecución satisfactoria de un caso de uso debe proporcionar algún valor al actor para alcanzar su objetivo. Esto ayuda a evitar encontrar CU demasiado pequeños.
    
- Actores concretos: Los CU proporcionan valores a usuarios individuales, evitando que los CU se hagan demasiado grandes.
    

- Describir brevemente cada caso de uso.
    

- Se explica un poco nomas, secuencia de pasos general.
    
- Con algunas frases que resumen las acciones y con una descripción paso a paso de lo que el sistema necesita hacer cuando interactúa con sus actores.
    
- También necesitamos ver el cuadro completo. Necesitamos explicar cómo están relacionados entre sí los casos de uso y los actores y cómo juntos constituyen el modelo de casos de uso.
    

- Describir el modelo de casos de uso completo(brevemente) (este paso también incluye la preparación de un glosario de términos).
    

- Prepararemos diagramas y descripciones para explicar el modelo de casos de uso en su totalidad, especialmente cómo se relacionan los casos de uso entre sí y con los actores. 
    
- No hay una regla estricta sobre lo que se debe incluir en el diagrama. De hecho, elegimos el conjunto de diagramas que describen más claramente el sistema. 
    
- La salida de este paso es la descripción breve del modelo de caso de uso.
    

  

  

  

  

  

  

#### Actividad: Priorizar casos de uso![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdv-0iYeJbswhpsiW6NkebGwZcfYpnJXR-w_0OIRBhgcyc26X1SiXxQ-dKiqbt3mK8zhn55SMofUtJfsJDqHIkUwRW37WC26FibW6KI1TAnyz2lnak1wW8zY40i9dowafcQzlZugYsuiwOOjADE-DyKRMbb?key=VReuh94fGGpJZLGsXsGdUQ)

El objetivo es priorizar los casos de uso para determinar cuáles deben desarrollarse en las primeras iteraciones y cuáles pueden postergarse.

Los resultados se recogen en la vista de la arquitectura del modelo de casos de uso, la cual es revisada con el jefe de proyecto. La vista sirve como entrada para planificar el desarrollo en cada iteración.

La vista (descripción de la arquitectura) debe resaltar los casos de uso relevantes desde el punto de vista de la arquitectura.

#### Actividad: Detallar un caso de uso![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXepG3IxC0RUe48QgcPfO2Wtj9L2k9MIXdLZm-wHVldCN_LFz_TT78d0bGYGqCeVDgLErq6iHQAvbJopbTPeIg-5opBlcyLzNis08IgVK7bhEbLUSZ1VWI2JbL_2yx9d7AERDSbOKYOpl0pZM65_6wafzHST?key=VReuh94fGGpJZLGsXsGdUQ)

Su objetivo es detallar cada caso de uso describiendo su flujo de sucesos, cómo comienza, termina y cómo interactúa con los actores.

El especificador de casos de uso debe trabajar en estrecha colaboración con los usuarios reales, entrevistándolos, discutiendo propuestas y revisando las descripciones.

Se obtiene como resultado una descripción detallada del caso de uso en texto y diagramas.

A partir del modelo y los diagramas de casos de uso, se debe especificar cada caso en detalle, describiendo paso a paso las acciones (entradas, salidas y flujo de eventos).

Estructurar la descripción de CU  
Pensando como máquina de estado, secuencia de acciones o estados en un CU.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdRM3_mVKXDOLO6TyxYXvN30NVqXJ0k6FP7c40fgD8I2FTB14nVCh7CAnZmUQDucgEkfvh_7JEjtCoRNYrvJv6WRTRrYjEqWxMcLrnggPRs1OQtNJpZ2opHQnTO2Uc5QozN6Ed319V9a23wiXplsgB8Z77B?key=VReuh94fGGpJZLGsXsGdUQ)

¿Qué debe incluir la descripción?

Para una descripción completa de un caso de uso, se deben incluir los siguientes elementos:

1. Precondición: Definir el estado inicial antes de que comience el caso de uso.
    
2. Inicio: Especificar cómo y cuándo comienza, es decir, la primera acción a ejecutar.
    
3. Secuencia: Ordenar las acciones de forma numerada, indicando el orden requerido si lo hay.
    
4. Finalización: Describir cómo y cuándo termina el caso de uso, junto con las postcondiciones (estados finales).
    
5. Caminos no permitidos: Incluir rutas de ejecución que no están permitidas (ej. acciones imposibles para el usuario).
    
6. Caminos alternativos: Describir las rutas alternativas dentro del caso de uso, indicando si solo se ejecutan bajo ciertas condiciones.
    
7. Interacción del sistema con los actores: Explicar cómo el sistema interactúa con los actores y los cambios que estas acciones producen.
    
8. Uso de objetos, valores y recursos del sistema: Detallar cómo el sistema utiliza sus recursos y asigna valores (ej. transferencias de dinero, uso de facturas, etc.).
    
9. Acciones del sistema: Especificar claramente las acciones que realiza el sistema, diferenciándose de las acciones de los actores. Esto asegura que la descripción sea lo suficientemente precisa para usarla como especificación del sistema.
    

Por otro lado estan requisitos no funcionales asociados a cada CU particular

FORMALIZACIÓN DE DESCRIPCIÓN

En caso de tener una descripción demasiado compleja, en lugar de un diagrama de máquinas de estados, se puede optar por las siguientes opciones:

- Diagramas de estados de UML para describir los estados de los casos de uso y las transiciones entre esos estados.
    
- Diagramas de actividad para describir las transiciones entre estados con más detalle como secuencias de acciones.
    
- Diagramas de interacción para describir cómo interactúa una instancia de caso de uso con la instancia de un actor.
    

  

#### Actividad: Prototipar interfaz de usuario![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf2Cu49ecSDwcLBJoXQmXRXRtTBvXhsGX88-b0E4R64HxhNGVnwHR8SQDhO6KtE4aauvALVpmHUK86Wm2NTpCD60krtIeJGVkkM48fsp-5xABycw7xR_cA6Z2QrVvFhUa5Z16oLVn2p0fhtVMoX60F5iW0?key=VReuh94fGGpJZLGsXsGdUQ)

Su objetivo es construir un prototipo de interfaz de usuario que permita a los usuarios ejecutar los casos de uso de manera eficiente.

Se parte de la base de que el analista de sistemas ya ha desarrollado un modelo de casos de uso que define los usuarios y sus necesidades. Además se tiene la descripción completa de cada CU.

Proceso:

- Diseñar la interfaz de usuario basándose en los casos de uso, comenzando con un diseño lógico que identifique los requisitos de la interfaz para cada actor.
    
- Luego, crear el diseño físico y desarrollar prototipos que ilustran cómo los usuarios interactúan con el sistema.
    

Se obtiene como resultado un conjunto de esquemas y prototipos que representan la apariencia de la interfaz para los actores más importantes.

Puntos clave para crear el diseño lógico de una interfaz de usuario:

El diseñador debe identificar los elementos de la interfaz (como íconos, listas u objetos) que los actores utilizarán para interactuar con los atributos de los casos de uso (usualmente están en el glosario).

Para cada actor, se debe revisar cada caso de uso que este pueda acceder, y determinar los elementos de interfaz necesarios para habilitar sus acciones.

Flexibilidad: Un mismo elemento de interfaz puede desempeñar distintos roles en diferentes casos de uso, por lo que debe diseñarse con flexibilidad.

Preguntas clave para cada actor:

- ¿Qué elementos de interfaz necesita para el caso de uso?
    
- ¿Cómo se relacionan entre ellos?
    
- ¿Cómo se utilizan en los diferentes casos de uso?
    
- ¿Cuál debería ser su apariencia?
    
- ¿Cómo deberían manipularse?
    

Puntos clave sobre la creación de un diseño y prototipo físico de la interfaz de usuario:\

- Notas adhesivas: Técnica para representar los elementos de la interfaz de usuario.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdK3mULFdpwOX_UKmiBpMoHij-QRDtCGJLGHLL9u72BA2QThXE8yVstIDnsIqZUEqOwLvbqYrzjALmhTA3bCGesj-o1IbljstgHh_ZB9paEHaeFS0xON270yiStwRUKBNJHULzDkMEpmk0sgNHbCtvUoiwJ?key=VReuh94fGGpJZLGsXsGdUQ)
    
- Accesibilidad y coherencia: Los diseñadores deben asegurarse de que cada caso de uso sea accesible a través de los elementos de la interfaz y que esta sea consistente, fácil de usar e integrada para el actor.
    
- Diseño físico de la interfaz: Los diseñadores luego crean esquemas aproximados de la disposición física de los elementos de la interfaz. Estos esquemas incluyen componentes adicionales necesarios, como ventanas, herramientas, carpetas y controles, que unen los elementos para formar una interfaz completa.
    
- Iteración entre lógica y física: Los esquemas físicos pueden desarrollarse después o junto con el diseño lógico, que utiliza las notas adhesivas para identificar los elementos clave de la interfaz.
    

  

#### Actividad: Estructurar el modelo de casos de uso ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXffp-P1cWVPyUIurKRAz0VZ1ZYhp3w60tzMTkXjHLwHjow-D3SWfn7q3jpagZwW9F2QJ7nnFZ_wWq_aiS4KoXeovnuhBIu0RS9c-FeOkhVOUSJGdzAIwDWYfH1xe-gfXDBH-TUG5nQDBhjTiv5JndfnOwM?key=VReuh94fGGpJZLGsXsGdUQ)

Objetivos:

- Extracción de funcionalidad general: Identificar descripciones de funcionalidad compartida que se pueden utilizar en descripciones más específicas de casos de uso.
    
- Extensión de funcionalidad opcional: Extraer funcionalidades adicionales u opcionales que pueden complementar las descripciones de casos de uso más específicas.
    

Antes de estructurar, el analista de sistemas debe haber identificado actores y casos de uso, representándolos en diagramas y explicando el modelo de casos de uso en su totalidad.

Los especificadores de casos de uso deben haber desarrollado descripciones detalladas de cada caso de uso, lo que proporciona una base para la reestructuración.

El analista puede reorganizar el conjunto completo de casos de uso para mejorar su comprensión y facilitar su uso. Esto implica buscar comportamientos compartidos y posibles extensiones dentro del modelo.

  

Identificar descripciones de funcionalidad compartida:

Se trata de encontrar acciones o conjunto de acciones repetidas por varios CU. Una solución posible es mandar todo a un CU que agrupe todo lo repetido (reduce la redundancia) y usar generalización.

Casos de Uso Concretos: Son los casos de uso terminados que pueden ser iniciados por un actor. Su instancia representa una secuencia completa de acciones ejecutadas por el sistema.

Casos de Uso Abstractos: Son casos de uso "semifabricados" diseñados para ser reutilizados por otros casos de uso. No pueden instanciarse por sí mismos y sirven como plantillas para definir comportamientos que serán utilizados por los casos de uso concretos.

Pagar Factura → Concreto.  
Ejecutar Transacción → Abstracto, es llamado por Pagar Factura.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfSybUtIT8p01J1LxC8hOUtJmVAJepLfMFxCqOHzuiH7hzpvbXzTnb5qK4nFBK_WI4hGoJXV4rlmAsbHOuy0QaLx1Q7c9GqQqbvhOJTKRgrrYEi4vYiCNvYgvd0_GT3dNgaCHjS_SpHRsMz8Mr8noFnMkgw?key=VReuh94fGGpJZLGsXsGdUQ)

CASO DE USO REAL:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfkcYSwCcVibciOVMY5ApRJ4qm-WPVeIkheGYIBFwiI6R7KdKJE_BKZMXHGOVzHJwdHBsxMZHxjLG-4aYUFqm0NTTP-Qmf_aZd9UPvqd6tqcXqqqgmRqW6wwI_MVW0MbH7-GWrfDkjxPS45JM2iHtkA1hA?key=VReuh94fGGpJZLGsXsGdUQ)

Identificar descripciones de funcionalidad adicionales y opcionales:

Las extensiones permiten agregar comportamiento adicional, ya sea opcional u obligatorio, de manera que otros casos de uso puedan utilizar esa funcionalidad sin tener que duplicarla.

Tenemos entonces:

Un caso de uso concreto no debe incluir comportamientos que son compartidos con otros casos de uso concretos; estos comportamientos deben ser extraídos en casos de uso abstractos o mediante extensiones.

Un caso de uso abstracto permite definir y reutilizar comportamientos compartidos por varios casos de uso concretos. HERENCIA

Una vez identificados los casos de uso concretos, abstractos y las extensiones, se pueden combinar para obtener un caso de uso real que ofrezca una secuencia completa de acciones observables por los actores.

Normalmente, al comenzar el modelado, se identifican los casos de uso reales, luego se extraen comportamientos comunes para definir casos de uso abstractos y, finalmente, se identifican comportamientos adicionales que se modelan como extensiones.

  

  

  

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXerAjbEGs6pqUxBg5jrHgLRqDXeRamHFzaKjZtZP5YhQEGWmpWzfpv6Eb_yl4IazR8Xh0OAeWrSMLbhlNMaslqcfhZHp2scLUA-6lDE-Emky3DvjIJFKCyA3dEafNncr_dbeHwcGv_mBUaOoZGkIS79lPM?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf4qJeVue7cMAS5RCpIfEu2In-ZUKxaGEfcgNiF3Ut73muhyjNTEFmTdqhmIydvVhaft2bSvzKgRjmlmYomD0vxoHMreaG-3vQ9Z0jDRn0FQlA-Nm0bIKG0F8AOnciUx_VVV-emEzD07xsomYV6dqtsyP6o?key=VReuh94fGGpJZLGsXsGdUQ)

  

Por otro lado las relaciones de inclusión, también usadas para compartir comportamiento. Son una herramienta útil cuando se necesita reutilizar comportamiento incondicional y encapsulado entre casos de uso. Sin embargo, debe usarse con precaución para no complicar innecesariamente la estructura del modelo. Es importante mantener los casos de uso alineados con los casos de uso reales del sistema, gestionando cuidadosamente el número y tamaño de los casos de uso para evitar una sobrecarga en el proceso de especificación y análisis.

### Resumen de la Captura de Requisitos

Se aborda la captura de requisitos de un sistema mediante:

- Modelo del negocio o del dominio: Establece el contexto del sistema.
    
- Modelo de casos de uso: Captura los requisitos funcionales y no funcionales específicos. Incluye una descripción general, diagramas y detalles de cada caso de uso.
    
- Esbozos de interfaces de usuario y prototipos: Representan el diseño de las interfaces para cada actor.
    
- Especificación de requisitos adicionales: Detalla requisitos genéricos no vinculados a un caso de uso específico.
    

Estos resultados son fundamentales para los flujos de trabajo de análisis, diseño, implementación y prueba. Los casos de uso guiarán el trabajo iterativo, vinculando las fases de análisis y diseño con un conjunto de casos de prueba en la fase de pruebas.