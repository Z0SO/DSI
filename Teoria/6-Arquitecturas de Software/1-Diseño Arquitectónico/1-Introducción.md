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

---

## Referencias Visuales

![Imagen Final](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcth-bGk5IgBmgmmFbIh8VZQMw_VPY-b6DkRaD_N5rJmlF_wWwE4gxQw16Afdu6q4otgIUm6tPEOBYdcG8Xjle7Le9_VpwlMyLqcQkb7t3qX_jxqPQKwHtPtkC-V_4QKZpnnSg2sOhp_GdJVm3vH_gNWtLo?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  

## Estilos Arquitectonicos

Define una familia de sistemas en términos de un patrón de organización estructural. [Garlan y Shaw].

Determina el vocabulario de componentes y conectores que se pueden utilizar en instancias de ese estilo.

Un patrón arquitectónico es una descripción estilizada y abstracta de buenas prácticas, que ha sido probada en diferentes sistemas y entornos [Somerville].

## Patrones de Arquitectura (Centralizados)

### En Capas (Layered)

Se la considera monolítica: ensamblada en un solo bloque de código, archivo o ejecutable.

El patrón por capas divide el software en unidades llamadas capas.

Cada capa es una agrupación de módulos que ofrece un conjunto cohesivo de servicios.

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc29xbKnN2mLq3-Da7aGlomRvwTQiP3oTSTf2w5xSsTEhFH_682Hx3Wbh-Mn97HqYrix6cdIQo_gqMXCDsAeybXSWFJyHB5KVvwdtbxgQoaNCQWSFN2pdp8afldIvHJYD26dMy3xAlBhX2ejOEq9IhYz2r_?key=VReuh94fGGpJZLGsXsGdUQ)

- Una forma de lograr la separación e independencia.
    
- La funcionalidad se organiza en capas separadas.
    
- Cada capa depende de la capa inmediatamente inferior.
    
- Cada capa es independiente de las capas superiores.
    
- Desarrollo incremental de sistemas.
    
- Cambiable, una nueva capa puede reemplazar una capa existente.
    
- Portable, ya que los sistemas en capas localizan las dependencias de la máquina, implementaciones multiplataforma.
    
- Una separación limpia entre capas suele ser difícil.
    
- El rendimiento puede ser un problema.
    
- RIGUROSAMENTE cada capa solo puede comunicarse con la inmediata superior e inferior NADA MÁS.
    

LAYER y TIER SE TRADUCEN COMO CAPA

- LAYER: Capa lógica.
    
- TIER: Capa física o de implementación.
    

Mensajes de abajo hacia arriba: Asincronicos, no se espera una respuesta para continuar.

Mensajes de arriba hacia abajo: Sincronicos, se espera una respuesta para continuar.

La capa vertical de la derecha indica la infraestructura (por ej. el lenguaje que se utiliza), refleja que en la realidad es imposible utilizar un modelo riguroso de capas.

Ejemplos:

- Modelo OSI.![OSI Model 7 Layers](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdMaCqJerZSy4297dZrNXdTmGLQuKH-KnWgjwkXNg3b5WpgA5LCla3QcGu26uzmcLiyzu2j5pGnI2OM3jRDzoopgj_mftSBVI7X_IASX9pfHdxHA8OhbOkVamCujePA2eytupXJG696T-rGevi0AekNkubW?key=VReuh94fGGpJZLGsXsGdUQ)
    
- Un diagrama de capas sencillo con una clave sencilla que responde a la pregunta de usos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeNelua2Oem78hh_HhHtHPMU8ZJlh9XDiYm0ZtiUnYrYiM3PBo7hWujl75jBpXc6BW7bXUM8zADMvp-Fu8pP6fUo8AAKB-GCJAFpGOv-nMUbrsCEKXaQ29Wz9txo5gneDHSjGYKaG6CZh1m2OaUMU8_fl-N?key=VReuh94fGGpJZLGsXsGdUQ)
    

  

- Un lobo vestido de capas.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdQbxAJVpiJMEKZQIV5MdteGmyZNEI_wdFu4eWFT1mMx9LsWwj4CKkaP12RANyFjRWbBksXeh8CYmaysRnzuzSffTdiF-00Xb0gGXeCzyzijYSeHyorFvimKi-5Dthl2UNBeMGtsQ4PZtiYqAPQ9kXfaoA?key=VReuh94fGGpJZLGsXsGdUQ)
    

Esto no es un diseño por capas porque al estar todo conectado todas las capas dependen de todas y hay dependencia total.

