## Alta Cohesión - High Cohesion

Este principio promueve diseñar clases con un propósito claro y enfocado. Una clase altamente cohesionada tiene responsabilidades bien relacionadas que contribuyen a una sola funcionalidad.

### Tipos de Cohesión
- **Cohesión coincidente**: El módulo realiza múltiples tareas sin ninguna relación entre ellas.
- **Cohesión lógica**: El módulo realiza múltiples tareas relacionadas, pero en tiempo de ejecución solo una será llevada a cabo.
- **Cohesión temporal**: Las tareas del módulo deben ser ejecutadas al mismo tiempo.
- **Cohesión de procedimiento**: Las tareas del módulo corresponden a una secuencia de pasos del producto.
- **Cohesión de comunicación**: Las tareas del módulo afectan a los mismos datos en una secuencia de pasos.
- **Cohesión de información**: Las tareas del módulo tienen su propio punto de arranque y trabajan sobre los mismos datos.
- **Cohesión funcional**: El módulo ejecuta una sola tarea con un único objetivo a cumplir.

### Relación entre Cohesión y Acoplamiento
- Un mayor grado de cohesión implica un menor acoplamiento.
- Maximizar la cohesión intramodular minimiza el acoplamiento intermodular.
