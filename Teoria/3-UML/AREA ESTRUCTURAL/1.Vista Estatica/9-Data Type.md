
## DataType

Un **DataType** es un clasificador cuyas **instancias son identificadas por sus valores.** 

- **Diferencia con la identidad de un objeto**:
  - En un **DataType primitivo**, por ejemplo, `1` y `1` son lo mismo.
  - Dos objetos con atributos iguales, por el concepto de identidad, siguen siendo únicos.

- **Conveniencia de uso**:
  - En ciertos casos, es conveniente usar un DataType en lugar de una clase, dependiendo de si se quieren instanciar objetos únicos.

>	Ese tipo de dato pueden ser tanto clases, como interfaces o algún tipo de clasificador
### Tipos

#### PrimitiveType
- **Predefinidos en UML**:
  - `Integer`
  - `Boolean`
  - `Real`
  - `String`
  - `UnlimitedNatural`
- **Características**: Son atómicos, no tienen estructura.

#### EnumerationType
- **Definidos por el usuario**.
- **Descripción**: Conjunto de valores posibles para determinado tipo que tienen determinada semántica.
- **Ejemplo**: `ESTADO DE TRÁMITE` (`'CERRADO'`, `'ABIERTO'`).


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXd206Zp5FdTV4yoK4KbHvb-YYt2sTCEXbyibLhB0WIeRMvF0yIPsMXjK1FdCkZS4Zo7MyL9tQ3E4pTU81KmX7UR7VMHeMGIrEWHs4AcB5RCso77YjiQDgZxcPV3a9tr2HJwpL7BSRz0inAn8tnEVmwWcN8c?key=VReuh94fGGpJZLGsXsGdUQ)


---