- Capas con un lateral.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbMRzvWmoNFwzuYY6j-O90mI7lUjalkxht-LCyFHM_DlE3MSeCOflq_LZ5aVnyPatfQdj9PTbMXcY5-iy3n4qPjyl05ueg59Qv_8uKlcyvc3wNfbczLt5SUxOeIewtSB4h2S383JsFGOSks-8J1SYfswU?key=VReuh94fGGpJZLGsXsGdUQ)
    

La capa D contiene cosas comunes que necesitan todas las capas (manejo de errores, métodos de acceso a BD, etc.).

- Diseño de capas con capas segmentadas![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXft61leKUwQtNHXzT2_Tn97y1XXFo6niPjpkiQLPueTR17Ib_OathZSlVcT73JLMsU2J6KNrwSKmMcnjjBplyrKhvTmA9xqRwz8DV6dRC0eI5QnVVBndWdsAiYJCAkGgXVS_aSSfHtnh7K4v0Vu6bkQulUs?key=VReuh94fGGpJZLGsXsGdUQ)
    

Los segmentos de la capa superior no pueden utilizarse entre sí, pero sí los segmentos de la capa inferior.

### Repositorio / Pizarrón (Shared-Data)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdptz5mXhZfH4aXsMFosH-dYi2YJCC49YurDvXX-7kX3wzrA7NVxJ0q-xqz9fbJaeOmvYjKEv6ExVbxZaC83z4ql417i2a-iuJ_wCcS91n0cZrfZM8R0sW4SYUNQDoojrC7Dsj-l9X4MI0aTq2TQePpEkaV?key=VReuh94fGGpJZLGsXsGdUQ)  
Los componentes independientes se comunican a través de un repositorio de datos central (tmb componente).

Los componentes independientes no interactúan directamente.

Todos los datos se pueden administrar de manera consistente.

Conviene cuando:

- Se generan grandes volúmenes de datos que tienen que ser almacenados durante mucho tiempo (repositorio-pasivo).
    
- La inclusión de datos en el repositorio desencadena una acción (pizarrón-activo).![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXddoKi781-j2rSLuzwyv9pQWfQoFHxpGMerqHYovy3baQ6qFo8WtSJSzuTz_wP7dFGYhpl_2G4sjSGU7xdK2deZ_f8-FL8q6V34UjT3yIGZS5VfgZv56vX-kls1He2tf3Hjy_9TmkYz72u1SoInBROjwqY?key=VReuh94fGGpJZLGsXsGdUQ)
    
- Lo uso cuando tengo datos y necesito trabajarlos en conjunto.
    

Desventaja:

- Cuello de botella.
    
- El repositorio es un único punto de fallo (afecta a todo el sistema).
    

  
  
  

Ejemplo: IDE con varias herramientas y un repositorio con control de versiones.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf5pwPUSQ0_p30zhVej0si4qLABVisDdphaL8CIWUqnWhOndh681uGggvp8Ta6wBlU4E-yKO3FFK_XGEWZnzUdwAEdEZkEndZ8n2FTVdkcJjgxdxGdVo6uCqESOZw4zRBY03ygQ3hGP1J1intfOo48no6s?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXchs4RsA5I1EvV-NYhSYOBscyi1bmcLbDCRL88jWhgEZr3WI6LKcqwCk0ezsLG1Wq3vNBPGno9yYmYB9SGQR5q3Eviz3zcnTp4RpMTvnWopnomaDTkelAmHFNSYQR8Bbv55Ilcp4ed7898SCKLG2O9UNDs?key=VReuh94fGGpJZLGsXsGdUQ)

### Pipes and Filters  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXffVmDpPOu_ArQkf-Tbsb-G-cs1KV4jEt7wfZUSNIDLQf1x0emEFyAUJkD0_iaGjE3b2oWO5fMTtzOC3pX23gBbb5WvBxxmKQy6SvoMxKv00GMsApJ62wn7UD4WQRZrGzup3_IXnJb3BOgXT-9DolDFyYA8?key=VReuh94fGGpJZLGsXsGdUQ)

Arquitecturas de tuberías o filtros o canalizaciones → PIPELINES.

Voy a usarla cuando necesite funcionalidades o transformaciones sucesivas sobre un conjunto de datos.

Cada componente tiene un conjunto de entradas y de salidas.

Filtro: Produce un resultado aplicando una transformación local a los flujos de entrada y calculando de forma incremental (usualmente) para que la salida comience antes de que se consuma la entrada.

