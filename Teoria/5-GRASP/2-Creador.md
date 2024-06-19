## 🏭 Creador - Creator

Este principio se centra en asignar la responsabilidad de crear objetos de una clase. Puede hacerlo la propia clase (método de fábrica) o una clase creadora dedicada.

### Detalles del Patrón Creador
El patrón creador nos ayuda a identificar quién debe ser el responsable de la creación o instanciación de nuevos objetos o clases.

Este patrón nos dice que la nueva instancia podrá ser creada por una clase si:
- Contiene o agrega la clase.
- Almacena la instancia en algún sitio (por ejemplo, una base de datos).
- Tiene la información necesaria para realizar la creación del objeto (es 'Experta').
- Usa directamente las instancias creadas del objeto.

#### Consecuencias y Ventajas
- **Visibilidad**: Mayor visibilidad entre la clase creada y la clase creadora.
- **Bajo acoplamiento**: Facilita el mantenimiento y reutilización del código.