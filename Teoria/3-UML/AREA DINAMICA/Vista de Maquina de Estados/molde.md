

# Diseño de Sistemas de Información

## Condición de guarda

La condición de guarda es algo que se verifica luego de que ocurre un evento, y dependiendo si la condición se cumple, las acciones se ejecutan para producir la transición de estado.

- Es una condición booleana entre corchetes referida a los atributos del objeto o a los parámetros del evento disparador, que se evalúa después de que ocurra el evento disparador de la transición.
- Solo se evalúan una vez por transición.
- Es posible tener muchas transiciones desde el mismo estado origen y con el mismo evento de disparo, siempre y cuando sus condiciones no se solapen.

## Acciones (efectos)

Una acción es un cómputo atómico y breve. Tipos:

- Una sentencia de asignación.
- Una operación aritmética.

- La invocación de una operación propia.
- Asignación de valores de retorno.
- Creación o destrucción de objetos.
- Una secuencia de acciones simples.

### Acciones específicas


## Estados avanzados y transiciones

Para modelar comportamiento más complejo que en una máquina de estado plana.

### Palabras reservadas

- `entry`
- `exit`
- `do`

No se pueden usar como nombres de eventos y etc.

### Acciones `DO`

- Se ejecutan mientras el estado esté activo. Luego de las acciones de entrada.
- Asociadas a transiciones de finalización.

### Transiciones internas

- Nunca se sale del estado, se ejecutan acciones simplemente.
- En especial cuando no quieres hacer acciones de entrada o salida.

### Diferencia entre transición interna y auto-transición

- **Auto-transición**: Un evento dispara la transición, se abandona el estado, se ejecuta una acción (si la hay), y se vuelve a entrar en el mismo estado. Como la transición sale y entra en el estado, una auto-transición ejecuta la acción de salida, después ejecuta la acción de la auto-transición y, por último, ejecuta la acción de entrada del estado.
- **Transición interna**: Queda esperando a que algo ocurra, es una transición interna cuando no se ejecutan acciones de `ENTRY` ni `EXIT`.

### Evento diferido = Deferred Event

- Escuchando eventos y aplicándolos, ante un cambio de estado se van desapilando.

## Acciones `entry` & `exit`

- Útiles para entrada (configuración inicial) o salida (limpieza final).
- Sí o sí se ejecutan, no pueden tener argumentos o condiciones de guarda.
- Sin embargo, el efecto de entrada del nivel superior de una máquina de estados de una clase puede tener parámetros, para los argumentos que recibe la máquina cuando se crea el objeto.

## Estados compuestos (subestados)

Estados que a su vez poseen varios estados. Una transición de un estado a un subestado rompe el encapsulamiento. Pueden ser:

- **Estados no ortogonales**: Un objeto puede tener un estado a la vez. Son los que más vemos. No puede haber dos estados concurrentes.
- **Estados ortogonales**: Múltiples estados simultáneos, estos tienen más sentido cuando modelamos un sistema completo.

## Estado de Submáquina

Sinónimo de `REF` en diagrama de secuencia. Sale de la idea de la máquina de estado, por lo que no lo vemos. Al estado que referencia a la submáquina se lo llama estado de submáquina.

### Vértices

- Estado
- Rombo
- `exit`
- `entry`

Los estados no son clasificadores, se llaman elementos nombrados. Notación: `nombreInstancia:nombreSubmáquina`.

### Submáquina

Una máquina de estados ser referenciada desde, dentro de otra máquina. Una máquina de estados así referenciada se denomina submáquina. Éstas son útiles para construir grandes modelos de estados de manera estructurada.
