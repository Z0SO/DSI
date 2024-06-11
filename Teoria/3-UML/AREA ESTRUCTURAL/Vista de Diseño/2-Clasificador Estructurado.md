
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcKiWIUZhzw9Cqln17GbpnVkEEvE4N2n3no49Ek2SxtMa6Hc_-ruFzjad4uf8eaZQsCarat-Ya6qArlPa3u2492kyNa0umdHWkjbxGjXEqVjvXggBkKVFqTpHUcyFHwFzZr9Nt1cb1arnhj9_jh7wEuhg0?key=VReuh94fGGpJZLGsXsGdUQ)


# Definicion

Un **clasificador estructurado (CE)** es un clasificador con estructura interna. Contiene un conjunto de partes conectadas mediante conectores.

## Características Principales

- **Estructura Interna**: Un CE tiene una estructura interna que consiste en partes y conectores.
- **Partes y Conectores**: Las partes son componentes del CE y están conectadas entre sí mediante conectores.
- **Instancias**: Una instancia de una clase estructurada es un objeto que contiene un conjunto de objetos correspondientes a cada parte.

## Detalles de las Partes

- **Composición**: Se habla de una parte cuando forma una composición con la clase madre que es el CE.
- **Tipo y Multiplicidad**: Una parte tiene un tipo y una multiplicidad dentro de su contenedor.
- **Pertenencia**: Un objeto que es una parte solo puede pertenecer a un objeto estructurado. Todos los objetos dentro de un único objeto estructurado están relacionados implícitamente por estar contenidos en el mismo objeto.

Este concepto simplifica el diseño e implementación del comportamiento dentro de clases estructuradas, permitiendo que las interacciones entre las partes se gestionen de manera más eficiente y coherente.

## Elementos Esenciales

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

## En Diagrama de Secuencia

Se utilizan roles y, para indicar que son roles, deben estar subrayados.

### Contexto

- **Clase de Contexto**: La clase `TicketOrder` (puede no ser una clase específica).






