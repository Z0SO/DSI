# Arquitectura de Software

La **arquitectura de software** es el esquema general de un sistema, un plano abstracto compuesto por elementos y sus relaciones. Toda arquitectura define la base sobre la cual se construye el sistema, guiando su estructura y evolución.

![Esquema general del sistema futuro](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeGc7WBBiiuJp3Oo8vPe73t8wjqO3I6uTwPX0iX0LoxChI-XN5I_yRhg8-NUd9XrPvi1r8YZ4Wyb0ykcYTtA8QihsQKsKwdptxs_dWkaDdG4N2uiYmtsTlS8jIub91nyOl5ObUVPw?key=VReuh94fGGpJZLGsXsGdUQ)

## Concepto

La arquitectura de software es un esquema abstracto que describe la estructura y la organización de un sistema. Aunque es fundamental para el diseño y desarrollo del sistema, no es la única parte que determina la calidad de un proyecto; todo el ciclo de vida del sistema influye en su éxito.

## ¿Por qué es necesaria la Arquitectura de Software?

### Potenciar Atributos de Calidad
La arquitectura permite mejorar las **características no funcionales** del sistema, como:
- Seguridad
- Rendimiento
- Modificabilidad
- Usabilidad
- Reusabilidad

Por ejemplo, si el sistema debe ser seguro, la arquitectura definirá los componentes y sus interacciones para proteger la información.

### Gestionar el Cambio
La arquitectura facilita **la modificabilidad** del sistema. Los cambios se pueden clasificar en tres categorías:
- **Local:** Modificación de un único componente.
- **No local:** Varios componentes modificados.
- **A nivel de arquitectura:** Requiere cambiar toda la estructura del sistema.

### Mejora la Comunicación entre Stakeholders
La arquitectura es suficientemente abstracta para que cualquier parte interesada (clientes, gerentes, desarrolladores) pueda comprenderla y dar retroalimentación sobre el sistema.

### Decisiones de Diseño Iniciales
Las decisiones tomadas en la fase de arquitectura son las más difíciles de cambiar. Es como la **fundación de una casa**: una vez construida, modificarla sería costoso y complicado.

### Definición de Restricciones
El arquitecto define las **restricciones de calidad** y recursos que deben cumplirse en el sistema. Esto incluye:
- Calidad del software.
- Recursos disponibles para el desarrollo.

Mientras se respeten estos límites, el sistema cumple con los estándares de la arquitectura.

### Influencia en la Estructura Organizacional
La arquitectura puede influir en la **estructura organizacional** y viceversa. Los grupos de trabajo asignados a tareas específicas afectan las decisiones arquitectónicas, como el diseño o las tecnologías a utilizar.

### Base para el Desarrollo Incremental
Una vez definida, la arquitectura permite comenzar con el **desarrollo incremental**. El sistema puede crecer en iteraciones con un esquema base ya estructurado.

### Planificación de Costes y Tiempo
La arquitectura permite **razonar sobre los costos y plazos** de desarrollo. Se pueden determinar de acuerdo con el equipo involucrado, el arquitecto y los desarrolladores.

### Reutilización y Transferibilidad
Una buena arquitectura puede convertirse en un **modelo reutilizable**, permitiendo desarrollar múltiples productos con una base similar.

### Enfoque en el Ensamblaje de Componentes
En lugar de centrarse solo en la creación de componentes, la arquitectura se enfoca en cómo **ensamblarlos adecuadamente** para que trabajen juntos y cumplan con los requisitos del sistema.

### Canalización de la Creatividad y Reducción de Complejidad
Al establecer restricciones claras sobre cómo deben desarrollarse los componentes, la arquitectura **canaliza la creatividad** de los desarrolladores, reduciendo la complejidad del sistema.

### Formación de Nuevos Miembros del Equipo
La arquitectura puede servir como una **herramienta de formación** para nuevos miembros del equipo, ayudando a entender rápidamente la estructura del sistema y las expectativas del desarrollo.
  

# Arquitectura de Software

La **arquitectura de software** es el conjunto de estructuras necesarias para razonar sobre un sistema. Estas estructuras comprenden los **elementos de software**, las **relaciones entre ellos** y sus **propiedades**. La arquitectura permite entender cómo se organiza el sistema y cómo interactúan sus componentes.

## Definición de Arquitectura

La arquitectura de software se puede entender como un subconjunto de **modelos** que representan la estructura de un sistema. Una **estructura** es un conjunto de elementos mantenidos unidos por relaciones, y una **vista** es la representación de una estructura.

- Un software está compuesto por muchas estructuras, y ninguna por sí sola constituye la arquitectura completa del sistema.
- La arquitectura es **abstracta**; los elementos no tienen una definición explícita, sino que se definen por sus relaciones y comportamientos.

