
---

# Eventos

Un evento es una ocurrencia significativa que tiene una localización en tiempo y espacio. Representa un estímulo o acontecimiento que ocurre en un punto específico en el tiempo y no tiene duración. Es importante diferenciar los eventos de las señales:

- **Evento**: Ocurre en un punto específico en el tiempo y puede ser interno o externo al objeto.
- **Señal**: Es un tipo de clasificador que vehicula la comunicación entre objetos de manera explícita, asincrónica y con nombre.

## Tipos de Eventos

### Externo
Proviene de fuera del objeto y puede ser, por ejemplo, una interacción del usuario como un clic en un botón.

### Interno
Ocurren dentro del objeto, como el cambio de estado de un temporizador en un dispositivo electrónico.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXe8FWGwisIjBBImEwRh_-hK2ivg5iaH95lu5Jc6YVxknE2d-sldtxvwXtoB4n0BJYhX15lsdjuoK3ziNHhI9Jy2mO1LshtW_wpD3Uyifv6xaUWtpzLnt_umpl2PHg5vAMYzoDZm1t-LuVr1-s3q9abtZwQ?key=VReuh94fGGpJZLGsXsGdUQ)

> **Nota de la Imagen:** Donde PUSH es Interno y POP en una Lista.

### Eventos de Señal
Representan la recepción de una comunicación asincrónica y explícita entre objetos, como un evento de un formulario.

### Eventos de Llamada
Son peticiones explícitas y síncronas donde un objeto invoca un método de otro objeto y espera una respuesta inmediata, como las operaciones push y pop en una lista.

### Eventos de Cambio
Representan un cambio en el valor de una expresión booleana y se disparan automáticamente cuando se cumple una condición lógica, como solicitar que un usuario sea mayor de 18 años.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcLU-Ef0Dmw3N7UPSi_TkjTcl3_oFHGxMAj1d9ww5GnWpuOHoCYBZFJffEZ0KxzpUNDEjAC0eGtwZQvd86n-5FVn6utwSfDUgtoihOB-ujwkRsh9Vr9wxNHyGNsEGLSRVUhEAiaSeHGUNzOfxyh6p7lxQlE?key=VReuh94fGGpJZLGsXsGdUQ)


### Eventos de Tiempo
Representan la llegada de un tiempo absoluto o el transcurso de una cantidad relativa de tiempo, como realizar una tarea a una hora específica o después de cierto lapso.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXf-GpqZYvLKhEctsEx-ALpvvHONIlUa0m3oNLZKT3Ig8GAHypaDEtP17TrEfMtkV7_ztmOpOMsNaCvRfl4CVbrIeD4n7NcTJDSmpgyhdBtP6zy9ldxxVa8CsNK2GGomA5Oof6yjtDMjzaFJWsvALLYwGto_?key=VReuh94fGGpJZLGsXsGdUQ)

## Comparación con Condiciones de Guarda

### Condiciones de Guarda
Son verificaciones que se realizan antes de permitir una transición, evaluándose en el momento de la transición.

### Eventos de Cambio
Se monitorean continuamente y se disparan automáticamente cuando la condición se cumple, provocando una transición.

Los eventos son fundamentales para modelar el comportamiento dinámico de un sistema, permitiendo definir cómo responde a estímulos y condiciones específicas.


## Estos eventos puede modelarse con Clases y Jerarquías

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfG_gEjWISDqudl3UyXXSpnV3Peqv4546wawkUmbzHlrZoKu1Pl-TFO4ksVTkw4gg3PPtD4tS29_wArob6qSJ7ZfWlJbgKimUMJCNIfO31mTe3NbFq2H4a20YSNQ8oSzLQM7z4zIZRU28LPPf8q6BzYe_Q?key=VReuh94fGGpJZLGsXsGdUQ)

> **Comentario de la Imagen** 
> - *Italica*   = Abstracto
> - Normal = Concreto

---


> Los eventos son ocurrencias significativas en el tiempo y espacio que pueden ser internas o externas a un objeto. Existen varios tipos, como eventos de señal, de llamada, de cambio y de tiempo, cada uno con características y usos específicos en el modelado de sistemas.