Tubería: Es un conector entre filtros, conducto para los flujos de datos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdznTRCTMCQri2LuBpageSte9WqzteLb2cYjYieJLbqz4J3ocFOW52KwXCdEdkrCRBy0n30P_7mEKSYwHCPg0OdjWrZ5G71WLDeUfG4XonFIRHaf5RWgc8UolQ_rntInNn9nJSLVfotd_ZUP6xzHKg1ucpV?key=VReuh94fGGpJZLGsXsGdUQ)

d![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeJZi0iIASfWQ3zTkmj-lJih9LQ6tuoAafGbJRtmspfdQaWfZNakaxXHZEQV9UGZbZL9BpmcPcVXDqWZ73K3i84zw0Qzc0617nRHYsxgZ2omTtALB96J--pC8_AG5UVvcjqy8Kvu1QZNmAgrB6De2mK02eb?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  

### Microkernel / Plug-in

Consta de un sistema central y plug-in’s que proporcionan extensibilidad, adaptabilidad y aislamiento de las características de la aplicación y la lógica de procesamiento personalizada.

Sistema Central: Componente con la funcionalidad mínima requerida para ejecutar el sistema.

Plug-ins: Componentes independientes y autónomos que contienen procesamiento especializado, características adicionales y código personalizado destinado a mejorar o ampliar el sistema central.

La comunicación suele ser punto a punto.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcjXGB6kzcv2y5hIJq-vbzGBtE1pk9ryhG4jKNu3KET9tL6ul7YjGwYdV7xgT2oXvP8-_ho4bCs3s7R9uPMqaVTFe8eSYoM95dc9bmscPe0hBRzUAG7_-imQ2as_OAX2TnjfPvvIKQNhWtZh5ILXHUbZ7TA?key=VReuh94fGGpJZLGsXsGdUQ)

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcQGHaUATIWvtzInuAZiql8zJb_13HO915jRHCLOIe5311m5gOlXoFcKtfueWrCYdNH-9R9jldh5xlFjM-5JLRivPnS_48mtz4iVoFgmytIVZt7IdFnndMha5LxjeXpoPf5WMe8LERbGRoHOD9vxN0gwpI?key=VReuh94fGGpJZLGsXsGdUQ)

- El estilo de arquitectura de microkernel es flexible y extensible, permitiendo agregar fácilmente funcionalidad y características adicionales a una aplicación existente.
    
- Los módulos complementarios son componentes independientes que contienen lógica de procesamiento especializada, características adicionales, lógica de adaptador o código personalizado que mejora o extiende el sistema principal.
    
- El sistema principal necesita saber qué módulos complementarios están disponibles y cómo acceder a ellos, a menudo a través de un registro de módulos complementarios.
    
- Los módulos complementarios se pueden implementar de varias maneras, ya sea como bibliotecas/módulos separados, dentro de un solo conjunto de código consolidado o como servicios remotos.
    
- Se basa en iterativo incremental.
    
- Bajo costo, simple de entender.
    
- Se presentan cuellos de botella. No es muy apto para sistemas que requieren alta escalabilidad o elásticos.
    
- El core es el punto de entrada, por lo tanto también es un vector de fallo bastante grande.
    
- Si siempre se modifica el core, este patrón no es el apto.
    

Resumen: La funcionalidad del CORE es extendida mediante los Plug-ins. La idea principal es definir el Core de manera tal de no volver a modificarlo.

Ejemplo: Google Chrome tiene funcionalidad básica y las extensiones agregan funcionalidad.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXegIqxKRhVms1dCGYbPQW0v9LTusZ-OVPdtwcplFxcxRsT9liOoNOwupAtSAR3nv0_v-qLQNCn0uN2nKfqNRu4xXxlmnnx3uvhpCqPD4qPC-PKKffywNSNwzKbB9COvKdwcAr_sCkaxSwqO5YRljLMr3LBG?key=VReuh94fGGpJZLGsXsGdUQ)

## Sistemas distribuidos (CONCEPTO)

Un sistema distribuido es un conjunto de ordenadores independientes que aparece ante sus usuarios como un único sistema coherente. ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdrIOp8NQ5BWOuKIdpn-0pENRdvuoRVR3NbDYCE2eScjSJYtXkK80xeyjHF0BCSM35i5lguoKMQPBimAUkLZHwOktn6amh-q5Hb85nS1gbfXYZ2tVCqfb94TrjTLaaENmkI5LKyaEO1Qj_tWb01EO75zrdL?key=VReuh94fGGpJZLGsXsGdUQ)

La idea es separar al sistema en varios nodos o componentes (computadores), solucionando el problema de cuello de botella o tolerancia a fallos que tenían algunas arquitecturas. Además, el usuario nunca se debe enterar, solo debe ver el sistema como tal.

