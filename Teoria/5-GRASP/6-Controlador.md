## 👮‍♀️Controlador - Controller

This principle assigns the responsibility of handling system events or coordinating activities to a controller class. This centralizes control flow and simplifies interactions between other objects.

### Descripción
El patrón controlador es un patrón que sirve como intermediario entre una determinada interfaz y el algoritmo que la implementa, de tal forma que es el controlador quien recibe los datos del usuario y quien los envía a las distintas clases según el método llamado.

Este patrón sugiere que la lógica de negocio debe estar separada de la capa de presentación, lo que aumenta la reutilización de código y permite a la vez tener un mayor control.

### Pregunta Clave
La pregunta a realizarse para este patrón es: ¿Cuál es el primer objeto más allá de la capa de UI en recibir y coordinar (“controlar”) una operación del sistema?

### Características del Controlador
- Representa el sistema general, un objeto raíz, un dispositivo en el que se ejecuta el software.
- Representa un escenario de caso de uso en el que se produce una operación del sistema.
- Debería ser el primer objeto llamado después de un cambio en la interfaz de usuario.
- Controla/ejecuta un caso de uso. No hace demasiado por sí solo, controla, coordina.
- Pertenece a la capa de aplicación o a la de servicios.

### Recomendaciones
Se recomienda dividir los eventos del sistema en el mayor número de controladores para poder aumentar así la cohesión y disminuir el acoplamiento.