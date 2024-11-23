## Caso de Uso (CU)

Un **caso de uso** es una **unidad de funcionalidad** externamente visible proporcionada por un clasificador (denominado sistema) y expresada mediante secuencias de mensajes intercambiados por el sistema y uno o más actores de la unidad del sistema.

### Propósito
Definir una **pieza de comportamiento** sin revelar la estructura interna del sistema.

### Características

- La definición de un caso de uso incluye todo el comportamiento que se le supone: las secuencias principales, distintas variaciones del comportamiento normal y todas las condiciones de excepción que pueden darse con dicho comportamiento, junto con la respuesta deseada.

- Pueden existir dependencias entre casos de uso, pero generalmente se habla de independencia.
- La especificación de un CU se da mediante los diagramas de interacción, de secuencia, etc.
- En el nivel del sistema, funcionalidades aplicadas a nivel sistema entre actores y CU.
- Un caso de uso interno se refiere a la relación entre casos de uso. Un caso de uso utiliza a otro para cumplir su funcionalidad.

### Cómo Identificar Casos de Uso
- **Por Actores**: ¿Qué funcionalidad tiene este actor?
- **Por Eventos**: Pensar en un evento y los casos de uso que tendrían que existir para ese evento.

### Descripción de Casos de Uso
La **descripción** es la secuencia de mensajes que se llevan a cabo entre el sistema y los actores para cumplir con la funcionalidad. Existen plantillas para esta descripción, cada una con un grado de especificidad:

- **Breve**: Resumen conciso de un párrafo, normalmente del escenario principal con éxito.
- **Informal**: Formato de párrafo en un estilo informal. Múltiples párrafos que comprenden varios escenarios.
- **Completo**: El más detallado, los pasos y variaciones, y hay secciones de apoyo como precondiciones y garantías de éxito. Este es el formato que solemos usar.

--- 
#### Relaciones

 **Generalización:** distintas variantes de un caso de uso ("es un tipo de"). Tiene una flecha de herencia, agrupa casos de uso con funcionalidades similares.
 
**Inclusión:** los CU no están completos sin los CU incluidos. 
- **La flecha va del lado incluido y parte del caso base.** 
- ¿Cómo represento la inclusión en un caso de uso? se representa con un "incluye nombre_casodeuso"
- Hay casos de usos abstractos y casos de usos concretos, los abstractos no pueden instanciarse por sí mismo, generalmente los bases son concretos y los incluidos abstractos
- Es la que más se usa, **se aconseja su uso cuando tenemos pasos o secuencias comunes a varios casos de uso** "algo que podemos factorizar"

**Extensión:** son utilizados de **forma condicional u opcional**, los CU están completos sin los CU extendidos.
- **La flecha va del lado del caso base y parte de las "partes extendidas"**
- Es factible hacer un extend como un camino alternativo, conviene trabajarlo como caso de uso cuando es una **recopilación de pasos bastante grande**, ya tuvimos una abstracción pero queremos congelar el resultado???¡¿
- Se utiliza mas q nada para agregar una funcionalidad, no se comparte con otros casos, justamente se la agrega pq no está

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdDpqkPTv0HIOkAoINcXh5R3GXWW-bfYsf9MaS-z1I7rRV98irViapCWyqxDwhSskUGLad24C2kOfevo0G11eapTDhJY_aQEj7lbLj0LwbAvB_bEDIESUQpSGBCbNaJV9NaiMlnlNfSy8GmpyfeVB7tpV2k?key=eC-A4tU6YurBdRY8QSa-gA)

![[Pasted image 20240804231045.png]]