Objetivos de los Sistemas Distribuidos (Ventajas):

- Recursos compartidos: Lo principal es que reduce costos, pero a medida que crece, también hay que ver la seguridad.
    
- Transparencia: Es ocultar el hecho de que sus procesos y recursos están físicamente distribuidos en varios ordenadores.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf5NMYxQRdcecEqiOlDIo3m55xgA5ZjaDdD9_zE53qjWb1COBU16mzkS8FdT7NZ4htQ_LmZvjX_ZVQF9zjIiPByByqNewARn2bGZdnhPoqMpH36v49X9T8hfNmS8k77rabeSdlUhpVPJg6DOEbRskkxNUM?key=VReuh94fGGpJZLGsXsGdUQ)
    

La transparencia nunca se puede conseguir al 100%, incluso en algunos casos no conviene conseguirla.

- Apertura: Es un sistema que ofrece servicios de acuerdo con reglas estándar (Lenguaje de definición de interfaces) que describen la sintaxis y la semántica de dichos servicios. Por ejemplo, en las redes informáticas, las reglas estándar rigen el formato, el contenido y el significado de los mensajes enviados y recibidos. Estas reglas se formalizan en protocolos.  
    La interoperabilidad caracteriza el grado en que dos implantaciones de sistemas o componentes de distintos fabricantes pueden coexistir y trabajar juntos simplemente basándose en los servicios de la otra parte, tal y como especifica una norma común.
    
- Concurrencia: Los procesos pueden funcionar simultáneamente en equipos separados. Los procesos pueden comunicarse entre sí.
    
- Escalabilidad: Puede medirse en al menos tres dimensiones:
    

- Escalable con respecto a su tamaño, lo que significa que podemos añadir fácilmente más usuarios y recursos al sistema.
    
- Escalable geográficamente es aquel en el que los usuarios y los recursos pueden estar muy alejados.
    
- Administrativamente escalable, lo que significa que puede seguir siendo fácil de gestionar aunque abarque muchas organizaciones administrativas independientes.
    

Desgraciadamente, un sistema escalable en una o varias de estas dimensiones suele presentar cierta pérdida de rendimiento a medida que se amplía. (más datos a manejar, peor rendimiento)

La vinculación de red (conectar todo para tener el sistema) limita la escalabilidad. Al conectar las computadoras, depende como se haga, la escalabilidad que tendrá el sistema va a ser una.

- Tolerancia a fallos: Disponibilidad de varios equipos y posibilidad de replicar información (redundancia).
    

Algunas Desventajas:

- Complejidad: Difícil de entender sus propiedades emergentes y de probar, p. ej., el rendimiento dependiente de un procesador vs dependencia del ancho de banda de la red y de varios procesadores.
    

- Seguridad: Acceso desde varios ordenadores diferentes, espionaje del tráfico de red. Es difícil garantizar la integridad de los datos. Degradación por ataques de denegación de servicio.
    
- Manejabilidad: Diferentes tipos de computadoras, diferentes versiones del sistema operativo. Los fallos pueden propagarse a otras máquinas. Se requiere más esfuerzo para mantener el sistema en funcionamiento.
    
- Imprevisibilidad: La respuesta depende de la carga global del sistema, de su organización y de la carga de la red.
    

  
  
  

Formas muy utilizadas de organizar la arquitectura de un sistema distribuido:

### Arquitectura Maestro/Esclavo

Las arquitecturas maestro-esclavo se utilizan habitualmente en los sistemas en tiempo real con plazos de procesamiento, en los que puede haber procesadores independientes asociados a la adquisición de datos del entorno del sistema, al tratamiento de los datos y a la gestión de los cálculos y los actuadores. También se utilizan en replicación de BD.

Arquitectura maestro-esclavo, que se utiliza en sistemas en tiempo real en los que se requieren tiempos de respuesta de interacción garantizados.

Proceso Maestro: Responsable del cálculo, la coordinación y las comunicaciones, y controla los procesos «esclavos».

Procesos Esclavos: Dedicados a acciones específicas, como la adquisición de datos.

Adecuado para el procesamiento distribuido predecible, requisitos de alto rendimiento, tolerancia a fallos o precisión.

Los procesadores esclavos se encargan de las operaciones computacionalmente intensivas, como el procesamiento de señales y la gestión de equipos.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcg-KI9MG4n9S7kYz2iugq54UISf2nii1SycWhkhI5QUnqNyb1BMgYz3WkxSdBa2YFDSmyrMyZfwbpnUYd9ksUe2MBkcWlbGn5HbF8mIV6eNYq089wLTHFQjqbvttRwKhgVNdp5NRzp66nfGcK18PKaxa5P?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  

