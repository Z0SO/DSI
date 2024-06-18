
----
## Principio de Sustitución de Liskov (LSP)

### Enunciado
"Las funciones que utilizan punteros o referencias a clases base deben ser capaces de usar objetos de clases derivadas de éstas sin saberlo."

### Interpretación
Las subclases deben comportarse adecuadamente cuando sean usadas en lugar de sus clases base.

![[Pasted image 20240618202437.png]]

### Explicación
El principio de sustitución de Liskov establece que los objetos de una clase derivada deben ser sustituibles por objetos de la clase base sin alterar la funcionalidad del programa. Esto implica que las subclases deben cumplir con el contrato establecido por sus clases base, comportándose de manera coherente cuando se usan en su lugar.

### Ejemplo Práctico


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdM0G0i6beZ1ZGFOdqvzgPLLKNH5c2fSDV5kol7KtjRjiGd1MqciTrti6Wp9sJrDbCb0cnD2TwbPHegRHSWDdSp1LdNBoLvFb5MOgZFCfH-OYCOLFnio5DWG52iTYcZDM3hpGR1oEq5fY9UufNMQiMx1fM?key=VReuh94fGGpJZLGsXsGdUQ)
### Beneficios del LSP
- **Consistencia**: Garantiza que las subclases se comporten de manera coherente con sus clases base, evitando errores inesperados.
- **Reusabilidad**: Aumenta la reusabilidad del código al asegurar que las subclases puedan ser usadas en lugar de sus clases base sin problemas.
- **Mantenibilidad**: Facilita el mantenimiento del código al asegurar que las extensiones del mismo no rompan el comportamiento esperado.



---

#### Otro Ejemplo
En un sistema, se define una clase `Rectangulo` con métodos para calcular el área. Luego, se crea una clase `Cuadrado` que hereda de `Rectangulo`. Aunque `Cuadrado` es un tipo de `Rectangulo`, su comportamiento no es consistente al calcular el área.

```java
class Rectangulo {
    protected int ancho;
    protected int alto;

    public void setAncho(int ancho) {
        this.ancho = ancho;
    }

    public void setAlto(int alto) {
        this.alto = alto;
    }

    public int calcularArea() {
        return ancho * alto;
    }
}

class Cuadrado extends Rectangulo {
    @Override
    public void setAncho(int ancho) {
        this.ancho = ancho;
        this.alto = ancho;  // Para asegurar que ancho y alto sean iguales
    }

    @Override
    public void setAlto(int alto) {
        this.alto = alto;
        this.ancho = alto;  // Para asegurar que ancho y alto sean iguales
    }
}

// Problema: Usar Cuadrado en lugar de Rectangulo rompe el comportamiento esperado
```

#### Solución
Para cumplir con el LSP, se puede usar herencia o interfaces adecuadamente para asegurar que las subclases se comporten de manera consistente con sus clases base.

```java
interface Figura {
    int calcularArea();
}

class Rectangulo implements Figura {
    protected int ancho;
    protected int alto;

    public void setAncho(int ancho) {
        this.ancho = ancho;
    }

    public void setAlto(int alto) {
        this.alto = alto;
    }

    @Override
    public int calcularArea() {
        return ancho * alto;
    }
}

class Cuadrado implements Figura {
    private int lado;

    public void setLado(int lado) {
        this.lado = lado;
    }

    @Override
    public int calcularArea() {
        return lado * lado;
    }
}

// Ahora, tanto Rectangulo como Cuadrado implementan Figura y son intercambiables
```


Aplicando el LSP, se mejora la solidez del software, haciendo que las jerarquías de clases sean más coherentes y predecibles.