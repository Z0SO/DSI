### ¿QUÉ ES?

Es el proceso de averiguar lo que se debe construir. De hecho, es tan difícil que todavía no es poco común para los equipos de proyecto comenzar a escribir código (lo cual es bastante fácil) antes de haber definido claramente lo que debe hacer ese código (lo cual es difícil de determinar).

**Objeto**: Guiar el desarrollo a un sistema correcto.

Se puede basar en el modelo de negocios o dominio.  
- **Modelo de negocios**: lo que quiere el cliente (actor de negocio).  
- **Modelo de dominio**: lo que se va a almacenar desde el punto de vista del sistema.

- **Modelo de negocios** = actividades de negocio.

#### Usuarios:
- Visión incompleta de sus necesidades.
- No comprenden el alcance del sistema hasta el final (retrasos).

---

### Visión general de la captura de requisitos

Cada proyecto de software es diferente. Esta singularidad proviene de las diferencias en el tipo de sistema, el cliente, la organización de desarrollo, la tecnología, etc. De igual forma, existen diferentes puntos de partida para la captura de requisitos:

- En algunas ocasiones, comenzamos haciendo un modelo del negocio, o comenzamos con un modelo de negocio que ya está en desarrollo por parte de alguna otra empresa.
- En otros casos, el cliente puede haber ya desarrollado una especificación de requisitos completa y detallada que no esté basada en un modelo de objetos, a partir de la cual podemos comenzar y negociar los cambios.

---

### El objetivo del modelado del dominio
Comprender y describir las clases más importantes dentro del contexto del sistema.  
Los dominios de tamaño moderado normalmente requieren entre 10 y 50 de esas clases. Los dominios más grandes pueden requerir muchas más. Los cientos de clases candidatas que los analistas pueden extraer del dominio se guardan como definiciones en un glosario de términos, para evitar que el modelo del dominio se haga demasiado grande y requiera más esfuerzo del necesario.

El glosario y el modelo del dominio ayudan a los usuarios, clientes, desarrolladores y otros interesados a utilizar un vocabulario común.

---

### Flujo de trabajo de la captura de requisitos
![Captura de requisitos](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcHYQiSUoKQ8iPc6mNw5fPJKhENud1yiyWUJdS6xwlaId-dkfROofJSxTXyRplz5XA8wmFa59FFODYjUck-H_o_sFENM1ClbPmE-QyLYoE2PiyNZDa5FeLuoHfEl-xMTDAQy4AKgCvex44ClhIORC6PLfOe?key=VReuh94fGGpJZLGsXsGdUQ)

1. **Listar los requisitos candidatos**  
   La lista de características deseadas del sistema constituye los requisitos candidatos. Es fundamental para la planificación.

   De cada característica se registra:
   - **Nombre corto**
   - **Descripción**
   - **Estado** (propuesto, aprobado, incluido o validado)
   - **Coste estimado de implementación** (en términos de recursos y horas-hombre)
   - **Prioridad** (crítico, importante o secundario)
   - **Nivel de riesgo asociado** a la implementación de la característica (crítico, significativo u ordinario)

   Relaciones de traza con el caso de uso:  
   Escribir lo que se espera del sistema. Escuchar al cliente y anotar frases. Hacer preguntas para especificar lo que se requiere. Usar nombres cortos de características y breves descripciones. Hablar en términos resumidos y planificar en líneas generales.

