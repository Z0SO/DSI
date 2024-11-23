### Clases Abstractas vs Interfaces

#### Interfaces

- **Métodos Abstractos**: Solo pueden contener métodos abstractos (sin implementación).
- **Atributos**: No pueden tener atributos.
- **Constantes**: Pueden definir constantes.
- **Herencia**: No tienen relación de herencia directa con ninguna clase en particular; se definen independientemente.
- **Implementación**: Pueden ser implementadas por múltiples clases y extendidas por otras interfaces.
- **Instanciación**: No se pueden instanciar.

#### Clases Abstractas

- **Métodos**: Pueden contener tanto métodos abstractos (sin implementación) como métodos concretos (con implementación).
- **Atributos**: Pueden tener atributos.
- **Herencia**: Están sujetas a la herencia; una clase abstracta puede ser la superclase de otras clases.
- **Implementación**: Proporcionan una implementación común que puede ser compartida por todas sus subclases.
- **Instanciación**: No se pueden instanciar.

#### Características Comunes

- **Definición de Métodos**: Tanto las interfaces como las clases abstractas definen métodos que pueden ser implementados por otras clases.
- **Generalización y Realización**: Entre interfaces y clases hay relaciones de implementación/realización, y entre interfaces y otras interfaces o clases y otras clases hay relaciones de generalización.
- **Instanciación**: No se pueden crear instancias directas de interfaces ni de clases abstractas.
- **Uso en Polimorfismo**: Las interfaces se pueden utilizar en cualquier lugar donde se pueda usar una clase, facilitando el polimorfismo.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdQfe4RsupgqxrJ386wgm_JT1pacbK1Xup4FPiV1srvbWJSQKRNSAZHjIwg4gmM0T_1vNtBKqmq1_Wd004RLVO5wAU3OfwYGVoqFtNtBJ83yrYmNvwfZK6RLsZjnB0LYA9odWT3Efi1gn_UhPhBY7pLuCE?key=VReuh94fGGpJZLGsXsGdUQ)


#### Diferencias Clave

- **Métodos Abstractos**: Todos los métodos de una interfaz son abstractos y no tienen cuerpo, mientras que una clase abstracta puede tener métodos con o sin implementación.
- **Implementación y Extensión**: Una interfaz solo puede ser implementada por clases o extendida por otras interfaces, mientras que una clase abstracta puede ser extendida por otras clases.
- **Uso de Métodos No Abstractos**: Las clases abstractas se usan para proporcionar una implementación común para todas las subclases, reduciendo la duplicación.

### Dependencias

- **Descripción**: Relación entre dos elementos donde uno es cliente y el otro proveedor.
- **Impacto de Cambios**: Los cambios en el proveedor pueden afectar al cliente.
- **Estereotipos**: Las dependencias pueden tener estereotipos para definir su naturaleza específica.

#### Ejemplo Comparativo

- **Interfaz**:
  ```java
public interface IAnimal {
    void eat();
    void sleep();
}
  ```

- **Clase Abstracta**:
```java
public abstract class Animal {
    private String name;
      
    public abstract void eat();
      
    public void sleep() {
        System.out.println("Sleeping...");
    }
    
    public String getName() {
        return name;
    }
      
    public void setName(String name) {
        this.name = name;
    }
}
  ```

En este ejemplo, `IAnimal` es una interfaz que define dos métodos abstractos `eat` y `sleep`, mientras que `Animal` es una clase abstracta que define un método abstracto `eat` y un método concreto `sleep`. Además, `Animal` tiene un atributo `name` con sus métodos getter y setter.

### Uso en Diagramas UML

- **Interfaz**: Se representa como un rectángulo con el nombre de la interfaz en cursiva y precedido por la palabra clave `<<interface>>`. Las clases que implementan la interfaz tienen una línea punteada con un triángulo hacia la interfaz.
- **Clase Abstracta**: Se representa como un rectángulo con el nombre de la clase en cursiva. Las clases que heredan de la clase abstracta tienen una línea sólida con un triángulo hacia la clase abstracta.



---

###### Conclusión
> Tanto las interfaces como las clases abstractas son herramientas poderosas en la programación orientada a objetos para definir contratos y compartir implementaciones comunes. La elección entre usar una interfaz o una clase abstracta depende de la necesidad de métodos concretos y la estructura jerárquica del modelo de clases. Las dependencias juegan un papel crucial en indicar cómo los cambios en un componente pueden afectar a otros componentes del sistema, y el uso adecuado de estereotipos puede ayudar a clarificar estas relaciones en los diagramas UML.