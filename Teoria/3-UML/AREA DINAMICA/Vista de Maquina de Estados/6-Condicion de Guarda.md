

# Condición de Guarda

Una condición de guarda es una expresión booleana referida a los atributos del objeto o a los parámetros del evento disparador, que se evalúa cuando ocurre otro evento disparador. Estas condiciones son fundamentales para controlar las transiciones entre estados en un diagrama de estado.

>  **Ejemplo del Libro de Martin Fowler**
>  Un ejercicio comúnmente utilizado para comprender las condiciones de guarda es el de la vela en el libro de Martin Fowler. En este ejercicio, se puede establecer una condición de guarda que evalúe si la vela está encendida antes de apagarla.

## Acciones (Efectos)

Una acción es un cómputo atómico y breve que ocurre como resultado de una transición de estados. Estas acciones pueden incluir:

- Asignación de valores.
- Operaciones aritméticas.
- Envío de señales a otros objetos.
- Invocación de operaciones propias.
- Creación o destrucción de objetos.
- Secuencia de acciones simples.

Las acciones pueden ser cualquier método, y aunque en principio se espera que sean breves, no hay un límite específico para su duración.

## Estados Avanzados y Transiciones

Palabras reservadas como `entry`, `exit` y `do` se utilizan para definir acciones específicas asociadas a estados y transiciones. Las acciones de `do` se ejecutan mientras el estado esté activo y están asociadas a transiciones de finalización.

### Diferencia entre Transición Interna y Auto-Transición

- Transición Interna: Espera a que ocurra un evento para cambiar de estado. No ejecuta acciones de `entry` ni `exit`.
- Auto-Transición: Ocurre cuando el estado no cambia, pero se ejecutan acciones de `entry` y `exit`.

## Evento Diferido

Los *eventos* *diferidos*, también conocidos como `deferred events`, son aquellos que se escuchan y se apilan. Se desapilan ante un cambio de estado y se utilizan para gestionar la prioridad de eventos en un sistema.

## Estados Compuestos (*Subestados*)

Existen dos tipos de estados: no ortogonales, donde un objeto puede tener un estado a la vez, y ortogonales, donde pueden existir múltiples estados simultáneos. Las transiciones entre estados compuestos rompen el encapsulamiento.

## Submáquina

Una submáquina es una manera de simplificar diagramas de estado al agrupar múltiples estados y transiciones bajo un solo estado. Se utiliza para reducir la complejidad y mejorar la legibilidad del diagrama.

---
### Resumen

Las condiciones de guarda, acciones y tipos de transiciones son elementos esenciales en el modelado de sistemas mediante diagramas de estado, permitiendo representar el comportamiento dinámico de un sistema de manera precisa y eficiente.