### Arquitectura Cliente Servidor

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcT30jbU-9QuN4gepmmeJoBzXSqTKM8OAwBWMBP1tztxjqxACekzjZLSxoC55Z3ETxWx9273aoaPExzpo22Xp2GfvaScfaKY-EqOe42c9ZqZKFZLEmsESYLYA3yLF78a_6J4UhJJFZhbD5WBvDL0EZhhGgB?key=VReuh94fGGpJZLGsXsGdUQ)

- La aplicación se modela como:
    

- Un conjunto de servicios proporcionados por servidores.
    
- Los clientes pueden acceder a estos servicios.
    

- Los clientes conocen a los servidores, pero no se conocen entre sí.
    
- Algún mecanismo de descubrimiento de los servidores.
    
- Los servidores no conocen a los clientes (a priori).
    
- Los servidores pueden o no tener estados.
    
- Los clientes y los servidores son procesos separados, en la misma máquina o en máquinas diferentes.
    

Los clientes interactúan solicitando servicios a los servidores, que proporcionan un conjunto de servicios. Algunos componentes pueden actuar como clientes y servidores. Puede haber un servidor central o varios distribuidos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdghZH87dYW6aUL_gd0kt-dx7Gl-wvbusRW1YwFJqrlmGphu_Uja_JAQV53sJRmfYP0kWOgXoPM5nmkVajT6wMg46GcJVzfMGJGJiYfGmwDK5q89w2GDWK8uqzNFJ9tD97hwiYH72xc_1SRH-bb4mbwQFw?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcwbZl717vkiapTGvVG-Pnjshu71fKQehuf2_8D7e8pltKqhKc_G88oCQ4CLYL6vXObYgiRLQZNyOdhzo9aQ84rqFJ6xcGHkH3sD8mz_w6cqHVq3eglyZ4wSLaUxAMRi1aMRG1wwLy-aEsk_Qa6LcpPtMJM?key=VReuh94fGGpJZLGsXsGdUQ)

Servidores tiene servicios usados por clientes

Internet es el ejemplo más facil, HTTP seria el conector, cliente el navegador, servidores de internet  
  

### Arquitectura C/S (Cliente-Servidor) de dos niveles (2-tier)

En una arquitectura cliente-servidor de dos niveles, el sistema se implementa como un único servidor lógico más un número indefinido de clientes que utilizan ese servidor.

Dos formas:

Cliente liviano: Capa de presentación en cliente, el resto en el servidor. La capa de presentación se implementa en el cliente y todas las demás capas (gestión de datos, procesamiento de aplicaciones y base de datos) se implementan en un servidor.

- Fácil gestión de clientes.
    
- Gran carga de procesamiento en el servidor y en la red.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc_4CZDraFfjGFaNBo81oztON4qtAgQEtHLJiZY6KQUxvXlxjrDLjNttSKszCYDCDPRFdlqzgO5q4doN5HCn_-i8oP634az-lgEsobzz0UapviMDhZyGNwtzBHvCTminjz3GFWGC3z7-VwCeRPB_rXcNgA?key=VReuh94fGGpJZLGsXsGdUQ)
    

Se utiliza cuando los sistemas viejos se migran a arquitecturas cliente-servidor. El sistema viejo actúa como un servidor en sí mismo con una interfaz gráfica implementada en un cliente.

Su principal desventaja es que supone una gran carga de procesamiento tanto para el servidor como para la red.

Cliente Pesado: Capa de presentación + aplicación en cliente. datos en servidor. Una parte o la totalidad del procesamiento de la aplicación se realiza en el cliente. Las funciones de gestión de datos y bases de datos se implementan en el servidor.

- Hace uso de la potencia de procesamiento disponible en el cliente.
    
- Se necesita desplegar y mantener el software en el cliente.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXckAX2Pk44AS4zJN0s06awRhW_f6dOpM8SHo3EQROtI53qET1FEPmTdDLYCzO_pHRkiEoHcTauQrGNqhWItwmQ9_UR4Lp1E5lu-xYsreniqxXdhE1UkmOby1DW8EYXHTX9BRqBgtQvH4GZ20Q_WVYO7Qu3n?key=VReuh94fGGpJZLGsXsGdUQ)
    

Se delega más procesamiento en el cliente, ya que el procesamiento de la aplicación se ejecuta localmente.

Más adecuado para nuevos sistemas C/S en los que las capacidades del sistema cliente se conocen de antemano.

Más complejo que un modelo de cliente ligero, especialmente para la gestión. Hay que instalar nuevas versiones de la aplicación en todos los clientes.

