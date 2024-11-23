## IMPLEMENTACION

### Propósitos de la implementación

- Planificar las integraciones de sistema necesarias en cada iteración. Seguimos para ello un enfoque incremental, lo que da lugar a un sistema que se implementa en una sucesión de pasos pequeños y manejables.
    
- Componentes ejecutables a nodos en el despliegue, con lo encontrado en diseño
    
- Componentes que son ficheros (lenguaje de programación), cada uno es una clase o subsistema del diseño
    
- Probar los componentes individualmente, y a continuación integrarlos comparándolos y enlanzándolos en uno o más ejecutables, antes de ser enviados para ser integrados y llevar a cabo las comprobaciones de sistema.
    

Este flujo más que nada ocurre durante la fase de construcción. Aca es la programación heavy

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXflA-1j4GnGa7U5maD4MZ7bW-s4fC-bdUnQX5H0LbXgBCC0d7w3NbjvQuW7g2p4I5dPU-CsuZ0xohn54Gt0pFeCTa0Hw3xHANuDU-Ie6iFAM8Cohl8grR01bj1YN5bcXejvXDtuUTm0Y1SVe1UcWYpPdY9u?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  

### TRABAJADORES Y ARTEFACTOS![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe-QAgZHUQiDLA_yFkWhVx21m9bqNq-EHCfUX9AVCzkXozRv-WQMdwW0DPJV4QNnHkJXxxNYC_X3Gh_BV5bIrSewdc0yHYAHjrldsw9N2pP8J3KpJRqvBguC5kijXdGf5p4bJMILw?key=VReuh94fGGpJZLGsXsGdUQ)

### ARTEFACTOS

- Artefacto: Modelo de Implementación
    

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXem3HRgg9YOq0nWk6uFK5kTlHhoD03ptOYQWjFqcPE8J3rHIoEaLdBx2uh2TUXarzws7PttOLHPfs6gECfuGcCCrfgc0F6fEAi_tJyNIqNknYJhCUv76Hep-hhc75KMvq5GKS0N-7Bq0IEN6OaZEz4N5h4?key=VReuh94fGGpJZLGsXsGdUQ)

Definición: Describe cómo los elementos del modelo de diseño (ej. clases) se implementan como componentes (ej. archivos de código fuente, ejecutables).

Organización: Los componentes están organizados jerárquicamente, con un subsistema de implementación de nivel superior para estructurar el modelo en partes manejables.

  

- Artefacto: Componente
    

Concepto: Un componente empaqueta elementos del modelo (ej. clases). Existen estereotipos como ejecutables, archivos, librerías, tablas y documentos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcrq5CoXNoXtXdCze9zhz8yH4IBIjiaJ193fjnyarHbHPHlOSMZXLTdWhEV2VapW8Xt5Lxc7N7w7rBzmQJRVLVyFS9KL5NvpJZdWhSlHHOzsa7_Cey_-qtPxKDA8VbMAeSI7CwjEVQXjlf6vjhgQUs4Tw?key=VReuh94fGGpJZLGsXsGdUQ)

Características:

- Tienen relaciones de traza con los elementos del modelo.
    
- Pueden implementar múltiples clases y deben ofrecer interfaces equivalentes a los elementos que representan.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdQvHcC3BTq6Z5APNUOzGIlYZEEwf0xSCInPKg3WFYSl0uePaIlNaN21o5fQVXehKvAVsp0cXAlvgVtFN9xsjwZ5tOuwp7y5uqQBpOPvmCppqAUizTaPtAr72AmoZcTGgNNjJ9hPKOrIHAGIk5pazPZXIZ6?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfpW6GzTAuWInWbqTIkishqrA38HInkshq0tbhHkKfQGNTosYV2-RKLfkEjiZDXmwx4MYLm3mZ4btzF3kL3uFl2HCJv6LC2XKK_sQujOCQtdZjOPftF1rwgwY81J_JJ8nrFk_tQ2ftUt0jYMOZRxSI8S7q9?key=VReuh94fGGpJZLGsXsGdUQ)
    

  
  
  
  