## Categorías de Estructuras (Vistas)

### 1. Vista de Componentes y Conectores

- **Componentes**: Son las unidades principales de cálculo en tiempo de ejecución, como servicios, clientes, servidores, etc.
- **Conectores**: Representan los vehículos de comunicación entre componentes (por ejemplo, callbacks, operadores de sincronización).

**Ejemplo de patrones de conectores**:
- **Publish-Subscribe**: Publicador-Subscriptor.
- **Client-Server (con conmutación automática ante fallos)**: Un sistema cliente-servidor con respaldo automático en caso de fallo.

![Vista de Componentes y Conectores](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeG8Yoi9yUx1H8J05bnDnTjyziWRQ-8v8RjUTVZ_DcvUiCMRplrJS6yvdvNxD1nwyaraPXktEy1uZI14EnaytyYCsROyhW7jlu0LbvWwgdiH56u-7DOjBzPzndaT6WydbQBOk5ztvZtX-tCEUqt3lrIsK9W?key=VReuh94fGGpJZLGsXsGdUQ)

---

### 2. Vista de Módulos

- **Módulos**: Representan unidades de código o datos que deben construirse o adquirirse.
- Se equipara a la vista de paquetes en UML, mostrando cómo se estructura el sistema a nivel de unidades funcionales.

**Relación con el tiempo de ejecución**:
- No se centra en el comportamiento en tiempo de ejecución, sino en cómo se organizan los módulos dentro del sistema.

![Vista de Módulos](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdxNKCCZqiTaqiB_5nSX3OuO8xHpfBI2jB-b69JK-71vV-DjCuLi7mv0t16Vc279mAPQ5UbCdmv7Z9dd5IsPhWNmNTmyRyA_Lhwi9j-NbvVehtcTfGPsEffbcEjRBX4gcgtuxxejbEVPud4hN0Gi3JVQtIN?key=VReuh94fGGpJZLGsXsGdUQ)

- **Dirección de las flechas**: Acceso de uso.
- **En blanco**: Capa a nivel de usuario.
- **En gris**: Capa a nivel de núcleo del sistema.

---

### 3. Vista de Asignación

- **Asignación**: Establece la relación entre las estructuras de software y las estructuras no relacionadas con el software, como los entornos de desarrollo, prueba y ejecución.
- Se equipara a la vista de despliegue en UML.

![Vista de Asignación](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdRZaScY7LOdiB4te2p2WTMiYAJiJ08wQtOzxNaGON6MSDzL73q97XoGcRP4wCk0TX2cI2yUX8NjhR89glmAlpWl1Jkaxzl2BVEcEUSIFLyJOsVjfmIfCILDq4b1gYYYchgTN1dOgCUx50aIKrbVWfpi-hc?key=VReuh94fGGpJZLGsXsGdUQ)

---

### ¿Cómo se Relacionan las Vistas?

Cada una de estas vistas ofrece una perspectiva única del sistema. A pesar de que son distintas, no son independientes. Los elementos de una estructura están relacionados con los de otras vistas, y entender estas relaciones es crucial para comprender el sistema en su totalidad.

**Ejemplo**: Dos vistas para un sistema cliente-servidor.
- **Vista de Módulos (descomposición)** y **Vista de Componentes y Conectores (interacción)**.

![Ejemplo de Relación entre Vistas](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd8foDv_HOqX3E8dqRkrxtKp7CIVYz0TZhzekRFUtMyiXYfdX8dGUycSAnRCH2G4uzb2qlV3afKx-jyZtdU1fs0_ehLXJ4xbyRhrpKf6dXfrBXoaeYPL8Fwuazmoc5ZXI-ll-qXb2-UbjgFrbZ6gbii04uc?key=VReuh94fGGpJZLGsXsGdUQ)

---

# Diseño Arquitectónico

El **diseño arquitectónico** se ocupa de comprender cómo debe organizarse un sistema de software, identificando los principales elementos estructurales y sus relaciones. Este es un nexo crítico entre el diseño y la ingeniería de requisitos, pues ayuda a identificar y planificar la estructura general del sistema.

### Características del Diseño Arquitectónico
- **La funcionalidad no determina la arquitectura**.
- Se diseñan sistemas como conjuntos de elementos arquitectónicos cooperativos, como **módulos, capas, clases**, entre otros.

**Arquitectura a pequeña escala**: Se enfoca en la organización de programas individuales.  
**Arquitectura a gran escala**: Trata sistemas distribuidos y empresariales complejos.

---

## Flujo del Diseño Arquitectónico