###   
Arquitectura C/S multinivel (multitier)

En una arquitectura cliente-servidor multinivel, las distintas capas del sistema, a saber, presentación, gestión de datos, procesamiento de aplicaciones y base de datos, son procesos separados que pueden ejecutarse en distintos procesadores.

De este modo se evitan problemas de escalabilidad y rendimiento si se opta por un modelo thin-client de dos capas, o problemas de gestión del sistema si se utiliza un modelo fat-client.

Desventajas: su coste y complejidad. En sistemas sencillos, las ventajas de la arquitectura multinivel pueden no justificar sus costes iniciales y continuos, en términos de hardware, software y complejidad de diseño e implementación.

Los niveles no son componentes, sino agrupaciones lógicas de componentes. Tampoco hay que confundir niveles con capas. Las capas son un patrón de módulos (una unidad de implementación), mientras que los niveles sólo se aplican a las entidades en tiempo de ejecución.

###   
Componentes distribuidos![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdJB9MTCPqyN8uCgynIZZc9_QqdkP8stBvum6e_kuuE1he4tdd_LPKgQohw2yPgvlTmN3IoYHJo3cPJggaVzOCqHiPBlJPbp3kyLdyfdUiqDPmt2asFmuA5ilUSKgymKj9A_IB114IL2cGdMU5mgU0jrxhJ?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdnO704ZBAYFUtTgYILaoAHoMXUKf02fNx60Xl6PqLoe1baU1sh7YU1c4AfuSooKOyzgSjnfizXWpYCMdRG2Q9013-qoQPy6vwQAac7ShSJlNtV87sPGmsR-EHaQ9MR5Cs_nL0ls0p7cD2c0cVjlaVjpD0X?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeD1hDX76pRKGFxImCNu730mzLM9YtPucwpkH7sqtF-xl5v6aEbqlCNru95GQh3Xnaoe6LdH_5i1P9NKezelDYhZ1XpkeOmsL1Pd4Yo07Dn9J7JRMm0W0V_T_yF3gnQx7m4FbOJ160CDwqYe_CUYvxlDonc?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcvf5Q_O1Zn1mgOePR1bDE8nGthSUXCNmg_k-oEzegkKrJx7eJ16ClLjxLZ9lWVWGkR5UtQO0jDZxSFI1WM5NuQnD_pJWJqfsEyErZd1G7K97gDDQf4OEYaFRC-9YqTGzdvkwXKZATDE0Mh3tc_ReD1LYY?key=VReuh94fGGpJZLGsXsGdUQ)

En una arquitectura de componentes distribuidos no hay distinción entre clientes y servidores.

Cada entidad distribuible es un componente independiente que presta servicios a otros componentes y recibe servicios de otros componentes.

La comunicación entre componentes se realiza a través de un sistema middleware.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf7X7xBnt-YUeVoToIK6o7BMPX5sYgi00D2kVDkOl-pS6lcuPXxIYjrwZGIEJmrYLKYV2XVdL24eTz1A88Q9SV736tT5o90sD-ouVbtEbAqEoNC7_EJtdg7vB_U7Ugv0oskTY0K2vqA-B_20wQz0BUQ1z6e?key=VReuh94fGGpJZLGsXsGdUQ)

Ventajas:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfum8DUOwpvjaioNmUV0P0EtnVW_08KMf_x1hbdasHNSiytyKb4M2YM1W36y5AC3q8zLoJnR-qluQ5HCU24P4MtNB0pGG_IqZ6_6dX5IiN2xzywzv4R_cW-Op7lWpYfANY4ycJ8Gj60l4WEjhT8n_h_6Che?key=VReuh94fGGpJZLGsXsGdUQ)

- Permite al diseñador del sistema retrasar las decisiones sobre dónde y cómo deben prestarse los servicios.
    
- Es una arquitectura de sistema muy abierta que permite añadir nuevos recursos según las necesidades.
    
- El sistema es flexible y escalable.
    
- Es posible reconfigurar el sistema dinámicamente con objetos que migran a través de la red según sea necesario.
    

Desventajas:

Las arquitecturas de componentes distribuidos adolecen de dos grandes desventajas:

- Son más complejas de diseñar que los sistemas cliente-servidor. Las arquitecturas de componentes distribuidos son difíciles de visualizar y comprender.
    
- El middleware estandarizado para sistemas de componentes distribuidos nunca ha sido aceptado por la comunidad. Diferentes proveedores, como Microsoft y Sun, han desarrollado middleware diferente e incompatible.
    