- Dependencias de compilación indican qué componentes son necesarios para compilar otros.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfdvUL49d_u7pgyfG33ATv9OdlxJPcmM8vSZO7lLekSBo2LMJYd7LvwgUNivAVvNX5mOW3cs46C_-3onIVWkOhpVPAuN3ksunetF-mH0kJ_tVTOKxBKyL04mdhqj5BxOCGqAJOY9Qzl5QqFn5QmcZQvuu0?key=VReuh94fGGpJZLGsXsGdUQ)
    

Stubs: Son implementaciones mínimas de componentes, usadas para pruebas y desarrollo de otros componentes.

  

- Artefacto: Subsistema de Implementación![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe48aKua4Qw8pE7d7In7-e7ygTm13CyAEuxqAOnKeosp7UZFZCPY-9xp_rThK1yl_WUCEAqgP98XFGxaJsdCzg_EVH7V9wyz7mIde2GpoJleVUFbHZXG_itIdy4CNEN1GUejKVe-VMH3yyUAbTuUtjHw6A?key=VReuh94fGGpJZLGsXsGdUQ)
    

Función: Organiza artefactos en partes manejables. Un subsistema puede incluir componentes, interfaces y otros subsistemas.

Representación: Se presenta de distintas formas según el entorno (ej. paquetes en Java, directorios en C++).

  

Relación con subsistemas de diseño: Deben seguir la traza de sus equivalentes de diseño y mantener las mismas interfaces y dependencias.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXetgmMQaYqRmUTFa7RNfGkTcCPBxm7jhHEW2Xw6Et7Zofc7-aG06xrkGQZbCqCRO5-AkCHt451mL4J7XTeVxx8AI9kp9721wGU360SLYs3qjtY6bRub6fMgRdh0MVYb4VVa4YELzEA4JSTSf4bI_bEfMtI?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeqTqd2QD6Rakk2Zd9vDlxG0tGKU1C1WE4CF7RYLxPIZhuYfiiTuHAUrOF2Cb2ppL8x6gLOP3MTz5JEF9TgnKpE8h5J3Bv8RFM0rysJ4y0nk-0Ymv_dFWH9HcuHNwpKvBHENOC_k85vxqpa3p6NpHpxn2LP?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  
  
  

- Artefacto: Interfaz![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe1srKhrOChsH2D_XSTAgGYP1DeIOmAHXtM9wnaf5F6mx-xSOJ12lqoM7iq5-CkL2JCQY1HoXvZNk7XarQIwCDjyuKDB2I5H_Rb8L1UOAg2qrdiK8U2peAfFC5fY6I8FG2-TqByOw?key=VReuh94fGGpJZLGsXsGdUQ)
    

Propósito: Las interfaces especifican las operaciones implementadas por componentes y subsistemas. Un componente que proporciona una interfaz debe implementar todas las operaciones de esta.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXexZQ6MN5_zOh5F0uzCr8i0UcQwD6LHd0KCVx9VemQcFlxTJDzL_PHY9S1yHxNDNZH2pwomXr_jIHZqwZFs-TSmpbLwYsRMmK03KQuTkvq3NAylQNkXx4M5xefMJuv36t1HgDJjkfSiAw4pX5X9kKNNOHA_?key=VReuh94fGGpJZLGsXsGdUQ)

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXelL14PBCUJAJC9dnwxstZO6078hXEUh1v7T0iRjMownhl-dDuCwSJae-WXzccGGnDTNkLb6aGTDNuTzOiwsDUOYTlNg8bLUHQ1shQO1DwZxnzOmxydbhJJpp_zmgcu6-4WlsMs_WzKrXr82qRvqQfibF67?key=VReuh94fGGpJZLGsXsGdUQ)  
  
  
  
  