![Flujo del Diseño Arquitectónico](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdb_XpZ2LRPNYJnOvuRIOafAk25V0B7-z2fxohL2EpB6u-64AYkHqkzq75beGKJoyiEUzyrmhG7wfAfQvn8RV1vPYlSR48EwpBitMu78RXXuKm5j-YPxDcVv-DC3vu9JKX5m_bCId-N1wBauc2vAKNmEm4?key=VReuh94fGGpJZLGsXsGdUQ)

---

## Decisiones de Diseño

La arquitectura de software puede verse como un conjunto de decisiones que deben tomarse durante el diseño del sistema. Estas decisiones incluyen preguntas clave que guiarán la elección de los elementos estructurales y sus interacciones.

![Decisiones de Diseño](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeaJJllfu2RqBQJQ23cN51JTw0LGToYVlE-YX1jefcdSqYcfBCWjyoWdzjuzAWpmAlaFkJz2lbT7eOW6qr3zR_TcO2iHr8vdGOe-jiiSVI9PPtOKpvsXruBN5IMOoCKaA_tkaJYtXbyCvUjU8MoXPTgI0LC?key=VReuh94fGGpJZLGsXsGdUQ)

---

### Vista 4+1 (Krutchen)

El modelo **Vista 4+1** describe la arquitectura del sistema utilizando múltiples vistas concurrentes. Cada vista representa el sistema desde el punto de vista de diferentes interesados, como usuarios finales, desarrolladores o directores de proyecto. El **+1** es la vista central que describe el sistema a través de **casos de uso**.

