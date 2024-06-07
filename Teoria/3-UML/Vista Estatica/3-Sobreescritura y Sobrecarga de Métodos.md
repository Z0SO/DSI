
# Definiciones
## Sobreescritura de Métodos (Overriding)
- **Definición:** En POO, es una característica que permite a una subclase proporcionar una implementación específica de un método que ya está definido en una de sus superclases.
- **Polimorfismo:** Permite un tipo específico de polimorfismo llamado subtipado. Los objetos de diferentes clases (subclases y superclases) pueden responder de manera diferente a las mismas llamadas de método.
- **Requisitos:**
  - El método en la subclase debe tener la misma firma (nombre y parámetros) que el método en la superclase.

## Sobrecarga de Métodos (Overloading)
- **Definición:** Capacidad de una clase de tener múltiples métodos con el mismo nombre pero con diferentes parámetros.
- **Características:**
  - Pueden existir varios métodos con el mismo nombre en una clase, pero cada uno con una lista de parámetros diferente.
  - El método a ejecutar se determina en función de los parámetros que se pasan cuando se llama al método.

---

### Ejemplo de Sobreescritura de Métodos

```java
class Animal {
    void hacerSonido() {
        System.out.println("El animal hace un sonido");
    }
}

class Perro extends Animal {
    @Override
    void hacerSonido() {
        System.out.println("El perro ladra");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal miAnimal = new Perro();
        miAnimal.hacerSonido(); // Salida: El perro ladra
    }
}
```

### Ejemplo de Sobrecarga de Métodos

```java
class Calculadora {
    int suma(int a, int b) {
        return a + b;
    }

    double suma(double a, double b) {
        return a + b;
    }

    int suma(int a, int b, int c) {
        return a + b + c;
    }
}

public class Main {
    public static void main(String[] args) {
        Calculadora calc = new Calculadora();
        System.out.println(calc.suma(5, 3)); // Salida: 8
        System.out.println(calc.suma(2.5, 3.5)); // Salida: 6.0
        System.out.println(calc.suma(1, 2, 3)); // Salida: 6
    }
}
```

---

### Resumen
- **Sobreescritura (Overriding):** Permite a una subclase proporcionar una implementación específica de un método definido en una superclase, permitiendo el polimorfismo de subtipado.
- **Sobrecarga (Overloading):** Permite que una clase tenga múltiples métodos con el mismo nombre pero diferentes parámetros, determinando el método a ejecutar según los parámetros pasados.

---
