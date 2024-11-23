

# Condición de Guarda

La condición de guarda es algo que se verifica luego de que ocurre un evento, y dependiendo si la condición se cumple, las acciones se ejecutan para producir la transición de estado.

- Es una condición booleana entre corchetes referida a los atributos del objeto o a los parámetros del evento disparador, que se evalúa después de que ocurra el evento disparador de la transición.
- Solo se evalúan una vez por transición.
- Es posible tener muchas transiciones desde el mismo estado origen y con el mismo evento de disparo, siempre y cuando sus condiciones no se solapen.

>  **Ejemplo del Libro de Martin Fowler**
>  Un ejercicio comúnmente utilizado para comprender las condiciones de guarda es el de la vela en el libro de Martin Fowler. En este ejercicio, se puede establecer una condición de guarda que evalúe si la vela está encendida antes de apagarla.


---
### Resumen

Las condiciones de guarda, acciones y tipos de transiciones son elementos esenciales en el modelado de sistemas mediante diagramas de estado, permitiendo representar el comportamiento dinámico de un sistema de manera precisa y eficiente.