![Vista 4+1](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfjchy8DjeSCRBImrFjqsVLC1RdfWyVvxfnANPmXC5yT07Xpt0tMBOnx7bHgABNe0VJVRZhkGpvvbpQDlPU1raDBs8qgeUa5vM3C5TLkDNbTWQqOEyq8JJnc_xa24dvEoQKQmT6otU91-UrHO4VHoBIcZXl?key=VReuh94fGGpJZLGsXsGdUQ)
[Ver Video Explicativo](https://www.youtube.com/watch?app=desktop&v=r8ucofiI8vY)
## ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcth-bGk5IgBmgmmFbIh8VZQMw_VPY-b6DkRaZxvppCORevovom_QVu7bB_vanGE0S8ApzP9W9grlccthO0iFuGTrIttK0K2sXoqPhkwi2xFeqH3nQjakH6BWNq_lHagz-uEpVK9EBxfCu0jAlrnIvOAsIi?key=VReuh94fGGpJZLGsXsGdUQ)  

---
## Estilos Arquitectónicos

Un **estilo arquitectónico** define una familia de sistemas en términos de un patrón de organización estructural. Según Garlan y Shaw, este estilo determina el vocabulario de **componentes** y **conectores** que se pueden utilizar en instancias de ese estilo.

Un **patrón arquitectónico** es una descripción estilizada y abstracta de buenas prácticas, probadas en diferentes sistemas y entornos, como menciona Somerville.

---

## Patrones de Arquitectura (Centralizados)

### En Capas (Layered)

El patrón **en capas** se considera monolítico, ya que agrupa todo en un solo bloque de código, archivo o ejecutable. Este patrón divide el software en unidades denominadas **capas**, donde cada capa es una agrupación de módulos que ofrecen un conjunto cohesivo de servicios.

#### Características:

- **Independencia y separación**: Cada capa depende únicamente de la capa inmediatamente inferior y es independiente de las superiores.
- **Desarrollo incremental**: Permite un desarrollo modular y escalable.
- **Cambio y portabilidad**: Las capas pueden ser reemplazadas sin afectar al sistema global. Además, la localización de dependencias facilita la implementación multiplataforma.
- **Dificultades**: Mantener una separación limpia entre capas puede ser complicado, y el rendimiento podría verse afectado.

#### Comunicación entre capas:

- **Mensajes de abajo hacia arriba**: Asíncronos, sin necesidad de esperar una respuesta.
- **Mensajes de arriba hacia abajo**: Síncronos, se espera una respuesta para continuar.

#### Términos:

- **LAYER**: Capa lógica.
- **TIER**: Capa física o de implementación.

La **infraestructura** se refleja en la capa vertical derecha, que representa la realidad de que un modelo de capas riguroso no siempre es posible de implementar.

---

### Ejemplos de Aplicación:

- **Modelo OSI**: ![OSI Model 7 Layers](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdMaCqJerZSy4297dZrNXdTmGLQuKH-KnWgjwkXNg3b5WpgA5LCla3QcGu26uzmcLiyzu2j5pGnI2OM3jRDzoopgj_mftSBVI7X_IASX9pfHdxHA8OhbOkVamCujePA2eytupXJG696T-rGevi0AekNkubW?key=VReuh94fGGpJZLGsXsGdUQ)
    
- **Diagrama de capas sencillo**: ![Diagrama de Capas](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeNelua2Oem78hh_HhHtHPMU8ZJlh9XDiYm0ZtiUnYrYiM3PBo7hWujl75jBpXc6BW7bXUM8zADMvp-Fu8pP6fUo8AAKB-GCJAFpGOv-nMUbrsCEKXaQ29Wz9txo5gneDHSjGYKaG6CZh1m2OaUMU8_fl-N?key=VReuh94fGGpJZLGsXsGdUQ)
    
- **Ejemplo gráfico de capas con un lobo vestido**: ![Lobo vestido de capas](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdQbxAJVpiJMEKZQIV5MdteGmyZNEI_wdFu4eWFT1mMx9LsWwj4CKkaP12RANyFjRWbBksXeh8CYmaysRnzuzSffTdiF-00Xb0gGXeCzyzijYSeHyorFvimKi-5Dthl2UNBeMGtsQ4PZtiYqAPQ9kXfaoA?key=VReuh94fGGpJZLGsXsGdUQ)
    

Este ejemplo muestra un diseño erróneo de capas, ya que las capas están completamente interconectadas, lo que genera una dependencia total.

---

#### Ejemplos adicionales:

- **Capas con un lateral**: ![Capas con lateral](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbMRzvWmoNFwzuYY6j-O90mI7lUjalkxht-LCyFHM_DlE3MSeCOflq_LZ5aVnyPatfQdj9PTbMXcY5-iy3n4qPjyl05ueg59Qv_8uKlcyvc3wNfbczLt5SUxOeIewtSB4h2S383JsFGOSks-8J1SYfswU?key=VReuh94fGGpJZLGsXsGdUQ)
    
- **Capas con funciones comunes**: La capa D contiene funcionalidades comunes que necesitan todas las capas, como manejo de errores y métodos de acceso a bases de datos.
    
- **Diseño de capas segmentadas**: ![Capas segmentadas](https://lh7-rt.googleusercontent.com/docsz/AD_4nXft61leKUwQtNHXzT2_Tn97y1XXFo6niPjpkiQLPueTR17Ib_OathZSlVcT73JLMsU2J6KNrwSKmMcnjjBplyrKhvTmA9xqRwz8DV6dRC0eI5QnVVBndWdsAiYJCAkGgXVS_aSSfHtnh7K4v0Vu6bkQulUs?key=VReuh94fGGpJZLGsXsGdUQ)
    

En este diseño, los segmentos de la capa superior no pueden ser utilizados entre sí, pero sí pueden hacerlo los de la capa inferior.

## Repositorio / Pizarrón (Shared-Data)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdptz5mXhZfH4aXsMFosH-dYi2YJCC49YurDvXX-7kX3wzrA7NVxJ0q-xqz9fbJaeOmvYjKEv6ExVbxZaC83z4ql417i2a-iuJ_wCcS91n0cZrfZM8R0sW4SYUNQDoojrC7Dsj-l9X4MI0aTq2TQePpEkaV?key=VReuh94fGGpJZLGsXsGdUQ)

El **repositorio** es un componente central de almacenamiento de datos que permite la comunicación entre otros componentes del sistema. Estos componentes **independientes** no interactúan directamente entre sí, sino que comparten datos a través de este repositorio.

### Ventajas

- **Gestión consistente de datos**: Todos los datos se almacenan y gestionan de manera centralizada.
- **Uso eficiente de grandes volúmenes de datos**: Es útil para almacenar grandes cantidades de datos a largo plazo.
- **Acciones desencadenadas por los datos**: Puede utilizarse como un _pizarrón activo_ donde la inclusión de datos genera acciones.

### Desventajas

- **Cuello de botella**: El repositorio centralizado puede convertirse en un punto de congestión.
- **Punto único de fallo**: Un error en el repositorio puede afectar a todo el sistema.

### Ejemplo de uso

- **IDE con control de versiones**: Los datos de código y otros archivos se almacenan en un repositorio centralizado que permite la interacción con diferentes herramientas del IDE.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf5pwPUSQ0_p30zhVej0si4qLABVisDdphaL8CIWUqnWhOndh681uGggvp8Ta6wBlU4E-yKO3FFK_XGEWZnzUdwAEdEZkEndZ8n2FTVdkcJjgxdxGdVo6uCqESOZw4zRBY03ygQ3hGP1J1intfOo48no6s?key=VReuh94fGGpJZLGsXsGdUQ)

---

## Pipes and Filters (Canalizaciones y Filtros)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXffVmDpPOu_ArQkf-Tbsb-G-cs1KV4jEt7wfZUSNIDLQf1x0emEFyAUJkD0_iaGjE3b2oWO5fMTtzOC3pX23gBbb5WvBxxmKQy6SvoMxKv00GMsApJ62wn7UD4WQRZrGzup3_IXnJb3BOgXT-9DolDFyYA8?key=VReuh94fGGpJZLGsXsGdUQ)

La arquitectura **Pipes and Filters** es un patrón en el que los datos fluyen a través de una serie de filtros conectados por tuberías.

### Conceptos clave

- **Filtros**: Cada filtro transforma los datos de entrada y produce una salida. Los filtros procesan los datos de forma **incremental**, comenzando la salida antes de que toda la entrada haya sido procesada.
- **Tuberías**: Las tuberías actúan como **conectores** entre los filtros, permitiendo que los datos fluyan de uno a otro.

### Cuándo usar este patrón

Este patrón es útil cuando se requiere **transformaciones sucesivas** sobre un conjunto de datos, permitiendo que cada componente (filtro) realice su tarea en una secuencia ordenada.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdznTRCTMCQri2LuBpageSte9WqzteLb2cYjYieJLbqz4J3ocFOW52KwXCdEdkrCRBy0n30P_7mEKSYwHCPg0OdjWrZ5G71WLDeUfG4XonFIRHaf5RWgc8UolQ_rntInNn9nJSLVfotd_ZUP6xzHKg1ucpV?key=VReuh94fGGpJZLGsXsGdUQ)

