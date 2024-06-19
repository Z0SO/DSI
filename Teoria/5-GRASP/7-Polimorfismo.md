## ♻️Polimorfismo - Polymorphism

This principle encourages leveraging polymorphism (ability to treat objects of different classes in a similar way) to achieve flexible and adaptable code. It can be implemented through inheritance and interfaces.

### Problema
¿Cómo manejar las alternativas en función del tipo? ¿Cómo crear componentes de software conectables?

### Solución
Cuando las alternativas o los comportamientos relacionados varían según el tipo (clase), asigne la responsabilidad del comportamiento mediante operaciones polimórficas a los tipos para los que varía el comportamiento.

### Corolario
No pruebe el tipo de un objeto y use la lógica condicional para realizar diversas alternativas según el tipo. Este principio fundamental de la orientación a objetos permite que una misma función sea implementada de diferente forma según la clase que la implementa.

### Idea Principal
Evitar el uso de condicionales cuando pueden ser reemplazadas por polimorfismo, redefiniendo el método en las clases que lo necesiten.