Como consecuencia de estos problemas, las arquitecturas orientadas a servicios están sustituyendo a las arquitecturas de componentes distribuidos en muchas situaciones.

### Peer to peer (P2P)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeu0BLbI-4EXXrUzvanSJ3frbzfbKlKq1Mqf4L_rhCbb48-nw_R6sH5BY_oEf12e7aogNVG0WmR1lMZayuOoPYeEnzuLUC8lECV24QX1CYZPUIgD-xiXV13HL0dZmeRIeVQR3yI0LRFdkML_BxgbwprbkbN?key=VReuh94fGGpJZLGsXsGdUQ)

Los sistemas peer to peer (p2p) son sistemas descentralizados en los que cualquier nodo de la red puede realizar cálculos.

El sistema en su conjunto está diseñado para aprovechar la capacidad de cálculo y almacenamiento de un gran número de ordenadores conectados en red.

La mayoría de los sistemas p2p han sido sistemas personales, pero cada vez es mayor el uso empresarial de esta tecnología.

Sistemas Peer-to-peer

- Sistemas de intercambio de archivos basados en el protocolo BitTorrent
    
- Sistemas de mensajería como Jabber
    
- Sistemas de pago - Bitcoin
    
- Bases de datos - Freenet es una base de datos descentralizada 
    
- Sistemas de telefonía - Viber
    
- Sistemas de computación - SETI@home
    

  

Modelos arquitectónicos Peer-to-peer

- La arquitectura lógica de la red.
    

- Arquitecturas descentralizadas.
    
- Arquitecturas semicentralizadas.
    

- La arquitectura de las aplicaciones.
    

- Organización genérica de los componentes de una aplicación p2p.
    

- Se centra en las arquitecturas de red.
    

Arquitectura p2p descentralizada                                            Arquitectura p2p semicentralizada![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcQz17dpCAIclxJI_mqZZLXK97YeAeIawuZr0thwtze8U7Rixt56HHqhxJd2aF4ydJGBVEVVNfYeXK6aCpWIpIt00R3jKun9cakak8XgdnZIOTeOfENqUSr66agk2sF2MFZAIXUsGoIqkPacLUwZ7bcbtM9?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeWP11MKTbL2azMTtqXeqNvHlYrEOxva2mrTes9EUESLsyEay7Ua19AdE5SHzRpzqd27CLnAfTsoorkzmEV7f4kbEqvypHA5NYVfj8dKiKdS27iThxOc0DywouH29r16Agzc_y8AZHDtDPRbuABa-XsTbk?key=VReuh94fGGpJZLGsXsGdUQ)

Cuando se usa una arquitectura p2p

- Cuando un sistema es intensivo desde el punto de vista computacional y es posible separar el procesamiento necesario en un gran número de cálculos independientes.
    
- Cuando un sistema implica principalmente el intercambio de información entre ordenadores individuales de una red y no hay necesidad de que esta información se almacene o gestione de forma centralizada.
    

Problemas de seguridad en el sistema p2p

- Los problemas de seguridad son la principal razón por la que las arquitecturas p2p no se utilizan de forma generalizada.
    
- La falta de una gestión centralizada permite a los nodos maliciosos enviar spam y malware a otros nodos de la red.
    
- Las comunicaciones P2P requieren una cuidadosa configuración para proteger la información local y, si no se hace correctamente, ésta queda expuesta a los demás usuarios.
    

### Orientada a Servicios (SOA)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfTkjk23TF2Nif3ZSoV5bHNnE7fwjx9njIMC0ca92jaPe77Lm5MgeAVpsf8MaUOXfFrET43X8mPyFYGlcqpbxPhwFeOss5HKQtyjonQTx16EsXJJBV-g8H325pcTQHAeih0nLF23L1zHclQguISJS9Gmzip?key=VReuh94fGGpJZLGsXsGdUQ)

La arquitectura orientada a servicios es un enfoque para estructurar un sistema de software como un conjunto de servicios separados y sin estado, que pueden ser proporcionados por múltiples proveedores y pueden estar distribuidos.

Normalmente, las transacciones son cortas: se llama a un servicio, éste hace algo y devuelve un resultado.

La computación se consigue mediante un conjunto de componentes que cooperan y que proporcionan y/o consumen servicios a través de una red. El cálculo suele describirse mediante un lenguaje de flujo de trabajo.

Elementos:

Componentes:

- Proveedores de servicios que proporcionan uno o más servicios a través de interfaces publicadas. Las preocupaciones suelen estar vinculadas a la tecnología de implementación elegida e incluyen el rendimiento, las restricciones de autorización, la disponibilidad y el coste. En algunos casos, estas propiedades se especifican en un acuerdo de nivel de servicio.
    