---

## Microkernel / Plug-in

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcjXGB6kzcv2y5hIJq-vbzGBtE1pk9ryhG4jKNu3KET9tL6ul7YjGwYdV7xgT2oXvP8-_ho4bCs3s7R9uPMqaVTFe8eSYoM95dc9bmscPe0hBRzUAG7_-imQ2as_OAX2TnjfPvvIKQNhWtZh5ILXHUbZ7TA?key=VReuh94fGGpJZLGsXsGdUQ)

El patrón **Microkernel** consta de un sistema central mínimo y una serie de **plug-ins** que extienden y mejoran la funcionalidad de dicho sistema.

### Características

- **Sistema central**: Proporciona la funcionalidad básica necesaria para ejecutar el sistema.
- **Plug-ins**: Son componentes autónomos que aportan características adicionales y código personalizado.
- **Comunicación punto a punto**: Los plug-ins se comunican directamente con el sistema central o entre sí.

### Ventajas

- **Flexibilidad y extensibilidad**: Es fácil agregar nuevas funcionalidades sin modificar el sistema central.
- **Aislamiento de características**: Las funcionalidades adicionales están aisladas, lo que permite la adaptación del sistema.

### Desventajas

- **Cuello de botella**: La modificación del sistema central puede convertirse en un punto de fallo crítico.
- **Escalabilidad limitada**: No es ideal para sistemas de alta escala o con necesidades dinámicas.

### Resumen

Este patrón permite la **extensión del core** del sistema mediante el uso de plug-ins sin necesidad de modificar el sistema base.

### Ejemplo

- **Google Chrome**: El navegador tiene una funcionalidad básica, y las **extensiones** agregan nuevas características sin modificar el sistema central.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXegIqxKRhVms1dCGYbPQW0v9LTusZ-OVPdtwcplFxcxRsT9liOoNOwupAtSAR3nv0_v-qLQNCn0uN2nKfqNRu4xXxlmnnx3uvhpCqPD4qPC-PKKffywNSNwzKbB9COvKdwcAr_sCkaxSwqO5YRljLMr3LBG?key=VReuh94fGGpJZLGsXsGdUQ)

### Sistemas Distribuidos: Concepto y Arquitecturas

Un **sistema distribuido** es un conjunto de computadoras independientes que, al ser interconectadas, se presentan como un único sistema coherente para los usuarios. Esta arquitectura resuelve problemas de cuellos de botella y tolerancia a fallos, que eran comunes en sistemas más centralizados. La principal característica de los sistemas distribuidos es que el usuario interactúa con un sistema único, sin necesidad de saber que está compuesto por varios nodos.

![Sistemas Distribuidos](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdrIOp8NQ5BWOuKIdpn-0pENRdvuoRVR3NbDYCE2eScjSJYtXkK80xeyjHF0BCSM35i5lguoKMQPBimAUkLZHwOktn6amh-q5Hb85nS1gbfXYZ2tVCqfb94TrjTLaaENmkI5LKyaEO1Qj_tWb01EO75zrdL?key=VReuh94fGGpJZLGsXsGdUQ)

#### Objetivos de los Sistemas Distribuidos

1. **Recursos Compartidos**:
    
    - Reducen costos, pero a medida que crece el sistema, también surgen desafíos de seguridad.
