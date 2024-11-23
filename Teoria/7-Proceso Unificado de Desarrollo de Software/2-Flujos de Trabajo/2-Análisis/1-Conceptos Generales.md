## ANÁLISIS

La fase de análisis en el desarrollo de software tiene como objetivo refinar y estructurar los requisitos capturados previamente, permitiendo una comprensión más precisa y detallada del sistema.

### Importancia del Análisis

1. **Refinamiento de Requisitos**: El análisis busca resolver los aspectos no tratados durante la captura de requisitos, los cuales, debido al uso del lenguaje natural del cliente, pueden haber quedado imprecisos o incompletos. Se utiliza un lenguaje más formal y técnico, adecuado para desarrolladores, para aclarar estos detalles. **COMPRENSIÓN DETALLADA**.
    
2. **Estructuración y Mantenibilidad**: El análisis permite estructurar los requisitos de manera que sean más fáciles de comprender, modificar y mantener. Esta estructura, que se basa en clases de análisis y paquetes, no depende de la estructura definida en los casos de uso, pero existe una trazabilidad directa entre ambas. Esto asegura que las diferentes descripciones de un mismo requisito se mantengan consistentes a lo largo del tiempo.

### Problemas no Resueltos en la Captura de Requisitos

1. **Interferencia, Concurrencia y Conflictos entre Casos de Uso**:  
   Pueden surgir conflictos cuando varios casos de uso compiten por recursos compartidos del sistema. Por ejemplo, "Ingresar Dinero" y "Sacar Dinero" pueden acceder a la misma cuenta bancaria, lo que puede generar problemas de concurrencia. El análisis permite resolver estos conflictos.
    
2. **Lenguaje del Cliente**:  
   El análisis permite introducir un lenguaje más formal (diagramas de estado, actividad, interacción, etc.) para detallar con mayor precisión los aspectos funcionales y no funcionales del sistema.
    
3. **Redundancias y Descomposición de Casos de Uso**:  
   En el análisis, se puede encontrar un equilibrio entre la comprensibilidad y la mantenibilidad, descomponiendo los requisitos de manera que faciliten el diseño e implementación del sistema.

### Propósito del Análisis

El propósito del análisis es resolver los problemas y ambigüedades que puedan haber surgido en la captura de requisitos, utilizando un enfoque más formal y técnico. Además, el análisis permite estructurar los requisitos de forma que sean más manejables a largo plazo, preparando el terreno para las fases de diseño y desarrollo del sistema.

### Comparación entre Modelos de Casos de Uso y Modelos de Análisis