2. **Comprender el contexto del sistema (más importante)**

   **Modelo de Dominio**:  
   Comprender, describir y capturar las clases más importantes de objetos en el contexto del sistema. Esto abarca:
   - Cosas que existen o eventos que ocurren en el entorno del sistema.
   
   Tres formas típicas:
   - **Objetos del negocio**: cosas que se manipulan en el negocio (como pedidos, cuentas, contratos, etc.).
   - **Objetos del mundo real**: conceptos de los que el sistema debe hacer seguimiento (como aviación enemiga, misiles, trayectorias, etc.).
   - **Sucesos**: cosas que ocurrirán o han ocurrido (como la llegada de un avión, su salida, la hora de la comida, etc.).

   El Modelo de Dominio (MD) se representa mediante diagramas de clases y permite usar un vocabulario común.

   **Modelo de dominio** = Modelo de clases conceptuales.  
   **Modelo de negocio** = Procesos del negocio desde la perspectiva de uso, ofreciendo valor.

   El modelo de objetos del negocio describe cómo cada caso de uso de negocio es llevado a cabo por un conjunto de trabajadores que utilizan un conjunto de entidades del negocio y unidades de trabajo.

   ![Diagrama de Modelo de Negocio](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKtS3C_7sRiudv1QB633uvFPFulcFxz4bLERFB_riVX6NcMn4tRoAWRaDccNhymucdcHLiiYB3ZDbN1zFYqIOQrhRA83BVuXUMyUBQZ-OAYw-fcG3PvgHZsRvwFJYvKv9CKk8NxxIXB7qptoulhkTj9m03?key=VReuh94fGGpJZLGsXsGdUQ)

Se pueden usar distintos enfoques: modelo de dominio, modelo de negocio o ninguno de los dos. Idealmente, se debe utilizar alguno y reflejar el diagrama de clases. Incluye modelo de negocio y modelo de objetos del negocio.

---

### ¿Cuáles son los diagramas del modelo de negocio?
- **Diagrama de interacción**.
- **Diagrama de actividades**.

3. **Capturar requisitos funcionales**  
   Son las cosas que el sistema debe hacer. Se identifican a través de los casos de uso, que describen las interacciones entre los actores y el sistema.

   Se capturan los requisitos funcionales y no funcionales específicos para cada caso de uso.

4. **Capturar requisitos no funcionales**  
   Los requisitos no funcionales especifican las propiedades del sistema, tales como:
   - **Requisitos de interfaz**: formatos, tiempos, u otros factores relevantes en la interacción.
   - **Requisitos físicos**: material, forma, tamaño o peso.
   - **Restricciones de implementación**: ambientales y de implementación.
   - **Restricciones de diseño**: rendimiento, dependencias de la plataforma, mantenimiento, extensibilidad y confiabilidad.

   Algunos requisitos no funcionales son más genéricos y no se pueden conectar a un caso de uso particular ni a una clase específica del mundo real. Se mantienen como una lista de requisitos suplementarios.

## Captura de Requisitos como Casos de Uso

Los requisitos funcionales pueden estructurarse eficazmente como **casos de uso**. Esta forma de modelado permite capturar las necesidades del sistema de una manera **sistemática** e **intuitiva**. Además, se enfoca en los **usuarios** y en las **necesidades comerciales** que deben satisfacer, asegurando que se agregue valor a cada usuario o sistema externo.

---

### Casos de Uso

Los **casos de uso** ofrecen una estructura clara para detallar las interacciones del sistema, y se enfocan en los resultados valiosos para los actores involucrados.

#### Componentes Clave del Modelo de Casos de Uso:

- **Actor**: Representa a los usuarios externos del sistema. Pueden ser trabajadores o actores del negocio que interactúan con el sistema.
  
- **Caso de Uso**: Son fragmentos de funcionalidad que el sistema ofrece, con el fin de proporcionar un valor a los actores. Pueden tener atributos específicos para cada ejecución del caso de uso, como ejemplos de valores locales que no son compartidos entre instancias.

![Diagrama de casos de uso](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZhxKakRt-LVhASW78zDLys3elvsw_h-qqKMb1r609iFL5W_XfJ6-kmRsqHfUqDwPONnyakJPEYG3RZQi5Vhqliz2nTbN5TOqFJgAXC88Xm_7DpFPhm6w_gkBAB4TV_me1YesxHTJiIe3qCmkuLisTuvUR?key=VReuh94fGGpJZLGsXsGdUQ)

#### Otros Elementos Importantes:

- **Descripción de la Arquitectura**: Una vista del modelo que resalta los casos de uso más significativos para la arquitectura del sistema.
  
- **Glosario**: Define términos clave utilizados por los analistas y diseñadores para describir el sistema.