2. **Transparencia**:
    
    - Ocultar la distribución física de los procesos y recursos. Aunque la transparencia total no siempre es alcanzable, es un objetivo fundamental.
    - Ejemplo de transparencia: ocultar si los datos se encuentran en un nodo o en varios.
    
    ![Transparencia](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf5NMYxQRdcecEqiOlDIo3m55xgA5ZjaDdD9_zE53qjWb1COBU16mzkS8FdT7NZ4htQ_LmZvjX_ZVQF9zjIiPByByqNewARn2bGZdnhPoqMpH36v49X9T8hfNmS8k77rabeSdlUhpVPJg6DOEbRskkxNUM?key=VReuh94fGGpJZLGsXsGdUQ)
    
3. **Apertura**:
    
    - El sistema sigue reglas estándar (protocolos) para describir la sintaxis y semántica de los servicios, permitiendo la interoperabilidad entre sistemas diferentes.
4. **Concurrencia**:
    
    - Los procesos pueden ejecutarse simultáneamente en equipos separados, permitiendo una mayor eficiencia y flexibilidad.
5. **Escalabilidad**:
    
    - Escalable en **tamaño** (más usuarios y recursos), **geográficamente** (distribución en grandes distancias) y **administrativamente** (gestión a través de varias organizaciones).
    - Sin embargo, a medida que se escala un sistema, puede experimentar pérdida de rendimiento debido al mayor volumen de datos y procesamiento.
6. **Tolerancia a fallos**:
    
    - Permite la disponibilidad continua mediante la redundancia y replicación de datos.

#### Desventajas de los Sistemas Distribuidos

- **Complejidad**:
    
    - Los sistemas distribuidos son difíciles de entender y gestionar, especialmente cuando se combinan dependencias como el procesamiento de múltiples procesadores o el ancho de banda limitado de la red.
- **Seguridad**:
    
    - La accesibilidad desde diferentes ordenadores puede abrir puertas a riesgos como espionaje o denegación de servicio, lo que complica la integridad de los datos.
- **Manejabilidad**:
    
    - La diversidad de componentes (hardware y software) hace que los fallos puedan propagarse y que se requiera más esfuerzo para mantener el sistema en funcionamiento.
- **Imprevisibilidad**:
    
    - La respuesta de un sistema distribuido depende de factores como la carga global, su organización interna y la carga de la red.

---

### Arquitecturas Comunes en Sistemas Distribuidos

#### 1. **Arquitectura Maestro/Esclavo**

- Utilizada en sistemas de tiempo real o en la replicación de bases de datos, esta arquitectura tiene un **proceso maestro** que coordina las acciones de varios **procesos esclavos**.
    
- **Proceso Maestro**: Responsable de la coordinación y control, gestionando la comunicación y los cálculos.
    
- **Procesos Esclavos**: Dedicados a tareas específicas como la adquisición de datos o el procesamiento de señales.
    

![Arquitectura Maestro/Esclavo](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcg-KI9MG4n9S7kYz2iugq54UISf2nii1SycWhkhI5QUnqNyb1BMgYz3WkxSdBa2YFDSmyrMyZfwbpnUYd9ksUe2MBkcWlbGn5HbF8mIV6eNYq089wLTHFQjqbvttRwKhgVNdp5NRzp66nfGcK18PKaxa5P?key=VReuh94fGGpJZLGsXsGdUQ)

**Aplicaciones**:

- Procesamiento distribuido predecible.
- Requiere tolerancia a fallos y alto rendimiento.

#### 2. **Arquitectura Cliente-Servidor**

- En esta arquitectura, los **clientes** solicitan servicios a los **servidores**, que proporcionan los recursos necesarios. Los clientes pueden estar distribuidos y no se conocen entre sí.
    
- **Características**:
    
    - Los servidores ofrecen servicios y los clientes los consumen.
    - Los clientes interactúan con los servidores a través de un protocolo estándar (por ejemplo, HTTP en la web).

![Arquitectura Cliente Servidor](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcT30jbU-9QuN4gepmmeJoBzXSqTKM8OAwBWMBP1tztxjqxACekzjZLSxoC55Z3ETxWx9273aoaPExzpo22Xp2GfvaScfaKY-EqOe42c9ZqZKFZLEmsESYLYA3yLF78a_6J4UhJJFZhbD5WBvDL0EZhhGgB?key=VReuh94fGGpJZLGsXsGdUQ)

**Ejemplo**: La web, donde un navegador (cliente) solicita servicios a un servidor web.

#### 3. **Arquitectura Cliente-Servidor de Dos Niveles (2-Tier)**

- En esta arquitectura, un único servidor maneja las capas de **gestión de datos**, **procesamiento de aplicaciones** y **base de datos**, mientras que el cliente maneja la **capa de presentación**.
    
