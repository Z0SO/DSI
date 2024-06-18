
---

## Principio Open/Closed (OCP)

### Enunciado Original
> *Las entidades de software (clases, módulos, funciones, etcétera) deberían estar abiertas a la extensión pero cerradas a la modificación.*

### Interpretación
Cambia el comportamiento de una clase mediante herencia, polimorfismo y composición.

### Explicación
El **OCP** establece que el comportamiento de las entidades de software debe poder extenderse sin modificar su código fuente original. Esto se logra mediante la herencia, el polimorfismo y la composición, permitiendo que las clases sean reutilizables y resistentes a cambios futuros sin necesidad de alterarlas directamente.

### Ejemplo Práctico

#### Problema Inicial
En una aplicación de dibujo, la clase `EditorGrafico` tenía métodos definidos para dibujar cada tipo de figura. Esto provocaba que siempre que apareciera una nueva figura, hubiera que modificar la clase `EditorGrafico` y crear nuevas clases, no cumpliendo con el OCP.

```java
class EditorGrafico {
    public void dibujarCirculo(Circulo circulo) {
        // lógica para dibujar un círculo
    }

    public void dibujarCuadrado(Cuadrado cuadrado) {
        // lógica para dibujar un cuadrado
    }

    // Nuevas figuras requerirían modificación de esta clase
}
```

#### Solución
Usar clases abstractas e interfaces para separar el comportamiento, evitando modificar las clases bases cada vez que aparezcan nuevos requisitos.

```java
interface Figura {
    void dibujar();
}

class Circulo implements Figura {
    @Override
    public void dibujar() {
        // lógica para dibujar un círculo
    }
}

class Cuadrado implements Figura {
    @Override
    public void dibujar() {
        // lógica para dibujar un cuadrado
    }
}

class EditorGrafico {
    public void dibujarFigura(Figura figura) {
        figura.dibujar();
    }
}

// Agregar nuevas figuras no requiere modificar EditorGrafico
class Triangulo implements Figura {
    @Override
    public void dibujar() {
        // lógica para dibujar un triángulo
    }
}
```

### Beneficios del OCP
- **Flexibilidad**: Permite que las entidades de software se adapten a nuevos requisitos sin cambiar el código existente.
- **Mantenibilidad**: Facilita el mantenimiento del código, ya que las extensiones no afectan la funcionalidad existente.
- **Reusabilidad**: Aumenta la reusabilidad de las clases y módulos al permitir que se extiendan sin ser modificados.

Aplicando el OCP, se mejora la robustez del software, haciéndolo más fácil de mantener y extender a lo largo del tiempo.

