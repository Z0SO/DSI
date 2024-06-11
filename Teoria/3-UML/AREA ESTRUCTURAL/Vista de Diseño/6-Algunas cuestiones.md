
# Diferencias y Similitudes con las Clases en UML 2.X

## Clases

- **Aspectos Estáticos**: Modelan los aspectos estáticos de un sistema.
- **Características**: Definen atributos y operaciones.
- **Relaciones**: Pueden tener relaciones como asociación, herencia, dependencia, etc.

## Componentes

- **Unidades Ejecutables**: Representan un conjunto de clases relacionadas que componen una unidad ejecutable.
- **Interfaces**: Tienen interfaces proporcionadas y requeridas.
- **Modularidad y Desacoplamiento**: Son modulares y pueden ser sustituidos por otros componentes que cumplen con las mismas interfaces.
- **Relaciones**: Se conectan a otros elementos del modelo mediante relaciones de interfaz, atributos y operaciones.

## Similitudes

- **Interfaces**: Ambos pueden tener interfaces y conectarse a otros elementos del modelo por medio de relaciones.
- **Atributos y Operaciones**: Las clases que componen los componentes tienen atributos y operaciones que definen su comportamiento y características.

## Relaciones entre Componentes y Artefactos

- **Diseño e Implementación**: Se puede diseñar un sistema utilizando componentes y luego implementar estos componentes utilizando artefactos.
- **Sistema Ejecutable**: En un sistema ejecutable, se pueden usar artefactos que implementen componentes que conforman o proporcionan una interfaz.
- **Extensión del Sistema**: Es posible extender el sistema haciendo que los componentes proporcionen nuevos servicios a través de otras interfaces.

## Instanciación de Componentes

### ¿Qué implica que un componente pueda ser instanciado directa o indirectamente?

- **Instanciación Directa**: Se produce cuando se crea una instancia del componente en la misma ubicación física en la cual se utiliza.
- **Instanciación Indirecta**: Ocurre cuando se crea una instancia del componente en otra ubicación y se utiliza a través de alguna conexión.

### ¿Qué significa que un componente pueda ser instanciado?

- **Utilización en Tiempo de Ejecución**: Significa que el componente puede ser utilizado por otros componentes, conectándose mediante sus interfaces y siendo utilizado en tiempo de ejecución.
- **Copia al Instanciar**: Al ser instanciado, se crea una copia del componente.

### Convergencia de Puertos

- **Convergencia de Puertos**: Este concepto implica que los puertos de un componente pueden unirse y trabajar conjuntamente, facilitando la comunicación y la interacción entre diferentes componentes en el sistema.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfRIkRDtpr67xz5T5GLNTZ8FpSSMjgs7KbCf6dKitAP-YTg-8naVswFCPf-mh4xGwyepsWk7uq01JDxv-kql8A9D9_sB0xtaJAeybu3vpSP0e_m-VXa8Yi2KQHYYiMbWOMp13i8CM1bVrHJyhmlUybNzQU?key=VReuh94fGGpJZLGsXsGdUQ)
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXd0-R0qbpiy49r98aC70hKehhtPBrYHunDbcoB53NEHZYIx0gwFUp4qcXNFezf2Zvcqr_AccPoAHj2J0_AKk-xMsmtDDFs2Ib0Pt_XaT0uq5NoIbf-djIx9prlmXTTTTaQpIDSoLJUlEfUgG2MlQm_RdfBe?key=VReuh94fGGpJZLGsXsGdUQ)




---

> **Nota**: Cuando se instancia alguna cosa, se le subraya para indicar que es una instancia.