- **Cliente Liviano**:
    
    - El cliente solo gestiona la presentación, mientras que el servidor maneja el procesamiento de datos y la base de datos.
    - **Ventajas**: Facilidad de gestión, pero con gran carga en el servidor y la red.
- **Cliente Pesado**:
    
    - El cliente maneja tanto la presentación como una parte del procesamiento de la aplicación.
    - **Ventajas**: Utiliza la potencia de procesamiento del cliente, pero requiere la instalación y mantenimiento de software en cada cliente.

![Cliente Pesado](https://lh7-rt.googleusercontent.com/docsz/AD_4nXckAX2Pk44AS4zJN0s06awRhW_f6dOpM8SHo3EQROtI53qET1FEPmTdDLYCzO_pHRkiEoHcTauQrGNqhWItwmQ9_UR4Lp1E5lu-xYsreniqxXdhE1UkmOby1DW8EYXHTX9BRqBgtQvH4GZ20Q_WVYO7Qu3n?key=VReuh94fGGpJZLGsXsGdUQ)

#### 4. **Arquitectura Cliente-Servidor Multinivel (Multitier)**

- Este modelo divide el sistema en múltiples capas que pueden ejecutarse en diferentes servidores. Esto mejora la escalabilidad y permite una mayor eficiencia, aunque aumenta la complejidad.
    
- **Características**:
    
    - Evita cuellos de botella que podrían aparecer con sistemas de 2 capas.
    - Aumenta la flexibilidad y el rendimiento, pero a costa de una mayor complejidad y costos.

**Desventajas**:

- Costos elevados de implementación y mantenimiento.

#### 5. **Componentes Distribuidos**

- Un sistema distribuido se compone de varios componentes interconectados que trabajan de manera conjunta para ofrecer servicios. Cada componente puede ser un nodo que ejecuta tareas específicas del sistema.

## Peer to Peer (P2P)

Los sistemas **peer-to-peer (P2P)** son sistemas descentralizados en los cuales **cualquier nodo** de la red puede realizar cálculos, aprovechando la capacidad de **cálculo** y **almacenamiento** de una gran cantidad de ordenadores conectados en red.

### Ejemplos de sistemas P2P:
- **Intercambio de archivos**: Protocolo BitTorrent.
- **Mensajería**: Jabber.
- **Sistemas de pago**: Bitcoin.
- **Bases de datos**: Freenet (base de datos descentralizada).
- **Telefonía**: Viber.
- **Computación distribuida**: SETI@home.

![Imagen ilustrativa P2P](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeu0BLbI-4EXXrUzvanSJ3frbzfbKlKq1Mqf4L_rhCbb48-nw_R6sH5BY_oEf12e7aogNVG0WmR1lMZayuOoPYeEnzuLUC8lECV24QX1CYZPUIgD-xiXV13HL0dZmeRIeVQR3yI0LRFdkML_BxgbwprbkbN?key=VReuh94fGGpJZLGsXsGdUQ)

### Modelos Arquitectónicos Peer-to-Peer

Existen diferentes modelos de arquitectura para redes P2P:

1. **Arquitecturas descentralizadas**: Todos los nodos tienen la misma capacidad.
2. **Arquitecturas semicentralizadas**: Un nodo central coordina algunas operaciones pero no gestiona completamente el sistema.

#### Ejemplo de Arquitecturas P2P:
- **Arquitectura P2P descentralizada**  
- **Arquitectura P2P semicentralizada**  
![Arquitectura P2P Semicentralizada](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcQz17dpCAIclxJI_mqZZLXK97YeAeIawuZr0thwtze8U7Rixt56HHqhxJd2aF4ydJGBVEVVNfYeXK6aCpWIpIt00R3jKun9cakak8XgdnZIOTeOfENqUSr66agk2sF2MFZAIXUsGoIqkPacLUwZ7bcbtM9?key=VReuh94fGGpJZLGsXsGdUQ)
![Arquitectura P2P Descentralizada](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeWP11MKTbL2azMTtqXeqNvHlYrEOxva2mrTes9EUESLsyEay7Ua19AdE5SHzRpzqd27CLnAfTsoorkzmEV7f4kbEqvypHA5NYVfj8dKiKdS27iThxOc0DywouH29r16Agzc_y8AZHDtDPRbuABa-XsTbk?key=VReuh94fGGpJZLGsXsGdUQ)

### Cuándo utilizar una arquitectura P2P:
- Cuando un sistema es **intensivo en cómputo** y el procesamiento puede ser distribuido en múltiples nodos.
- Cuando el sistema implica el **intercambio de información** entre nodos sin necesidad de centralizar la gestión o almacenamiento de la información.

### Problemas de Seguridad en P2P:
- **Seguridad**: La falta de una gestión centralizada permite que nodos maliciosos envíen **spam** y **malware**.
- Las **comunicaciones** deben ser cuidadosamente configuradas para proteger la **información local**, ya que, si no se hace correctamente, esta puede quedar expuesta a otros usuarios.

---

## Arquitectura Orientada a Servicios (SOA)

La **Arquitectura Orientada a Servicios (SOA)** organiza un sistema como un conjunto de **servicios independientes y sin estado**. Estos servicios pueden ser proporcionados por múltiples proveedores y estar distribuidos a través de la red.

### Elementos de SOA:
1. **Componentes**:
   - **Proveedores de servicios**: Ofrecen servicios a través de interfaces públicas, con preocupaciones como rendimiento, autorización, disponibilidad y costos.
   - **Consumidores de servicios**: Invocan los servicios, ya sea directamente o a través de un intermediario.
   - **ESB (Enterprise Service Bus)**: Intermediario que enruta y transforma mensajes.
   - **Registro de servicios**: Permite a los proveedores registrar servicios y a los consumidores descubrirlos en tiempo de ejecución.
   - **Servidor de orquestación**: Coordina las interacciones basadas en flujos de trabajo.

2. **Conectores**:
   - **Conector SOAP**: Utiliza el protocolo SOAP para comunicación síncrona.
   - **Conector REST**: Utiliza el protocolo HTTP para comunicaciones basadas en solicitudes/respuestas.
   - **Conector de mensajería asíncrona**: Utiliza un sistema de mensajería para intercambios asíncronos de mensajes.

### Desventajas de SOA:
- **Complejidad**: La construcción de sistemas SOA es compleja.
- **Evolución de los servicios**: No siempre es posible controlar cómo evolucionan los servicios independientes.
- **Rendimiento**: El middleware puede introducir sobrecarga y cuellos de botella en el rendimiento.
- **Garantías de rendimiento**: No siempre se ofrecen garantías de rendimiento.

![Imagen ilustrativa SOA](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfTkjk23TF2Nif3ZSoV5bHNnE7fwjx9njIMC0ca92jaPe77Lm5MgeAVpsf8MaUOXfFrET43X8mPyFYGlcqpbxPhwFeOss5HKQtyjonQTx16EsXJJBV-g8H325pcTQHAeih0nLF23L1zHclQguISJS9Gmzip?key=VReuh94fGGpJZLGsXsGdUQ)

---

## Microservicios

La arquitectura de **microservicios** es una forma de implementar **arquitecturas cliente-servidor**, donde el servidor se implementa como un conjunto de microservicios que interactúan.

### Características de los microservicios:
- **Autónomos**: No dependen de otros servicios, gestionan sus propios datos e interfaces.
- **Ligereza**: Usan protocolos ligeros para minimizar el gasto de comunicación.
- **Independencia de implementación**: Pueden implementarse usando diferentes tecnologías y lenguajes.
- **Desplegables independientemente**: Cada microservicio se ejecuta en su propio proceso y se puede desplegar de forma independiente.
- **Orientación al negocio**: Se enfocan en implementar las capacidades del negocio, no solo en servicios técnicos.

![Imagen ilustrativa de Microservicios](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfZXY1ksTdVGdAAjkBs4ArOxjWg6-SrBTcHvkfZZhucOmvC-pldwmrc6PunhRnpySNd0qLZpr7nO7xG9L6Zco163Qkim_NGgyfaGAUbmfjTImZYrNQyioot1ghF_V-Y-oeuP0k8NUg_4nSLks4LPFLw7KE?key=VReuh94fGGpJZLGsXsGdUQ)

### Comparación: Aplicación Monolítica vs Microservicios

En un **servicio de impresión de fotos**, la arquitectura monolítica es centralizada, mientras que los microservicios permiten tener una implementación distribuida y más flexible.

![Comparación Microservicios](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeIp-s1bikolsNN_Hl03IcVTW-uqHniZLNkaGTyq57Z7OzCjwgfcUQNKMKPlxc7rXnxHqpa8ihDEVdRqgmf5GCuT2TkndYM4Z3z7-utj3zqrkPJvEwyyFi_fN74CoqS3YDdiCaY86Be43wfu6gqW67XhDM?key=VReuh94fGGpJZLGsXsGdUQ)
![Ejemplo de Arquitectura Monolítica](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfBl3PMXpIrXzTtZJy2Oh3y_gj8kSFKZPtTDbnOHB1piLMpFW-__-0aldTHJk7RsdHd3lC_9k7sTKKbWFAvBUdw0R9kGEIJ8AKr1wh352MQ3lewikgjixyjZrFqBdNBCQKZUdbhIXE_mqlCa7MYwknescpK?key=VReuh94fGGpJZLGsXsGdUQ)