- Artefacto: Descripción de Arquitectura (vista del modelo de implementación)
    

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeblgyXP1rMBgarXwv6IxrgmkSftsX0KggCEfSS7GO3Loi6tDtRaaDt0h53SEx0DHaR9GZzLfrPNyH7WZPzAknhaZiSYXHpcVtiWadPT06Nexi-rO1vnQJdKtslFRZzVGSeH1XkmlWQMLo1b2L8UvonkZGM?key=VReuh94fGGpJZLGsXsGdUQ)

Contenido: Muestra los artefactos significativos en el modelo de implementación, como la descomposición en subsistemas y componentes clave.

Consideraciones arquitectónicas: Se centra en los subsistemas que siguen la traza de los subsistemas de diseño y en componentes esenciales que soportan mecanismos de diseño.

  

- Artefacto: Plan de Integración de Construcciones
    

Objetivo: Crear software incrementalmente, facilitando la integración y prueba de componentes mediante "construcciones" (versiones ejecutables). Construcciones se prueban primero y luego se avanza, sino se regresa a la versión anterior

Beneficios:

- Permite pruebas tempranas y facilita la localización de errores.
    
- Pruebas de integración enfocadas en pequeñas partes del sistema.
    

Proceso: Cada construcción añade una pequeña funcionalidad, y un plan de integración describe qué funcionalidades y componentes se incluyen en cada paso de la iteración.

  
  
  
  

### TRABAJADORES

- Trabajador: Arquitecto![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfsKQpip1khZVTGcQ7pnP52SMvIzxpWIexV_ez2N_G3kV47mHJurANibbAqKAVto6xYj9m5hVMS_jjpki6AfTIyltF07VlYgFBblS6MsnSaORn6rJLw26oBHHZt_VyF3tUtKXQ-z0DW1xQtYheSy1xTbFNZ?key=VReuh94fGGpJZLGsXsGdUQ)
    

En la fase de implementación, el arquitecto asegura la integridad y correctitud del modelo, garantizando que cumple con el diseño y los requisitos especiales. Supervisa la arquitectura del modelo (componentes significativos) y asigna los componentes a los nodos en el despliegue. No se encarga del desarrollo continuo; esto lo gestiona el ingeniero de componentes.

  

- Ingeniero de Componentes![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfhOUwc1EA7iFtwDbGFWZRsdVPbcySzmpLWs1hUDTQOyc7lKUFb_gv-YcbVv8W9fUbaZMBXZ3xj9YZf_xiLA0pC-7C_1iMJHn9SUBZpdHH51kl4ZPI41w5QFb3Rn_QVZqapXgXV5wcIESKO6iKgV7xcwBJ9?key=VReuh94fGGpJZLGsXsGdUQ)
    

Define y mantiene el código fuente de los componentes, asegurando que implementan la funcionalidad correcta. Además, mantiene la integridad de los subsistemas de implementación y es responsable del diseño y la implementación de las clases en su subsistema. Implementa los componentes e interfaces contenidos en el subsistema.

  

- Integrador de Sistemas![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdLiBs8pJg8hbVhUoy7nu3MkF-mzMUJBgiN4k1LrrD4ladSvTiqw6ZiONfjOh-1KudpqbJ92pd6sQo5u-trFAOzrZKYAh41GoDNL74syifNxv482MF54vhmGMieTlt95Ns9Y3Xi6qhb6o1ZW60SGBfmHbBt?key=VReuh94fGGpJZLGsXsGdUQ)
    

Responsable de la integración de componentes y de planificar la secuencia de construcciones en cada iteración para que el sistema funcione como un todo.

  

### Flujo de Trabajo de Implementación![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeRnvkEbVfOb2JmFdRF3wUYO2nQmfrh4VDNo0o5TnxkO3xzYfxMnVwx8f-dh_dihXCmw6ohoaKVJOW7bDDiosXcZTkqC34A0SOFEeSSr6gJ20g4gcNwRNkwltEDpTDBiPsc_y0QlwGXxgjdDEDwnyZ8QkF7?key=VReuh94fGGpJZLGsXsGdUQ)

