
# Vista Estática

## Propósito
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
- **Elementos del Sistema:**
  - **Clase:** Concepto del sistema modelado.
  - **Interfaz:** Conjunto de operaciones que caracterizan un comportamiento.
  - **Tipos de Datos:** Descripción de valores primitivos que carecen de identidad.
- **Conceptos de Comportamiento:**
  - **Casos de Uso:** Especificación del comportamiento de una entidad en su interacción con agentes externos.
- **Cosas del Entorno:**
  - **Actor:** Usuario externo al sistema.
- **Estructuras de Implementación:**
  - **Componente:** Parte modular de un sistema con interfaces bien definidas.
  - **Nodo:** Recurso computacional.
  - **Subsistema.**

## Características (Features)
### Estática y de Instancia
- **Característica Estática:** Compartida por una clase y no aplicable a un solo objeto. Se usa para modelar atributos o métodos comunes a todas las instancias de una clase. En UML se representan con subrayado.
  - **Ejemplos:** Valores constantes, contar cuántas veces se instanció una clase.
- **Característica de Instancia:** Asociada a cada instancia individual de una clase. Se usa para modelar atributos o métodos específicos de cada instancia.
  - **Ejemplo:** Datos de un empleado.

### Diferencias
- **Operaciones:**
  - Característica estática determina si una operación tiene acceso a una instancia específica (no estática) o a la clase en general (estática), como un operador de creación.
- **Valores:**
  - **Estáticos:** Clasificador tiene una única copia accesible por todas las instancias.
  - **No estáticos:** Cada instancia tiene su propia copia independiente.

### Clave
- En los de instancia, primero es necesario instanciar un objeto para luego llamar a los métodos.
- En los estáticos, se puede acceder directamente al método sin instanciar un objeto.

