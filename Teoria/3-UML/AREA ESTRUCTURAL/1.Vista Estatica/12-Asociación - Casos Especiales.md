
### Clase de Asociación

#### Descripción
- **Propósito**: Asignar atributos y operaciones a una asociación para hacerla única.
- **Identidad**: La asociación pasa a tener identidad.
- **Instancia Única**: Cada enlace tiene una instancia única de la clase de asociación.
- Desaparecen si un enlace se borra

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdGCzst-2zVK4Zntq_yA0XhV1jEzW9joZPN4QM1rotce-N8fceE314gl6iFBN7vj6XKw1bWQOBfk_bKTgwSSuJTjQ0wEmGCTG9xyxT9WeKDs1jybbgIranoemDeUYAPoZlM9_pNr3-2G0qyIghCpwRMzPVA?key=VReuh94fGGpJZLGsXsGdUQ)

### Relación Ternaria

#### Descripción
- **Diferencia**: A diferencia de la clase de asociación, las clases en una relación ternaria son independientes y no desaparecen si un enlace se borra.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdb2ND3auxZLnUqseB1OJ5WuBE2SVr9JLIdb24XYWvt7tEZDf0Kcq2jvIb6TF6Uz-rbZ5Tmyu5TPJt4BZeXznX-CFeEFpFKEJgHzg6Wyd0vKq61cTv30suTLEzffVacsN0YmhR8Ur41uBYyQrPADlkLo8vq?key=VReuh94fGGpJZLGsXsGdUQ)

### Asociación N-aria

#### Descripción
- **Navegabilidad**: No existe.
- **Multiplicidad**: Sí existe.
- **Participación**: En un enlace, todas las clases participan.
  
#### Ejemplo en PlantUML
```plantuml
@startuml
class Customer {
}

class Product {
}

class Order {
}

Customer "1" -- Order
Product "1..*" -- Order
Order "0..*" -- Customer
Order "0..*" -- Product
@enduml
```

### Asociación Calificada

#### Descripción
- **Descripción**: Ranura para un atributo o lista de atributos en una asociación binaria.
- **Implementación**: Generalmente con algún tipo de colección indizada.

###### Ejemplo

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcPbOFY1DSYUgmpD_oVNjHK_YKGLISFydbaAhjSr4P8FkiBJUwbrd6htzAfgxMl-K4596KuJGDTPEYT9AKwbOBbu_cNOydMfaE4sq6J26FdiP4Islz3U6v-Wo6qTxzUfU_IBIrlfVGES3RyRYf3u_DHx_E?key=VReuh94fGGpJZLGsXsGdUQ)


### Asociación Ordenada

#### Descripción
- **Propósito**: Reforzar la unicidad de los enlaces.

###### Ejemplo

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdY11CaWQA-lRZoADZKls4ioIBLpeMQZc56UVOECkfBhYn39NvR86h3T3yOEwSub1CCesJYiOCla7SgcMbG0fYB1O6veaSrukceAonEut5eYbbO38P15YwK-HDSYbWTkYuuJm47yrBMa5zUAkwRroCEL2U?key=VReuh94fGGpJZLGsXsGdUQ)

### Asociación con Restricción

#### Descripción
- **Cobertura**: Un objeto de una clase se asocia con otro objeto de una clase u otra mediante un `xor`.

###### Ejemplo

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdUgfRMSI0UbiY32sTMvvRHVa7vBHbQR3K2836PAli3u68qO1aCl1m_VO9c844gDU4X9_mBB2nDzMz--f_hZRUtUzUCPx4PaQftIZ1LRWgQ2BiAX-MX1gwxG0Oe4rOpW5IFBDwfMATiP2TULMn1uChQVdE?key=VReuh94fGGpJZLGsXsGdUQ)
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdsDZNaN7y9EsByl1z0jtIvVfgpGwd3pF0ceIMHErAlZxr5NqNx2nTvLXwlz2mm-Woh_-jnqWs56zDi-wuV167cHUaRPxMaJAkgk0O4Y72zoBGAgU7yWHL1nAywpSbzNmj2S4esoMAjcM_5l_1FKJbDhRk?key=VReuh94fGGpJZLGsXsGdUQ)

---
### Asociación Calificada

Una **asociación calificada** es una asociación que usa un "calificador" para restringir la relación entre dos clases. El calificador es un atributo o conjunto de atributos que ayudan a identificar de manera única una instancia de la clase destino desde la clase origen.

- **Ejemplo**: Imagina un sistema donde un `Cliente` puede tener múltiples `CuentasBancarias`. Para encontrar una cuenta específica del cliente, puedes usar el número de cuenta como calificador.

  ```plaintext
  Cliente 1 --- 0..* CuentaBancaria
           |(númeroDeCuenta)
  ```

  Aquí, `númeroDeCuenta` es el calificador que ayuda a encontrar una `CuentaBancaria` específica para un `Cliente`.

- **Características**:
  - Ayuda a identificar de manera única una instancia en el extremo destino de la asociación.
  - No añade atributos propios ni métodos a la relación, solo califica la búsqueda.

### Clase de Asociación

Una **clase de asociación** es una asociación que, además de representar una relación entre dos clases, también tiene sus propios atributos y métodos. Es una combinación de una asociación y una clase.

- **Ejemplo**: Imagina que en un sistema académico, una `Asignatura` y un `Estudiante` están relacionados mediante una clase `Inscripción`, que tiene atributos como `fechaDeInscripción` y `notaFinal`.

  ```plaintext
  Estudiante 1 --- Inscripción --- * Asignatura
                   |    fechaDeInscripción
                   |    notaFinal
  ```

- **Características**:
  - Puede tener sus propios atributos y métodos, además de los atributos de las clases relacionadas.
  - Representa no solo la existencia de una relación, sino también propiedades y comportamiento asociados con la relación misma.

### Diferencias Clave

1. **Propósito**:
   - **Asociación Calificada**: Se usa para identificar de manera única una instancia específica en una relación.
   - **Clase de Asociación**: Se usa para añadir atributos y métodos a la relación misma, no solo para identificar instancias.

2. **Atributos y Métodos**:
   - **Asociación Calificada**: No tiene atributos propios ni métodos. Solo utiliza un calificador para restringir la búsqueda.
   - **Clase de Asociación**: Tiene sus propios atributos y métodos que describen la relación.

3. **Representación en UML**:
   - **Asociación Calificada**: Se representa con un pequeño rectángulo en el extremo de la asociación, conteniendo el calificador.
   - **Clase de Asociación**: Se representa como una clase normal unida a la línea de la asociación, indicando que la relación tiene atributos y posiblemente métodos.

### Ejemplo en UML

1. **Asociación Calificada**:

   ```plaintext
   Cliente 1 --- 0..* CuentaBancaria
            |(númeroDeCuenta)
   ```

2. **Clase de Asociación**:

   ```plaintext
   Estudiante 1 --- Inscripción --- * Asignatura
                    |    fechaDeInscripción
                    |    notaFinal
   ```

En resumen, una **asociación calificada** se utiliza para identificar instancias específicas de una relación, mientras que una **clase de asociación** se utiliza para modelar una relación que tiene sus propios atributos y métodos.