La implementación del sistema comienza con el arquitecto, quien define los componentes clave. Luego, el integrador de sistemas planifica la secuencia de integraciones para la iteración, detallando la funcionalidad y los subsistemas involucrados en cada construcción. Los ingenieros de componentes implementan y prueban los requisitos de los componentes, que después son integrados por el integrador de sistemas. La construcción finalizada se envía a los ingenieros de pruebas de integración para su verificación, antes de iniciar la siguiente fase, considerando posibles defectos detectados.

  

#### Actividad: Implementación de la Arquitectura![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcZTItSf-q6O8sp8EWm4QaKgr6BNIEj-MobRL6rfU90zlpHW4GjIj08jJ9A_bo41zLkYw5ZYErN1BUzvX8IHYc_ItXB1_Oatbnx0VN18PUqALY0yVHYekD7kkae-KwtZeZegZ00c-wLr7uI4lawAsODZw1p?key=VReuh94fGGpJZLGsXsGdUQ)

El objetivo principal de esta actividad es crear un modelo de implementación de la arquitectura que defina cómo se distribuirán y asignarán los diferentes componentes y subsistemas de diseño a los nodos del modelo de despliegue. Este proceso involucra:

1. Identificación de Componentes Significativos Arquitectónicamente:
    

- Identificar tempranamente los componentes ejecutables y aquellos con un rol relevante en la arquitectura.
    
- Evitar profundizar demasiado en la creación de componentes menores para no duplicar esfuerzos más adelante.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXebp-oA-6lFiYAQ536Ku2xIKzmCN2zFic-Ha-ZHdJRgJWLbSBzW5w35YOmfU9Quhow-oxF4q7lRG5Z3XuzY9CohC_DQR6cke62eENS0Vz6W_clU9CqZ1_praVQMMlCx-1dGK17tFfye3k84tHL6CD6SyMep?key=VReuh94fGGpJZLGsXsGdUQ)
    

3. Identificación y Asignación de Componentes Ejecutables a Nodos:
    

- Basarse en el modelo de diseño para identificar las clases activas y asociarlas con componentes ejecutables.
    
- Asignar estos componentes a nodos en la infraestructura, lo cual permite organizar la estructura de despliegue en un nivel más detallado.
    

  
  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcHBuQdGIa9TJhHxZSxYGHhvpLSY5ce33E26MN3eUzQCvqLgHi2apiGAi4UNd3-1ZV7AdQ2LvVd-11licJd2EYfljk1_OLHEQwqv8hdx0rAfn8VGp6TMKpOjeAxN764VD3BLjfKr1bfhPia3Li92i7Qk73f?key=VReuh94fGGpJZLGsXsGdUQ)

#### Actividad: Integración del Sistema![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe2UctoNoVvDAajviRymQGBxIkKwyI3IpKVvUUMmM6l8T9OtZaIYJn6g4qKp1js5LUtVSn7B6O0Tx4WXblmB3uzLGjx4thBlXu2YozYjAHifrjQ8RiRAy-Dg_kKkNBOJ-csynQLa-aIlpHUm2gCvSe0ZcHg?key=VReuh94fGGpJZLGsXsGdUQ)

Esta actividad busca integrar las diferentes construcciones del sistema a medida que se completan las iteraciones, mediante un plan de integración adecuado y pruebas correspondientes.

1. Planificación de Construcción:
    

- Definir un plan que organice la integración de los componentes y permita una prueba de integración sobre casos de uso completos (o por partes) y/o escenarios.
    
- Evitar agregar demasiados componentes en una construcción para facilitar las pruebas e integración. Aplicación de stubs.
    

3. Integración de una Construcción:
    

- Organizar la compilación e integración de componentes en cada construcción, respetando la jerarquía de capas para evitar dependencias cruzadas.
    