![Cuadro Comparativo](https://lh7-rt.googleusercontent.com/docsz/AD_4nXclcRXUWs63HZ23wNA47nrmFPe-KJJ4JnqgEzpXUcl9Z7wt1IgvHH57AImoz9HSCazNraZdh669MTAhoWZt3_3lbxaSCppDW-g4c1RKrBTnijnoXT2Q03rzMVDIBnG0SlSz8rAxjDAZTFjSSmG7zZe6ub6e?key=VReuh94fGGpJZLGsXsGdUQ)

### Análisis y el Ciclo de Vida

Dependiendo del proyecto, existen variantes en cómo manejar el análisis:

- **Usar el modelo de análisis y mantenerlo**: Costoso, pero proporciona un mayor detalle.
- **Usarlo y no mantenerlo**: Común durante las primeras etapas, generalmente elegida por su simplicidad.
- **No usarlo**: Se puede optar por saltarse directamente al modelo de diseño.

### Trabajadores y Artefactos

![Trabajadores y Artefactos](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfmDrmu2V2iZbFxCAVnY7oFF2jsjf3c_P0gcmHCWOW3uGEAJJKGbezeeQd3gFj_Rul1DhFzL4466-qeLkPM3Oa_Z3ej9_6cneh-dTtt7PJD2HwLHlnX_YChR_eibVvkYlA-qTUCdDMgvC_m2CyBdAgyzhUT?key=VReuh94fGGpJZLGsXsGdUQ)

El análisis es fundamental para afinar y estructurar los casos de uso de la fase anterior. El detalle sobre cómo se maneja esto se deja para los flujos de diseño e implementación.

Durante las primeras iteraciones de la fase de elaboración, se obtienen una arquitectura más estable y requisitos más definidos.

#### Artefactos

- **Modelo de Análisis**  
   ![Modelo de Análisis](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcUExzjy09MphNwxPfXrN2jEYsAghrpedNz6qeY7_N5rO8mUTJvufYQtR3bPOz_SfAJ66UTVmswtAx1Hq5aFTDQTqr5_mzR5Lyzp2QoixvLjDjPwCo2wKhI8s7ma4HqV0MdlqtgzWrwqE4H7Z6fm1zNvAjM?key=VReuh94fGGpJZLGsXsGdUQ)  
   Se estructura jerárquicamente mediante un sistema de análisis en el nivel más alto, subdividido en paquetes que representan subsistemas o capas del diseño.  

   - **Paquetes de Análisis**: Agrupan partes manejables del sistema, facilitando la comprensión y manejo de la complejidad.
   - **Clases de Análisis**: Son abstracciones de clases del diseño, representando componentes del sistema que se refinan desde los requisitos.
   - **Realización de Casos de Uso**: Describen cómo los casos de uso interactúan mediante colaboraciones entre clases de análisis.

- **Clases de Análisis**  
   ![Clases de Análisis](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeynIrWzra1wlq0ruTE9fEFrLDqhIFd86cpI-YyF4nDYL16KEYovDFeRPR6xkZNdSB7jNp0CD7W_b8QqVgvUIWry1jDRSooKDicq_AdL8AzZcJYlhd_ZgKAVcKJnjQZwwtsJyTDlfDBGi_m-3e5QsJ3Psk?key=VReuh94fGGpJZLGsXsGdUQ)  
   Las clases de análisis representan una abstracción de las clases de diseño, enfocándose en los requisitos funcionales a un nivel más conceptual y de mayor granularidad.

   - **Responsabilidades**: En lugar de definir operaciones, las clases de análisis describen el comportamiento de forma textual.
   - **Atributos**: Están basados en conceptos del dominio del problema y son de alto nivel.

   **Estereotipos de Clases de Análisis**:  
   - **Clases de Interfaz**: Modelan la interacción entre el sistema y los actores (usuarios o sistemas externos).
   - **Clases de Entidad**: Modelan información persistente y de larga duración, como personas u objetos.
   - **Clases de Control**: Encapsulan la lógica de control, secuencias y coordinación de objetos.

- **Realización de Casos de Uso - Análisis**  
   ![Realización de Casos de Uso](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcm3ekxyn5eKLgTa0NTwIc4iFwuA_xOuw1jbS8lgb2L7smscIxCBeuuKc9oG8WLL-t2_sVCo4YlX_ecuRhYUq6qqZJw8tjTeoUKPSN9GXa4mo3EKH9nM0GOJizz9BO3dHXgxhtsX8_ohFh7n_1pIwdXyTmi?key=VReuh94fGGpJZLGsXsGdUQ)  
   Descripción de cómo se ejecuta un caso de uso en términos de clases y objetos de análisis. Incluye una traza hacia el modelo de casos de uso.

- **Componentes de los Diagramas**  
   ![Componentes](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeaZAH2V3lAOKy4tvU6nh8VtvHYRSkTExr4ZY6GgoNw8kagxEbN4xvKUn0a_fqGOjKwP2L9_GoHcZEKrkZpXUnNfnYWxPOImmvY8QjvR6fwkYlRiLHueb0JwQa20eXXiS9oApp1t9qvLxiD2cnbzz5gKd9g?key=VReuh94fGGpJZLGsXsGdUQ)  
   Se describen las relaciones entre los objetos y clases de análisis en el flujo de ejecución del caso de uso.

### Diagramas de Clases e Interacción

- **Diagramas de Clases**:  
   Muestran las clases participantes en un caso de uso y sus relaciones.
   
- **Diagramas de Secuencia o Colaboración**:  
   Describen cómo las clases interaccionan y coordinan sus operaciones.

#### TRABAJADORES

**Arquitecto**:
- Responsable de la integridad del modelo de análisis, asegurando su corrección, consistencia y legibilidad.
- Mantiene las partes significativas para la arquitectura del sistema.
- Puede delegar tareas rutinarias a otros trabajadores, pero sigue siendo responsable de la descripción de la arquitectura.
- No gestiona el desarrollo continuo de artefactos del modelo de análisis.

**Ingeniero de Casos de Uso**:
- Responsable de la creación de los casos de uso, asegurando que estos cumplan con los requisitos y se ajusten a sus descripciones.
- No se encarga de las clases o relaciones del análisis.
- También diseña las realizaciones de los casos de uso, facilitando una transición entre el análisis y el diseño.

**Ingeniero de Componentes**:
- Mantiene las clases de análisis y sus atributos, relaciones y responsabilidades.
- Es responsable de los paquetes de análisis, asegurando que sus dependencias sean mínimas y correctas.
- Si es posible, también se encarga de los subsistemas de diseño asociados al paquete de análisis.

### FLUJO DE TRABAJO - ACTIVIDADES

El proceso comienza con los arquitectos, quienes crean el modelo de análisis, identificando los paquetes principales, clases de entidad y requisitos comunes. Luego, los ingenieros de casos de uso desarrollan cada caso de uso con base en estas clases, detallando los comportamientos requeridos. Después, los ingenieros de componentes consolidan estos requisitos, asignando responsabilidades, atributos y relaciones a las clases. A medida que el análisis avanza, se identifican nuevos paquetes, clases y requisitos, que los ingenieros de componentes refinan y mantienen continuamente para ajustar el modelo.

![Flujo de Trabajo](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdFgMvP4-8r_bKvGAvDcEYq6lYMxw-E6Q2xT4_sSOxOlytthbDW4_j0bg_cNFjMgSkcT2qJsKVFaHTpKrs2ZudIMOu_QAuq16ocihJMVKxBOMV9V2bPifQFf_OpYQBhOxEh9iTPEJGPf-vt-D0KeMgbg2E?key=VReuh94fGGpJZLGsXsGdUQ)

#### Actividad: Análisis de la Arquitectura

El objetivo principal es esbozar el modelo y la arquitectura mediante la identificación de paquetes de análisis, clases evidentes y requisitos especiales comunes.

![Análisis de la Arquitectura](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfnyd5sFSzrLS-m-eGk7PBsh6Giny1D1Tr6rD-CWLhx61nKzup78XjvjIuWTE__7IH5cLxOfMUjavBy-f0WPYQ4bOq9u6XUjObnfz1TyfBqKINtrtz6vMroir21LPTAhK8xvVTn26CWapB5-or9Dm_KbLI?key=VReuh94fGGpJZLGsXsGdUQ)

**Identificación de Paquetes del Análisis**:
- Los paquetes organizan el modelo en partes más manejables y pueden definirse al inicio o conforme evoluciona el modelo.
- Se identifican basándose en los requisitos funcionales y el dominio del problema. Una forma común es asignar casos de uso a un paquete, por ejemplo:
  - Soporte a un proceso de negocio.
  - Soporte a un actor del sistema.
  - Casos de uso relacionados por generalización o extensión.

![Paquetes del Análisis](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcdRfOLPLiNMUiCPB3sdCNF7c0kKV6O-U5R-pbNHLrKyPxBHvmquDVgCBcrvBQf0er0e5pGr2M8kYSvBYSp6vuWXOkLY_7dI2DCtXTJm6aRa4KtLdkK-97WIuHjna0vgz5MPyUk3Nf-zDXTLZspNdo_-0Gr?key=VReuh94fGGpJZLGsXsGdUQ)

**Gestión de Aspectos Comunes**:
Cuando varios paquetes necesitan compartir clases, se extraen esas clases en un paquete propio o fuera de cualquier otro paquete. Posteriormente, los otros paquetes dependerán de este paquete más general. Estas clases suelen ser de entidad, las cuales se pueden rastrear hasta clases del dominio o clases del negocio.

**Identificación de Paquetes de Servicio**:
- Estos paquetes se definen más adelante en el análisis, cuando los requisitos están claros. Cada paquete agrupa clases que contribuyen a un mismo servicio. Al identificar paquetes de servicio, se deben considerar los siguientes pasos:
  - Identificar un paquete de servicio para cada servicio opcional.
  - El paquete de servicio se convierte en una unidad de compra.

![Paquete de Servicio](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfWZ2PI9F6hNTDi2Ne0pbaiNfd9hV-WbplARyM8wX2lEfB-XKUPqAqx2JfVnMorxDl2cy7LeT9JK3mpRuABebMB2KCVgrFZPEN6ceLVt-b0kGnuuU29FDMJMLwWGs4ibMapzqbZ9mlI7fkH2zRtqEED4Nvz?key=VReuh94fGGpJZLGsXsGdUQ)

**Ejemplo de Caso de Uso Opcional: "Enviar Aviso"**:
- Algunos vendedores quieren avisos automáticos cuando se emita una factura atrasada, mientras que otros prefieren recibir la notificación y decidir si envían un aviso. Esta variabilidad se representa mediante dos paquetes de servicio opcionales y mutuamente exclusivos:
  - **Avisos Automáticos**: Para los avisos automáticos.
  - **Avisos Manuales**: El vendedor decide si contacta al comprador.
- Si un vendedor no desea este servicio, no se entrega ninguno de los paquetes con el sistema.

Cuando un servicio es opcional, el sistema debe estar diseñado para ofrecer una flexibilidad que permita que los paquetes puedan ser activados o desactivados según las necesidades de cada cliente.

**Dependencias entre Paquetes**:
- Se definen dependencias entre paquetes cuando están relacionados. El objetivo es conseguir paquetes que sean relativamente independientes pero que tengan alta cohesión interna, lo cual facilita el mantenimiento y reduce las dependencias entre los mismos.

![Dependencias entre Paquetes](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfs4S79JfATUkBY9V5t5aGm9t0q7LvzjIgfyBE0kUJVAzJLoH9RgDXdTFCtsZGx5h-1qYk021yIN3PBOeHmR5LQiGIlIm2JztJ0L9_tA5u6_I8hCfuCW_gO2V7CEuDvYY5VuQE73GGWluipmbxzyBJXJ7lI?key=VReuh94fGGpJZLGsXsGdUQ)

**Identificación de Clases de Entidad Obvias**:
- En esta etapa, se proponen preliminarmente las clases de entidad más importantes (aproximadamente entre 10 a 20), basadas en las clases del dominio o en las entidades del negocio identificadas previamente. Es importante no sobrecargarse con detalles en esta etapa, ya que muchas clases surgirán a medida que se realicen los casos de uso.

**Identificación de Requisitos Especiales Comunes**:
- Los requisitos especiales comunes surgen durante el análisis y es crucial documentarlos para su tratamiento en las siguientes fases (diseño e implementación). Estos deben ser identificados y documentados por el arquitecto para facilitar el trabajo posterior. Ejemplos de estos requisitos incluyen:
  - Persistencia.
  - Distribución y concurrencia.
  - Características de seguridad.
  - Tolerancia a fallos.
  - Gestión de transacciones.

# Análisis de Casos de Uso y Clases de Análisis

## Actividad: Analizar un caso de uso

### Refinamiento de casos de uso usando clases de análisis
![Refinamiento de casos de uso](https://lh7-rt.googleusercontent.com/docsz/AD_4nXePaJ60vf7ZFBhnA6zA9vGYk8yGIZMv3DrlsudggYvIsYmom2ckHpB_ah-oSMdIh7H2UKEwH6yMmyKKQB9Sr9Tc4M1OmOX1ma14c24cbxweLQSBuJjfPMLUFJXtdkj3j63YgvVN3z7KKCXw4v61wk6fzP9P?key=VReuh94fGGpJZLGsXsGdUQ)

#### 1. Identificación de clases de análisis

Las clases de análisis son fundamentales para comprender cómo se llevará a cabo el flujo de los requisitos en un caso de uso. Aunque en muchos casos los detalles no están completos, las clases de análisis se identifican a través de las siguientes normas generales:

- **Clases de entidad**: Representan el modelo de dominio y la descripción de los casos de uso. Algunos elementos podrían tratarse mejor como atributos.
- **Clase de interfaz central**: Se asigna por cada actor humano que interactúa con el sistema. Es una refinación de la interfaz primitiva.
- **Clase de interfaz primitiva**: Representa a cada clase de entidad que interactúa con un actor.
- **Clase de interfaz de sistema externo**: Se asigna a cada actor que es un sistema externo (software o hardware).
- **Clase de control**: Controla el tratamiento y la coordinación de las interacciones. En casos simples, este control puede delegarse a la interfaz.

Se recomienda utilizar un **diagrama de clases** para representar estas interacciones.

#### Descripción de interacciones entre objetos del análisis

**Objetivo**: Describir cómo interactúan los objetos del análisis en un caso de uso mediante diagramas de colaboración.

##### Diagramas de Colaboración
- Representan instancias de actores y objetos del análisis.
- Es recomendable crear un diagrama por cada flujo o subflujo del caso de uso.
- El flujo de interacciones debe comenzar con un mensaje de un actor hacia un objeto de interfaz.
- Cada clase de análisis debe tener al menos un objeto en el diagrama; de lo contrario, puede ser superflua.
- Los enlaces representan asociaciones entre clases del análisis y deben reflejarse en el diagrama de clases correspondiente.
- La secuencia de interacciones no es el objetivo principal; es más importante mostrar las relaciones y requisitos entre objetos.

##### Relaciones entre Casos de Uso
- El diagrama debe incluir todas las relaciones relevantes, como especializaciones de otros casos de uso.
- En casos complejos, se pueden agregar descripciones textuales como complemento.

#### Captura de Requisitos Especiales
Recoger requisitos no funcionales es crucial para la realización de un caso de uso y deben ser considerados en las fases de diseño e implementación.

---

## Actividad: Analizar una clase
![Análisis de clase](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfaYe7xGyEI2P6vuBcN-CyK_-KCmm53OJB-o7GUvhm8yIj13NRaHQv2K-B9JGER3Rn7nVkLUuDRUKRqBbyJVricMfhw6kfVB_R39BYDXyyOoMMBSiJ8OwguBefKS38lGBHG_64pmr4XUFyv2CNQPyqOoJc?key=VReuh94fGGpJZLGsXsGdUQ)

### Objetivos: Identificar responsabilidades, atributos, relaciones y requisitos especiales de una clase.

#### Identificación de Responsabilidades
- **Combinar roles**: Identificar todos los roles que cumple una clase en los casos de uso.
- **Estudiar diagramas de clases**: Revisar los diagramas de clases e interacción para determinar en qué casos de uso participa la clase.
- **Consultar artefactos de flujo de sucesos**: Estos artefactos pueden proporcionar requisitos textuales que ayudan a identificar responsabilidades.
  
Técnicas de recopilación:
- Extraer las responsabilidades de manera secuencial.
- Modificar o añadir responsabilidades según los cambios en las realizaciones de los casos de uso.

![Identificación de responsabilidades](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdxQ1bscHWkvV3SD98s0aGNRiYESJwzXzUtQMIbI6Fx8Vl4hazxOI3U-gltc745FPMH_EOtVW_RzLL8UOU_0yjmTib7T0JE335TBuVCbb4HALjECrnapZKBrCDeL9c25U0ky-NM1iZ4Xj5snRxlxmfOm9Gn?key=VReuh94fGGpJZLGsXsGdUQ)

#### Identificación de Atributos

Un **atributo** es una propiedad que define a una clase y es esencial para cumplir con sus responsabilidades. Para identificar atributos de manera efectiva, se deben seguir las siguientes normas:

- **Nomenclatura**: El nombre de un atributo debe ser claro y conciso.
- **Tipo conceptual**: El tipo de los atributos debe ser conceptual, no restringido al entorno de implementación.
- **Reutilización de tipos**: Se deben reutilizar tipos existentes cuando sea posible.
- **Claridad**: Si los atributos son difíciles de comprender, se puede crear una clase separada para ellos.
- **Clases de entidad**: Los atributos son evidentes en clases de entidad, y pueden identificarse a través de clases del dominio.

#### Identificación de Asociaciones y Agregaciones

Las asociaciones entre clases se representan en los diagramas de colaboración, reflejando cómo interactúan los objetos del análisis.

- **Proceso de identificación**: Estudiar los enlaces en los diagramas de colaboración para determinar las asociaciones necesarias.
- **Minimización de relaciones**: Reducir las relaciones innecesarias.
- **Modelar solo las relaciones necesarias**: Las relaciones deben ser lo más simples y necesarias posibles.

#### Identificación de Generalizaciones

Las **generalizaciones** se utilizan para extraer comportamientos comunes entre varias clases, simplificando el modelo y mejorando su comprensión.

- Mantener un nivel alto y conceptual en las generalizaciones.
- El objetivo es hacer que el modelo sea más fácil de entender, destacando similitudes entre clases.

#### Captura de Requisitos Especiales
Recoger los requisitos especiales, especialmente los no funcionales, es crucial para la fase de diseño e implementación de las clases del análisis.

# Análisis de Paquetes y Clases en el Desarrollo de Software

### Actividad: Analizar un Paquete

![Análisis de Paquete](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdoYTt_zAKM5EFqKr02VDf8wxedfQvE11D3FFp5CW01cSJ3E_OjDrdjWP8W2phM6lIYcCrVGdQVQKd3BAV5jsVrxNgau60YGo8IHZyIVMhWyrHVAFpcNEZJYDLipKInfOmZrWxZBZ9lfsfLgsh0-gwy9gkg?key=VReuh94fGGpJZLGsXsGdUQ)

#### Objetivos clave:

- **Independencia de Otros Paquetes**: Asegurar que el paquete sea lo más independiente posible de otros paquetes. Esto facilita el mantenimiento y reutilización del paquete. Se busca **bajo acoplamiento** para promover la modularidad.

- **Cumplimiento de Objetivos**: Verificar que el paquete cumpla su propósito, ya sea implementando clases del dominio o satisfaciendo casos de uso específicos.

- **Descripción de Dependencias**: Documentar las dependencias del paquete para estimar el impacto de futuros cambios. Esto es clave para la planificación y gestión de riesgos durante el ciclo de vida del software.

#### Normas Generales para el Análisis de Paquetes:

- **Definir relaciones entre paquetes**: Establecer claras interacciones entre diferentes paquetes.

- **Cohesión del Paquete**: Asegurar que los elementos dentro del paquete sean altamente cohesivos, es decir, que tengan una fuerte relación entre sí.

- **Limitación de Dependencias**: Mantener un bajo acoplamiento entre los paquetes, lo que facilita cambios sin que se afecten otros componentes del sistema.

![Paquete de Análisis](https://lh7-rt.googleusercontent.com/docsz/AD_4nXealp_LY4FRxGDHHL33fddjhxb3xFNVMMLJxLds7a3ZkvBwFU-bxnIPyMyj2Oc3WXyNE-nYApqwkkwLlRCbaeLTAh60DHDEL0br40oKwncYlPOXuRR6C0qdZ2R-KmSS620FKqZq9C4A-lkzXq7GCjSzO3YA?key=VReuh94fGGpJZLGsXsGdUQ)

---

### Resumen del Análisis

El **flujo de trabajo del análisis** culmina en el **modelo de análisis**, que tiene como objetivo refinar y estructurar los requisitos. Este modelo incluye los siguientes elementos clave:

- **Paquetes del Análisis**: Ayudan a aislar los cambios en los procesos del negocio y en los casos de uso, lo que facilita la gestión de estos cambios.

- **Paquetes de Servicio**: Aíslan los cambios en servicios específicos, promoviendo la reutilización de componentes dentro del sistema.

- **Clases del Análisis**: Definen las responsabilidades y las relaciones entre los componentes del sistema.

- **Clases de Control**: Son las encargadas de coordinar la lógica de negocio, asegurando que los procesos del sistema se realicen de acuerdo con las reglas establecidas.

- **Clases de Entidad**: Gestionan la información persistente, es decir, aquellas que representan datos que deben ser almacenados a largo plazo, como registros de base de datos.

- **Clases de Interfaz**: Se encargan de manejar las interacciones con los usuarios o con otros sistemas, funcionando como un punto de comunicación entre el sistema y los actores externos.

- **Realizaciones de Casos de Uso-Análisis**: Refinan los casos de uso y ayudan a aislar los cambios que pueden ocurrir durante el desarrollo del sistema.

- **Vista de la Arquitectura**: Proporciona una visión general del sistema y ayuda a identificar posibles cambios en la arquitectura a medida que se avanza en el diseño.

#### Influencia en el Diseño

El modelo de análisis tiene una **gran influencia** en el diseño del software, ya que:

- **Relaciona paquetes de análisis con subsistemas de diseño**, asegurando que la estructura del software sea coherente con los requisitos.

- **Guía el diseño de clases**, abordando específicamente los requisitos especiales que puedan haber surgido durante el análisis.

- **Sirve como base para las especificaciones de casos de uso**, detallando cómo cada caso de uso debe ser implementado en el sistema.

- **Provee una vista arquitectónica** que asegura trazas relevantes entre modelos, facilitando la evolución del software de manera coherente y estructurada.

Este enfoque sistemático permite un desarrollo de software **coherente** y **estructurado**, lo que facilita tanto el mantenimiento como la evolución del sistema a lo largo del tiempo.