- **Prototipo de Interfaz de Usuario**: Ayuda a definir cómo los actores interactúan con el sistema.

#### Roles de los Trabajadores en el Proceso:

- **Analista de Sistemas**: Responsable de mantener la consistencia entre los casos de uso y el modelo global.
  
- **Especificador de Casos de Uso**: Detalla cada caso de uso, trabajando directamente con los analistas y describiendo el funcionamiento detallado.

- **Diseñador de Interfaz de Usuario**: Realiza bocetos visuales de las interacciones de los usuarios, pero no se encarga de la implementación final.

- **Arquitecto**: Prioriza los casos de uso desde la perspectiva arquitectónica.

---

### Flujo de Trabajo en la Captura de Requisitos

El flujo de trabajo para la captura de requisitos en forma de casos de uso incluye actividades de identificación, priorización y análisis detallado.

![Flujo de Trabajo](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeOl0hjp7P_Sgn9Q41xxJAxihBEwznyu2PwW1H-0nzGyywa8tsIy8K4X7isEW_HJChTM-sLVY1PqINzcfSfwPHkDXy4dFiYO4DqZyY_30KQPwBam0OfuNYfAxDPYZMRfr3cTd0ZFwM6sz3bliBSA9_Co-fy?key=VReuh94fGGpJZLGsXsGdUQ)

#### Actividad 1: Buscar Actores y Casos de Uso

El objetivo principal de esta actividad es **delimitar el sistema** y **esbozar** las interacciones entre actores y funcionalidades esperadas. Se realiza mediante:

- **Modelos** y **Reuniones con el Cliente**.
- **Identificación de actores y casos de uso**, utilizando un glosario común para estandarizar las descripciones.

![Identificación de Actores y Casos de Uso](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdHt_NyrAXxgIvf-zHBQA7-wle1cPOzvMndSv5HbaV0BQQbrzGbgn9sRVMPrpKHKISKOhSFEeyI_oZayD3sAqX34p93frLzXnDN0BvdjnSsZ8XqKjaeBBdMMkuT5390wuYT1pxKQTalD_CiGUhiTZhGxKlX?key=VReuh94fGGpJZLGsXsGdUQ)

##### Pasos para Encontrar Actores y Casos de Uso:
1. **Encontrar los Actores**: Utilizar modelos existentes o reuniones con el cliente.
2. **Identificar Casos de Uso**: A través del modelo de negocio, entrevistas con actores y reuniones con el cliente.
3. **Definir Descripciones Breves**: Explicar de manera concisa cómo interactúan actores y sistema.

#### Actividad 2: Priorizar Casos de Uso

Una vez identificados, los casos de uso deben **priorizarse** según su importancia en el desarrollo inicial. Esto permite determinar qué funcionalidades se deben implementar primero.

![Priorizar Casos de Uso](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdv-0iYeJbswhpsiW6NkebGwZcfYpnJXR-w_0OIRBhgcyc26X1SiXxQ-dKiqbt3mK8zhn55SMofUtJfsJDqHIkUwRW37WC26FibW6KI1TAnyz2lnak1wW8zY40i9dowafcQzlZugYsuiwOOjADE-DyKRMbb?key=VReuh94fGGpJZLGsXsGdUQ)

El resultado de esta actividad se visualiza en la **vista de la arquitectura del modelo de casos de uso**, lo que ayuda a planificar las iteraciones de desarrollo y asegurar que se aborden primero los casos de uso más críticos.

#### Actividad: Detallar un caso de uso

