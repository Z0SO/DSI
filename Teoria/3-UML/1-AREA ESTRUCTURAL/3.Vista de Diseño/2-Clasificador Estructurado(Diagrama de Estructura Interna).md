
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcKiWIUZhzw9Cqln17GbpnVkEEvE4N2n3no49Ek2SxtMa6Hc_-ruFzjad4uf8eaZQsCarat-Ya6qArlPa3u2492kyNa0umdHWkjbxGjXEqVjvXggBkKVFqTpHUcyFHwFzZr9Nt1cb1arnhj9_jh7wEuhg0?key=VReuh94fGGpJZLGsXsGdUQ)

# Definicion

Un **clasificador estructurado (CE)** es un **clasificador con estructura interna.** Contiene un conjunto de partes conectadas mediante conectores.

### Características Principales

- **Estructura Interna**: Un Clasificador Estructurado tiene una estructura interna que consiste en **puertos, partes y conectores.**
- **Partes y Conectores**: Las partes son componentes del Clasificador Estructurado y están conectadas entre sí mediante conectores.
- **Partes**: Una parte es un pedazo estructural de un clasificador. Una parte describe el papel que la instancia juega dentro de una instancia del clasificador. Una parte tiene un nombre, un tipo y una multiplicidad. Cada parte puede tener un tipo. El tipo restringe el tipo de los objetos que pueden ligarse a un rol. El tipo de un objeto asociado a un rol debe ser igual que o un descendiente del tipo declarado del rol
- **Puertos**: Un puerto es un punto de interacción individual entre un clasificador y su entorno.
- **Conector**: Un conector es una relación contextual entre los objetos u otras instancias de roles en un clasificador estructurado. Define unas comunicaciones entre los roles. Un conector sólo es significativo dentro del contexto de un clasificador estructurado.
- **Instancias**: Una instancia de una clase estructurada es un objeto que contiene un conjunto de objetos correspondientes a cada parte.

### Detalles de las Partes

- **Composición**: Se habla de una parte cuando forma una composición con la clase madre que es el Clasificador Estructurado.
- **Tipo y Multiplicidad**: Una parte tiene un tipo y una multiplicidad dentro de su contenedor.
- **Pertenencia**: Un objeto que es una parte solo puede pertenecer a un objeto estructurado. Todos los objetos dentro de un único objeto estructurado están relacionados implícitamente por estar contenidos en el mismo objeto.

Este concepto simplifica el diseño e implementación del comportamiento dentro de clases estructuradas, permitiendo que las interacciones entre las partes se gestionen de manera más eficiente y coherente.
### Elementos Esenciales

- **Rol**: Cada rol tiene un nombre, tipo y multiplicidad dentro de su contenedor.
- **Nivel de Abstracción**: El nivel de abstracción más bajo en UML es un objeto.
- **Relaciones**:
  - Entre dos roles: Conectores.
  - Entre dos clases: Asociaciones.
  - Entre dos objetos: Enlaces.

---
## Ejemplos y Notaciones

- **Ejemplo de Objeto y Rol**: Un objeto "Persona" puede jugar el rol de "Customer".
- **Roles Normales y Partes**: Los roles normales son partes, como si "Ticket" tuviera una relación de composición con "Persona".
- **Roles Secundarios**: Indicados con líneas punteadas, no forman composición con la clase común y no forman parte de la clase.
- **Multiplicidad**: Por defecto, la multiplicidad es 1 del lado del tipo de objeto. Ejemplo: `seat: Seat[1..*]` indica multiplicidad de 1 a muchos.

![[Pasted image 20240618001703.png]]
## En Diagrama de Secuencia

Se utilizan roles y, para indicar que son roles, deben estar subrayados.

### Contexto

- **Clase de Contexto**: La clase `TicketOrder` (puede no ser una clase específica).






