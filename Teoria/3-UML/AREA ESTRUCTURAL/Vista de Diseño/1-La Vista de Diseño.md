
# Definicion

La vista de diseño muestra las decisiones sobre la descomposición de un sistema en unidades modulares con límites de encapsulamiento e interfaces externas. En el diseño se puede requerir conocer las partes constitutivas de un clasificador.

##### Definición en Detalle a Nivel Interno de un Clasificador
Incluye todos los conceptos y diagramas que permiten expresar que un clasificador tiene una estructura interna. Es una vista más próxima a la implementación.

### Componentes de la Vista de Diseño
Tenemos tres principales componentes:

### 1. Clases (Clasificador) Estructuradas
- **Descripción**: Clases que se descomponen en partes más pequeñas y específicas. Permiten organizar la funcionalidad interna de manera clara y modular.
- **Ejemplo**: Una clase "Orden" puede tener atributos como "id", "fecha" y "total", y métodos como "calcularTotal()" y "agregarItem()".

### 2. Colaboradores
- **Descripción**: Entidades que colaboran entre sí para cumplir una funcionalidad específica. Representan roles que objetos pueden jugar dentro de una interacción.
- **Ejemplo**: En una transacción bancaria, un "Cliente" y una "Cuenta" son colaboradores que interactúan para realizar una "Transferencia".

### 3. Componentes
- **Descripción**: Unidades modulares con interfaces bien definidas que encapsulan el comportamiento interno. Los componentes pueden ser clases, subsistemas o módulos que se comunican a través de interfaces.
- **Ejemplo**: Un componente "Motor de Pago" podría tener interfaces para "Autorizar Pago", "Procesar Reembolso", etc.

-----
### Resumen
La vista de diseño es crucial para entender cómo un sistema se descompone en partes manejables y cómo estas partes interactúan entre sí. Proporciona una base sólida para la implementación efectiva y la mantenibilidad del sistema.
