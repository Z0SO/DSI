
# Principios SOLID

Enfocados a la elaboración de software de calidad. Cuando estos principios se aplican en conjunto, es más probable que un desarrollador cree un sistema que sea fácil de mantener y ampliar en el tiempo. 

Los principios SOLID son guías que pueden ser aplicadas en el desarrollo de software para eliminar código sucio, provocando que el programador tenga que refactorizar el código fuente hasta que sea legible y extensible.

## Principios SOLID

1. **Single Responsibility Principle (SRP)**
   - Una clase debe tener una, y solo una, razón para cambiar. 
   - Cada clase debe encargarse de una única responsabilidad.

2. **Open/Closed Principle (OCP)**
   - Las entidades de software (clases, módulos, funciones, etc.) deben estar abiertas para extensión, pero cerradas para modificación.
   - Permite que el comportamiento de una clase se extienda sin modificar su código fuente.

3. **Liskov Substitution Principle (LSP)**
   - Los objetos de una clase derivada deben poder reemplazar objetos de la clase base sin alterar el funcionamiento del programa.
   - Las clase base deben ser sustituibles por sus subclases.

4. **Interface Segregation Principle (ISP)**
   - Los clientes no deben estar obligados a depender de interfaces que no utilizan.
   - Prefiere muchas interfaces específicas en lugar de una sola interfaz general.

5. **Dependency Inversion Principle (DIP)**
   - Los módulos de alto nivel no deben depender de módulos de bajo nivel. Ambos deben depender de abstracciones.
   - Las abstracciones no deben depender de detalles. Los detalles deben depender de abstracciones.

