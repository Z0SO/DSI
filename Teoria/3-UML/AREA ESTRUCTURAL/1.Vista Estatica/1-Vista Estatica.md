# Vista Estática
- Captura la estructura de los objetos.
- Es la base sobre la que se construyen otras vistas.
- Es un modelo incremental, especialmente útil en un proceso iterativo-incremental.

## Diagrama de Clases
- **Clase:** Descripción de un concepto del dominio de la aplicación o del dominio de la solución.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXetTtIQp1w-Q8WLFnR9e4iwJGYM_AN-VvtDRzEUBC3gc3gKtTuMMfQQ8EoNOoFyGqebY5e99m_dvyHY_Xzn-wYj7WbPzwLN-D8MzPWTtoTQhOjIxywL1UTPdvwQi81pNCI5g5eWbspFBWVukCtN-v8R6E2H?key=VReuh94fGGpJZLGsXsGdUQ)

## Clasificación
### Clasificadores y sus Relaciones
- **Clasificador:** Concepto discreto en el modelo con identidad, estado, comportamiento y relaciones. Es la superclase de todos los elementos en UML.
- **Otro Concepto:** Metaclase abstracta cuyas subclases concretas se usan para clasificar un conjunto de instancias con características comunes.
  - Una característica puede ser estructural o de comportamiento.

### Tipos de Clasificadores
**Elementos del Sistema:**
  - **Clase
  - **Interfaz
  - **Tipos de Datos:** Descripción de valores primitivos que carecen de identidad.

**Conceptos de Comportamiento:**
  - **Casos de Uso
  
**Cosas del Entorno:**
  - **Actor
  
**Estructuras de Implementación:**
  - **Componente
  - **Nodo
  - **Subsistema.**

## Características (Features)
### Estática
- **Característica Estática:** Compartida por una clase y no aplicable a un solo objeto. Se usa para modelar atributos o métodos comunes a todas las instancias de una clase. En UML se representan con subrayado.
  **Ejemplos:** Valores constantes, contar cuántas veces se instanció una clase.

### De instancia
- **Característica de Instancia:** Asociada a cada instancia individual de una clase. Se usa para modelar atributos o métodos específicos de cada instancia.
  **Ejemplo:** Datos de un empleado.

#### Diferencias

**Operaciones:**
  - Característica estática determina si una operación tiene acceso a una instancia específica (de instancia) o a la clase en general (estática), como un operador de creación.
  
**Valores:**
  - **Estáticos:** Clasificador tiene una única copia accesible por todas las instancias.
  - **De instancia:** Cada instancia tiene su propia copia independiente.
  
**Modo de acceso:**
- En los De instancia, primero es necesario instanciar un objeto para luego llamar a los métodos.
- En los Estáticos, se puede acceder directamente al método sin instanciar un objeto.

---
La clasificación en UML se refiere a organizar y agrupar los diferentes elementos del modelo en categorías o tipos.

Los clasificadores son los conceptos principales que se usan para hacer esta clasificación. Algunos ejemplos de clasificadores son:

Clase: Representa un concepto del sistema que se modela, como una entidad, objeto, etc.
Interfaz: Define un conjunto de operaciones/métodos que otros elementos deben implementar.
Tipo de Dato: Describe tipos de datos básicos como números, cadenas, etc.
Caso de Uso: Especifica un comportamiento o funcionalidad del sistema.
Actor: Representa a un usuario externo o entidad que interactúa con el sistema.

Estos clasificadores pueden tener características que los describen, las cuales pueden ser estáticas o de instancia:

Características Estáticas: Son comunes y compartidas por todos los miembros de la clase. Por ejemplo, un método estático que no requiere crear una instancia de la clase para usarlo.

Características de Instancia: Son específicas para cada instancia/objeto individual de la clase. Por ejemplo, los atributos de un objeto particular.

La principal diferencia es que las características estáticas se acceden directamente desde la clase, mientras que las de instancia requieren crear un objeto específico de esa clase primero.

En resumen, los clasificadores organizan los conceptos, y sus características describen sus detalles y comportamientos, pudiendo ser comunes (estáticas) a toda la clase o específicas (de instancia) para cada objeto.

Las "características" en este contexto se refieren a los atributos, operaciones, métodos y comportamientos que definen a un clasificador (clase, interfaz, etc).
En otras palabras, las características son las propiedades y funcionalidades que caracterizan o describen a un determinado concepto o elemento del modelo.
Por ejemplo, para una clase "Persona":

Los atributos como nombre, edad, etc. serían características.
Los métodos como caminar(), hablar(), etc. también serían características que definen el comportamiento de esa clase.

Entonces, las características estáticas serían aquellas compartidas por todas las instancias de esa clase (como un método estático), mientras que las características de instancia son específicas para cada objeto individual creado a partir de esa clase.
En resumen, características = propiedades y comportamientos que caracterizan y definen a un clasificador en el modelo UML.


