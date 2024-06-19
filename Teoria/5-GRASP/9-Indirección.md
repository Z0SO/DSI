## ↩️Indirección - Indirection

This principle suggests introducing an intermediate layer of indirection (like an interface or abstract class) between closely coupled classes. This allows for easier changes and decoupling.

### Descripción
El patrón de indirección nos permite mejorar el bajo acoplamiento entre dos clases asignando la responsabilidad de la mediación entre ellos a una clase intermedia.

### Problema
¿Dónde debo asignar responsabilidades para evitar o reducir el acoplamiento directo entre elementos y mejorar la reutilización? Si sabemos que un objeto utiliza otro que muy posiblemente va a cambiar, ¿cómo protegemos a un objeto frente a cambios previsibles? ¿Cómo desacoplar objetos para que se admita un acoplamiento bajo y el potencial de reutilización siga siendo mayor?

### Solución
Asignar la responsabilidad a un objeto que medie entre los elementos para proteger al primer objeto de los posibles cambios del segundo. Esto se hace con el propósito de separar responsabilidades. La idea es que no se acoplen directamente, y que los cambios exteriores no incidan dentro del sistema.

### Beneficios
- Introducir API's externas en la aplicación sin que tengan demasiada influencia en el código.
- Facilitar el cambio de la API utilizada sin afectar el resto del sistema.