- Consumidores de servicios, que invocan los servicios directamente o a través de un intermediario.
    

Los proveedores de servicios también pueden ser consumidores de servicios.

- ESB, que es un elemento intermediario que puede enrutar y transformar mensajes entre proveedores y consumidores de servicios.
    
- Registro de servicios, que puede ser utilizado por los proveedores para registrar sus servicios y por los consumidores para descubrir servicios en tiempo de ejecución.
    
- Servidor de orquestación, que coordina las interacciones entre consumidores y proveedores de servicios basándose en lenguajes de procesos empresariales y flujos de trabajo.
    

Conectores:

- Conector SOAP, que utiliza el protocolo SOAP para la comunicación síncrona entre servicios web, normalmente a través de HTTP.
    
- Conector REST, que se basa en las operaciones básicas de solicitud/respuesta del protocolo HTTP.
    
- Conector de mensajería asíncrona, que utiliza un sistema de mensajería para ofrecer intercambios de mensajes asíncronos punto a punto o publicar suscribir.
    

Relaciones:

- Fijación de los distintos tipos de componentes disponibles a los respectivos conectores.
    

Restricciones:

- Los consumidores de servicios están conectados a los proveedores de servicios, pero pueden utilizarse componentes intermediarios (por ejemplo, ESB, registro, servidor de orquestación).
    

Desventajas:

- Los sistemas basados en SOA suelen ser complejos de construir. No se controla la evolución de los servicios independientes. Hay una sobrecarga de rendimiento asociada al middleware, y los servicios pueden ser cuellos de botella de rendimiento, y normalmente no ofrecen garantías de rendimiento.
    

  

### ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdjvpfIBDS80bRrngTZuC3u1FmKcPlh0l-grlIaibqPs1JEBxTwWZtTG9SLaf6_JkDtT9O1C3lib7Tu7kgmmAr0S7n_ugT8BH9tS9moBJtp0oT2H36sZp3vivpdj2ZAeU-KiCfJXHePg2FFJvxbpQnGZp8?key=VReuh94fGGpJZLGsXsGdUQ)

### Microservicios

Este estilo de arquitectura se utiliza para implementar arquitecturas lógicas cliente-servidor donde el servidor se implementa como un conjunto de microservicios que interactúan.

Los microservicios son servicios a pequeña escala que se pueden combinar para crear aplicaciones.

Los microservicios son:

- Autónomos: no tienen dependencias externas. Gestionan sus propios datos e implementan su propia interfaz de usuario.
    
- Ligero: comunícate mediante protocolos ligeros, de modo que los gastos generales de comunicación del servicio sean bajos.
    
- Independiente de la implementación: pueden implementarse utilizando diferentes lenguajes de programación y pueden utilizar diferentes tecnologías (por ejemplo, diferentes tipos de bases de datos) en su implementación,
    
- Desplegable de forma independiente: Cada uno se ejecuta en su propio proceso y se puede desplegar de forma independiente, utilizando sistemas automatizados.
    
- Orientado al negocio: debe implementar las capacidades y necesidades del negocio, en lugar de simplemente proporcionar un servicio técnico.
    

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfZXY1ksTdVGdAAjkBs4ArOxjWg6-SrBTcHvkfZZhucOmvC-pldwmrc6PunhRnpySNd0qLZpr7nO7xG9L6Zco163Qkim_NGgyfaGAUbmfjTImZYrNQyioot1ghF_V-Y-oeuP0k8NUg_4nSLks4LPFLw7KE?key=VReuh94fGGpJZLGsXsGdUQ)  
  
  

Aplicacion Monolitica vs Arquitectura de Microservicios

Ejemplo: Servicio de impresión de fotos![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeIp-s1bikolsNN_Hl03IcVTW-uqHniZLNkaGTyq57Z7OzCjwgfcUQNKMKPlxc7rXnxHqpa8ihDEVdRqgmf5GCuT2TkndYM4Z3z7-utj3zqrkPJvEwyyFi_fN74CoqS3YDdiCaY86Be43wfu6gqW67XhDM?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfBl3PMXpIrXzTtZJy2Oh3y_gj8kSFKZPtTDbnOHB1piLMpFW-__-0aldTHJk7RsdHd3lC_9k7sTKKbWFAvBUdw0R9kGEIJ8AKr1wh352MQ3lewikgjixyjZrFqBdNBCQKZUdbhIXE_mqlCa7MYwknescpK?key=VReuh94fGGpJZLGsXsGdUQ)