![Imagen caso de uso](https://lh7-rt.googleusercontent.com/docsz/AD_4nXepG3IxC0RUe48QgcPfO2Wtj9L2k9MIXdLZm-wHVldCN_LFz_TT78d0bGYGqCeVDgLErq6iHQAvbJopbTPeIg-5opBlcyLzNis08IgVK7bhEbLUSZ1VWI2JbL_2yx9d7AERDSbOKYOpl0pZM65_6wafzHST?key=VReuh94fGGpJZLGsXsGdUQ)

Su objetivo es detallar cada caso de uso describiendo su flujo de sucesos, cómo comienza, termina y cómo interactúa con los actores.

El especificador de casos de uso debe trabajar en estrecha colaboración con los usuarios reales, entrevistándolos, discutiendo propuestas y revisando las descripciones.

Se obtiene como resultado una descripción detallada del caso de uso en texto y diagramas.

A partir del modelo y los diagramas de casos de uso, se debe especificar cada caso en detalle, describiendo paso a paso las acciones (entradas, salidas y flujo de eventos).

**Estructurar la descripción de CU**  
Pensando como máquina de estado, secuencia de acciones o estados en un CU.

![Diagrama de flujo](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdRM3_mVKXDOLO6TyxYXvN30NVqXJ0k6FP7c40fgD8I2FTB14nVCh7CAnZmUQDucgEkfvh_7JEjtCoRNYrvJv6WRTRrYjEqWxMcLrnggPRs1OQtNJpZ2opHQnTO2Uc5QozN6Ed319V9a23wiXplsgB8Z77B?key=VReuh94fGGpJZLGsXsGdUQ)

**¿Qué debe incluir la descripción?**

Para una descripción completa de un caso de uso, se deben incluir los siguientes elementos:

1. **Precondición:** Definir el estado inicial antes de que comience el caso de uso.
2. **Inicio:** Especificar cómo y cuándo comienza, es decir, la primera acción a ejecutar.
3. **Secuencia:** Ordenar las acciones de forma numerada, indicando el orden requerido si lo hay.
4. **Finalización:** Describir cómo y cuándo termina el caso de uso, junto con las postcondiciones (estados finales).
5. **Caminos no permitidos:** Incluir rutas de ejecución que no están permitidas (ej. acciones imposibles para el usuario).
6. **Caminos alternativos:** Describir las rutas alternativas dentro del caso de uso, indicando si solo se ejecutan bajo ciertas condiciones.
7. **Interacción del sistema con los actores:** Explicar cómo el sistema interactúa con los actores y los cambios que estas acciones producen.
8. **Uso de objetos, valores y recursos del sistema:** Detallar cómo el sistema utiliza sus recursos y asigna valores (ej. transferencias de dinero, uso de facturas, etc.).
9. **Acciones del sistema:** Especificar claramente las acciones que realiza el sistema, diferenciándose de las acciones de los actores. Esto asegura que la descripción sea lo suficientemente precisa para usarla como especificación del sistema.

**Requisitos no funcionales asociados a cada CU particular**

**Formalización de Descripción**

En caso de tener una descripción demasiado compleja, en lugar de un diagrama de máquinas de estados, se puede optar por las siguientes opciones:

- Diagramas de estados de UML para describir los estados de los casos de uso y las transiciones entre esos estados.
- Diagramas de actividad para describir las transiciones entre estados con más detalle como secuencias de acciones.
- Diagramas de interacción para describir cómo interactúa una instancia de caso de uso con la instancia de un actor.

---

#### Actividad: Prototipar interfaz de usuario

![Prototipo de interfaz](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf2Cu49ecSDwcLBJoXQmXRXRtTBvXhsGX88-b0E4R64HxhNGVnwHR8SQDhO6KtE4aauvALVpmHUK86Wm2NTpCD60krtIeJGVkkM48fsp-5xABycw7xR_cA6Z2QrVvFhUa5Z16oLVn2p0fhtVMoX60F5iW0?key=VReuh94fGGpJZLGsXsGdUQ)

Su objetivo es construir un prototipo de interfaz de usuario que permita a los usuarios ejecutar los casos de uso de manera eficiente.

Se parte de la base de que el analista de sistemas ya ha desarrollado un modelo de casos de uso que define los usuarios y sus necesidades. Además se tiene la descripción completa de cada CU.

**Proceso:**

- Diseñar la interfaz de usuario basándose en los casos de uso, comenzando con un diseño lógico que identifique los requisitos de la interfaz para cada actor.
- Luego, crear el diseño físico y desarrollar prototipos que ilustran cómo los usuarios interactúan con el sistema.

**Puntos clave para crear el diseño lógico de una interfaz de usuario:**

El diseñador debe identificar los elementos de la interfaz (como íconos, listas u objetos) que los actores utilizarán para interactuar con los atributos de los casos de uso (usualmente están en el glosario).

Para cada actor, se debe revisar cada caso de uso que este pueda acceder, y determinar los elementos de interfaz necesarios para habilitar sus acciones.

**Flexibilidad:** Un mismo elemento de interfaz puede desempeñar distintos roles en diferentes casos de uso, por lo que debe diseñarse con flexibilidad.

**Preguntas clave para cada actor:**

- ¿Qué elementos de interfaz necesita para el caso de uso?
- ¿Cómo se relacionan entre ellos?
- ¿Cómo se utilizan en los diferentes casos de uso?
- ¿Cuál debería ser su apariencia?
- ¿Cómo deberían manipularse?

**Puntos clave sobre la creación de un diseño y prototipo físico de la interfaz de usuario:**

- **Notas adhesivas:** Técnica para representar los elementos de la interfaz de usuario.

![Notas adhesivas](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdK3mULFdpwOX_UKmiBpMoHij-QRDtCGJLGHLL9u72BA2QThXE8yVstIDnsIqZUEqOwLvbqYrzjALmhTA3bCGesj-o1IbljstgHh_ZB9paEHaeFS0xON270yiStwRUKBNJHULzDkMEpmk0sgNHbCtvUoiwJ?key=VReuh94fGGpJZLGsXsGdUQ)

- **Accesibilidad y coherencia:** Los diseñadores deben asegurarse de que cada caso de uso sea accesible a través de los elementos de la interfaz y que esta sea consistente, fácil de usar e integrada para el actor.
- **Diseño físico de la interfaz:** Los diseñadores luego crean esquemas aproximados de la disposición física de los elementos de la interfaz. Estos esquemas incluyen componentes adicionales necesarios, como ventanas, herramientas, carpetas y controles, que unen los elementos para formar una interfaz completa.
- **Iteración entre lógica y física:** Los esquemas físicos pueden desarrollarse después o junto con el diseño lógico, que utiliza las notas adhesivas para identificar los elementos clave de la interfaz.

---

#### Actividad: Estructurar el modelo de casos de uso

![Estructuración de casos de uso](https://lh7-rt.googleusercontent.com/docsz/AD_4nXffp-P1cWVPyUIurKRAz0VZ1ZYhp3w60tzMTkXjHLwHjow-D3SWfn7q3jpagZwW9F2QJ7nnFZ_wWq_aiS4KoXeovnuhBIu0RS9c-FeOkhVOUSJGdzAIwDWYfH1xe-gfXDBH-TUG5nQDBhjTiv5JndfnOwM?key=VReuh94fGGpJZLGsXsGdUQ)

**Objetivos:**

- **Extracción de funcionalidad general:** Identificar descripciones de funcionalidad compartida que se pueden utilizar en descripciones más específicas de casos de uso.
- **Extensión de funcionalidad opcional:** Extraer funcionalidades adicionales u opcionales que pueden complementar las descripciones de casos de uso más específicas.

Antes de estructurar, el analista de sistemas debe haber identificado actores y casos de uso, representándolos en diagramas y explicando el modelo de casos de uso en su totalidad.

Los especificadores de casos de uso deben haber desarrollado descripciones detalladas de cada caso de uso, lo que proporciona una base para la reestructuración.

El analista puede reorganizar el conjunto completo de casos de uso para mejorar su comprensión y facilitar su uso. Esto implica buscar comportamientos compartidos y posibles extensiones dentro del modelo.

**Identificar descripciones de funcionalidad compartida:**

Se trata de encontrar acciones o conjunto de acciones repetidas por varios CU. Una solución posible es compartir estos fragmentos de funcionalidad para evitar redundancia y hacer el sistema más comprensible y flexible.

**Extensión de funcionalidad opcional:**

La extensión puede representar una funcionalidad adicional que se activa solo cuando se cumplen ciertas condiciones.
