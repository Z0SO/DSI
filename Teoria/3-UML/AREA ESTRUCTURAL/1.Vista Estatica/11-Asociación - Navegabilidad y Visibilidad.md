
---
## Asociación: Navegabilidad


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdKW_2ktrcGksBKOHpmkXyrPjHcos3a-Hy6XAw7Y2er0as-TJ4JQjSFKL9vDOIoWI0i1yKOVPaQnsvUD9crMfTkfP4J_Wc2fIedqIhVXo4W1ak5GZ-ku4QS6W9UU83dKuGAqnyEKKxmUiW8ppYY8iEdauhM?key=VReuh94fGGpJZLGsXsGdUQ)


**Navegabilidad**: Indica la dirección en que los objetos de una clase pueden acceder a los objetos de otra clase a través de una asociación, en tiempo de ejecución.
### Conceptos Clave

  - *Dirección de conocimiento*: En la imagen de arriba, pedidos CONOCE A productos, no al revés.
  - *Adorno de un extremo de asociación (association end)*: `> <`
  - *Relaciones binarias*.

### Ventajas de No Usar Navegabilidad Bidireccional en Todo

- **Reducir Complejidad**: Facilita la comprensión del modelo.
- **Seguridad y Eficiencia**: Mejora el control sobre el acceso a los objetos.
- **Mantenibilidad**: Hace el código más fácil de mantener y entender.

### Diferencia entre Navegabilidad (*Navigability*) y Posesión (*Ownership*)

- **Navegabilidad (Navigability)**: Permite acceder a objetos de otra clase.
- **Posesión (Ownership)**: Indica que una clase contiene o posee instancias de otra clase.

#### Relaciones entre Navegabilidad y Posesión

- **Pertenencia o Posesión implica Navegabilidad**.
- **Navegabilidad no implica Pertenencia**.

### Asociación en Detalle

- **Asociación**: Implica que tengo una referencia de un objeto de una clase dentro de otra.
  - Ejemplo: Hay una instancia de una clase dentro de la otra (PUNTEROS).

#### Notación

- **Punto (.)**: Indica pertenencia o posesión.
  - `(a).<->.(b)`: Significa que `(a)` tiene una instancia de `(b)` como atributo, y viceversa. Además de ser navegable.
  - **Con punto**: Instancias pertenecen al clasificador.
  - **Sin punto**: Instancias pertenecen a la asociación.
  - Ejemplo: `(a)<->.(b)` aquí `(a)` pertenece a la asociación.

### Convención en la Cátedra

- **Flecha (->)**: Se usa para indicar tanto navegabilidad como propiedad (en el sentido clásico).
- **Cruz (x)** y **Punto (.)**: No se usan salvo que se indique lo contrario.
- **Navegabilidad implica Pertenencia**: Según la convención de la cátedra, aunque teóricamente no es así.
### Casos Posibles

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdQyZHjGZy_2AMfoU_t-sooxa4_t2eiqGft27eNHy5meKFgUTkWLD9Hrd8m1ndIlwdr4dHJ_Jha81u0_CvS3-bxja4pgtPyJqE12iT6Kbb5ncGQ-RbobhB-UxKfQvxcm6xUqkCMwkoAQluKDnWqkQo6XoU?key=VReuh94fGGpJZLGsXsGdUQ)


## Asociación: Visibilidad

### Conceptos Clave

- **Visibilidad**: Limita el acceso a través de la asociación en relación con los objetos fuera de la asociación.
  - **Público (`+`)**
  - **Privado (`-`)**
  - **Protegido (`#`)**

### Notación

- Se representa con símbolos:
  - **Público**: `+`
  - **Privado**: `-`
  - **Protegido**: `#`

- **Privado**: Indica que los objetos del extremo no son accesibles por ningún objeto fuera de la asociación.
  
### Comportamiento por Defecto

- Cuando no se declara explícitamente la visibilidad, todos los extremos de la asociación son **públicos**.


###### Ejemplos

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXc_npPeSI43YX1z7aL7S0xbv3P9tvwbU3o8aZLW24BWN9N9UY3bhr9g2nvPtFjZbWxV0LNDODW0mzPGbUatn_odmV5GkLZrVsKIG-Iw7MakVlI5_xc5qhGc4O1mF7m6Doc5G6-P32HA-wMJerYmZ0ycgLSZ?key=VReuh94fGGpJZLGsXsGdUQ)


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXePTpwIVuyjHyOGyJhUh-mGhc4Ui6d5IXCy7Rcu2W_Jpb2452mC1GkNLMbEo7QTExroeH2ju1xU3u59g8r_ODMlvPe3lFZD2KWxHtu5X_9X6ziIraOFFTL7NjuE751hAy6KTR6CimFkZYcJHN9iE7RItQGZ?key=VReuh94fGGpJZLGsXsGdUQ)



---