#### Actividad: Implementación de un Subsistema![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe0OL6NRa6lF1dsYwzdGBXr2dk6bKgzSKZiO7f_2XEOkRLTgtirmICAj7R023QVI8kyo_Y0OBgidofFLYK0ClcqRNdaWxuSXTHYWjkJ2708HVZzVgm86rsZ3Dt4jhJMUKtAkxb4fQ?key=VReuh94fGGpJZLGsXsGdUQ)

El propósito de esta actividad es asegurar que cada subsistema cumple con los requisitos de diseño en una construcción.

1. Mantenimiento de los Contenidos de los Subsistemas:
    

- Implementar clases de diseño en los componentes del subsistema de acuerdo con las necesidades de la construcción.
    
- Refinar los contenidos del subsistema según sea necesario, incluyendo la implementación de interfaces especificadas.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc5UQyXIo3qNfiv8atDIHlve3gasOLL2yp8nHgddnDFu4XB3XmhxM2y4xGvGl_C1oK_1u03Z4IAsB8QdORvkmCw3B-xNz5iYAmXPDp3yqg6zKlPPQBXkp1-leLtWRQTwsR9uEBc-FIrOMd8EmvL9SGYvwL7?key=VReuh94fGGpJZLGsXsGdUQ)
    

El sistema resultante se pasa entonces al integrador de sistemas para su integración.

#### Actividad: Implementación de una Clase

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcKm4mHkZno-becSfaQX1NYspUBotTW98Gcj7XgS1IGq3AmzgKS-gM1T1mRIPNi1ixt7S4ATeQRgrqbDX1GZdbGlWTDhmdZs3kkpTv3rndh64MjoyUZNDHTIfzORQQg8vk_YPPRlWiz839dBdr_jpdsgKNF?key=VReuh94fGGpJZLGsXsGdUQ)

Esta actividad se centra en implementar las clases de diseño en los componentes ficheros, completando el código y las relaciones de cada clase.

1. Esbozo de los Componentes Fichero:
    

- Determinar el alcance de cada fichero y asegurarse de que cumpla con las prácticas del lenguaje en uso, por ejemplo, un archivo por clase en Java.
    

3. Generación de Código a Partir de la Clase de Diseño:
    

- Generar el código esqueleto de las clases de diseño, incluyendo atributos, relaciones y métodos, 
    

5. Implementación de las operaciones y adaptación de los detalles a las convenciones del lenguaje de programación.
    
6. Interfaces provistas en diseño también se implementan.
    

  

#### Actividad: Realizar prueba de unidad

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcmtKU_W5RlY03Fj5a0Ap0n7JsvYXVBPjl1M9IqIMZPjLBW6VAjHeyb5IUc2Cds1JC7I5zTm74NeYR4UMXltOCwKqGM1wvQ4nX_3Q8KSHUit44dQ6cKeix92z0reyILfHr7DoQvMr6zBocRKjQnDbDr8WlB?key=VReuh94fGGpJZLGsXsGdUQ)

Las pruebas de unidad evalúan componentes individuales para asegurar su correcto funcionamiento. Existen dos tipos clave:

- Prueba de especificación (caja negra): Verifica el comportamiento externo sin examinar la implementación. Se utilizan clases de equivalencia para agrupar entradas, estados y salidas similares, reduciendo el número de pruebas necesarias.
    
- Prueba de estructura (caja blanca): Examina la implementación interna, asegurando que cada sentencia y los caminos críticos del código se ejecuten al menos una vez.
    

Además de estas pruebas, es importante realizar pruebas de rendimiento y de integración para asegurar el correcto funcionamiento de todo el sistema.

  

### Resumen de Implementación

La implementación genera el modelo de implementación, que incluye:

- Subsistemas y componentes: Subsistemas con dependencias e interfaces; componentes como archivos y ejecutables, que se prueban de forma individual.
    
- Arquitectura: La vista arquitectónica muestra los elementos clave de la implementación.
    
- Despliegue: Los componentes ejecutables se asignan a nodos en el modelo de despliegue.
    

Este modelo es la base para las pruebas de integración y de sistema, donde cada componente se evalúa en etapas posteriores para asegurar su correcto funcionamiento.