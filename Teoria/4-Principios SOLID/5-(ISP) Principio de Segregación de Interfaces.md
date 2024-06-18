
---
## Principio de Segregación de Interfaces (ISP)

### Enunciado Original
"Los clientes no deberían ser forzados a depender de interfaces que no utilizan."

### Interpretación
Mantén las interfaces pequeñas y cohesivas, que puedan coexistir unas con otras.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcjOA2NK3cxbuIyQvgZwNBnRpDCDZhgzOZDKB9L945d-jV8KqiXWjR493DFzUvIBC7_k8EC9HSpU5heCpr6odX3mqg6snpE2csoAr8yCxBMv2rEbKmzBn1iljGXQRjCP72K_OG7EpySvOlygMRCtwIcRupJ?key=VReuh94fGGpJZLGsXsGdUQ)
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXex7emURRGP_85QiK50PhkGFjvbe2JSxozMflcMWkg9RPJwJC5yeHOXRbWDG7XLq-XyrCB_dsdbfN4lQfgVjhW21z6A-FAjfjRFL5fcoWPpCUQ3_GH9RPdYN2ulRF-Y_AENaNbsNXIQz6C-c-6yi69YyFwd?key=VReuh94fGGpJZLGsXsGdUQ)![[Pasted image 20240618202719.png]]

### Explicación
El principio de segregación de interfaces establece que las interfaces deben diseñarse de manera que los clientes solo necesiten conocer los métodos que realmente usan. Si una interfaz es demasiado grande y contiene métodos que no son relevantes para todos los clientes, se corre el riesgo de que los clientes se vean obligados a implementar métodos que no necesitan. La solución es dividir las interfaces en grupos más pequeños y específicos.

### Ejemplo Práctico

#### Problema Inicial
Supongamos que tenemos una interfaz `Trabajador` que define métodos para diferentes tipos de trabajos. Algunas clases que implementan esta interfaz no necesitan todos los métodos, lo que rompe el ISP.

```java
interface Trabajador {
    void trabajarEnOficina();
    void trabajarEnCampo();
}

class Oficinista implements Trabajador {
    @Override
    public void trabajarEnOficina() {
        // lógica para trabajar en oficina
    }

    @Override
    public void trabajarEnCampo() {
        // Este método no es necesario para Oficinista
    }
}

class Agricultor implements Trabajador {
    @Override
    public void trabajarEnOficina() {
        // Este método no es necesario para Agricultor
    }

    @Override
    public void trabajarEnCampo() {
        // lógica para trabajar en campo
    }
}
```

#### Solución
Separar el comportamiento en interfaces más pequeñas y específicas para cumplir con el ISP.

```java
interface TrabajadorDeOficina {
    void trabajarEnOficina();
}

interface TrabajadorDeCampo {
    void trabajarEnCampo();
}

class Oficinista implements TrabajadorDeOficina {
    @Override
    public void trabajarEnOficina() {
        // lógica para trabajar en oficina
    }
}

class Agricultor implements TrabajadorDeCampo {
    @Override
    public void trabajarEnCampo() {
        // lógica para trabajar en campo
    }
}
```

### Beneficios del ISP
- **Cohesión**: Las interfaces pequeñas y específicas aumentan la cohesión del código, haciendo que cada interfaz tenga una única responsabilidad clara.
- **Flexibilidad**: Los clientes pueden implementar solo las interfaces que necesitan, lo que reduce la cantidad de código innecesario y mejora la flexibilidad.
- **Mantenibilidad**: El código es más fácil de mantener, ya que los cambios en una interfaz no afectan a clientes que no la utilizan.

Aplicando el ISP, se mejora la calidad del software, haciendo que las interfaces sean más precisas y relevantes para los clientes que las utilizan.