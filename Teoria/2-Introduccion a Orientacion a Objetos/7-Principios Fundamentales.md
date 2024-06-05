
# Abstracción

La abstracción es un mecanismo que nos permite concentrarnos en los detalles más importantes y dejar de lado otros. Trata la complejidad al dejar de lado aspectos irrelevantes. No es exclusiva de la programación orientada a objetos.

### Características de la Abstracción

- **Enfoque en lo esencial:** Denota las características esenciales de un objeto que lo distinguen de todos los demás tipos de objetos.
- **Vista externa del objeto:** Se enfoca en la vista externa de un objeto y así sirve para separar el comportamiento esencial de un objeto de su implementación.

### Niveles de Abstracción

- **Nivel de Entidad:** Útil para el dominio del problema. Los objetos asociados a conceptos útiles del dominio o de la solución son las mejores abstracciones.
- **Nivel Causal:** Considerado menos efectivo. Un objeto formado por un conjunto de métodos no relacionados es un ejemplo de mala abstracción.

### Importancia de la Abstracción

La abstracción de un objeto debe estar antes que las decisiones sobre su implementación. Básicamente, mientras estás diseñando, te das cuenta de que muchos objetos se pueden agrupar en una clase abstracta, simplificando tu modelo. En otras palabras, antes de decidir cómo se construirá un objeto, es necesario comprender, reflexionar y definir claramente qué representa ese objeto en el contexto del sistema y qué funcionalidades debe proporcionar.

---

# Encapsulamiento

El encapsulamiento es un mecanismo que permite ocultar los detalles de implementación de un objeto. Se complementa con la abstracción, donde la abstracción se enfoca en el comportamiento observable, mientras que el encapsulamiento se enfoca en la implementación de ese comportamiento. 

### Funcionalidades del Encapsulamiento

- **Empaquetamiento de datos y funciones:** Agrupa los datos y métodos relevantes en una unidad coherente.
- **Mantenimiento y control de la complejidad:** Ayuda a mantener la complejidad bajo control al ocultar detalles internos y exponer solo lo necesario para interactuar con el objeto.

### Proceso de Encapsulamiento

Es el proceso de compartimentar los elementos de una abstracción que constituyen su estructura y comportamiento. Sirve para separar la interfaz conceptual de una abstracción y su implementación.

### Niveles de Visibilidad

Permite controlar el acceso a los datos y métodos de una clase, limitando quién puede interactuar con ellos desde fuera de la clase. Esto protege el estado interno del objeto.

- **Público (+):** Son accesibles desde cualquier parte del programa.
- **Protegido (#):** Son accesibles desde la propia clase y desde las clases hijas.
- **Privado (-):** Son accesibles solo desde dentro de la misma clase.

### Ejemplo

Un ejemplo práctico de encapsulamiento sería una clase "Cuenta Bancaria" que oculta los detalles de su implementación, como el saldo, y solo expone métodos para depositar, retirar y consultar saldo, protegiendo así la integridad de los datos y simplificando el uso de la clase para otros componentes del programa.


---

# Herencia

La herencia es un mecanismo que permite que una clase (subclase) herede atributos y métodos de otra clase (superclase). Esta característica fomenta la reutilización de código y facilita la creación de jerarquías de clases, donde las clases más específicas heredan comportamientos y características de clases más generales.

### Características de la Herencia

- **Vínculo "es un tipo de":** Establece un vínculo "es un tipo de" entre la superclase y la subclase.
- **Generalización a Especialización:** Va de la generalización a la especialización.

### Implementación

> [Clase 1] ᐊ– [Clase 2]


Desde los métodos de la clase 2, no se puede acceder a atributos o métodos privados de la clase 1. 
**Solución:** Cambiar esos atributos de la clase 2 de privados a protegidos (#).

## Aplicación de Herencia Múltiple

La herencia múltiple se aplica cuando varias clases comparten comportamientos comunes o cuando un objeto puede ser descrito como "es un" tipo de varias clases diferentes. Permite a una clase heredar de múltiples clases para evitar la duplicación de código y modelar relaciones complejas. Sin embargo, su uso puede introducir ambigüedades y complicaciones en el diseño del programa.

---

# Polimorfismo y Sobrecarga (Overloading)

### Polimorfismo

El polimorfismo es la capacidad de un objeto para presentar diferentes formas o comportamientos en función del contexto en el que se utilice. Es el principio por el cual una misma operación es resuelta de manera diferente según el objeto que recibe el mensaje.

- **Definición:** Es el principio por el cual una misma operación es resuelta de manera diferente según el objeto que recibe el mensaje.
- **Implementación:** La definición del método reside en la clase base, mientras que la implementación del método reside en la clase derivada.
- **Invocación:** La invocación es resuelta en tiempo de ejecución.
- **Tipos de Vinculación:** Se puede realizar con vinculación temprana (early binding) o vinculación tardía (late binding).

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfndtt_NtYFjpq6upZlNcoEGcFu7YociYGLCw64oQpn0UqoDomAOSs_RyIo-j0S1IH49y53q8Cf1uugz9c6s88CCrcIoUjLQuOit3ckbjNDC-w9r6w1ixePyf-OnKHi9pio0DR8wXp-TUO3Xv6KLU_N2Yyf?key=VReuh94fGGpJZLGsXsGdUQ)

### Sobrecarga (Overloading)

La sobrecarga consiste en definir más de un método con el mismo nombre pero con diferentes parámetros.

- **Definición:** Consiste en definir más de un método con el mismo nombre pero con diferentes parámetros.

### Descripción Adicional del Polimorfismo

El polimorfismo es la habilidad de los objetos pertenecientes a diferentes clases de responder a llamadas a métodos del mismo nombre, cada uno acorde a un comportamiento específico de la clase a la que pertenecen. Por lo tanto, el programador no necesita conocer el tipo exacto del objeto por anticipado, ya que el mismo es resuelto en tiempo de ejecución.

---
