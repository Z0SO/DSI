## Variaciones Protegidas - Protected Variations

This principle addresses situations where subclasses might need to modify inherited behavior. It suggests using techniques like abstract methods or hooks to allow for controlled variations within a defined framework.

### Descripción
Variaciones protegidas, es el principio fundamental de protegerse frente al cambio. Esto quiere decir que lo que veamos en un análisis previo que es susceptible de modificaciones lo envolvemos en una interfaz y utilizamos el polimorfismo para crear varias implementaciones y posibilitar implementaciones futuras de manera que quede lo menos ligado posible a nuestro sistema. Este principio está muy relacionado con el polimorfismo y la indirección.

### Beneficios
- **Flexibilidad**: Se pueden agregar nuevos tipos de jugadores sin modificar el código principal.
- **Reutilización**: La lógica básica de las acciones se define en la clase abstracta `Jugador` y se reutiliza en las clases derivadas.
- **Modularidad**: El código está organizado en clases con responsabilidades bien definidas, lo que facilita su comprensión y mantenimiento.
- **Legibilidad**: El código es más claro y fácil de entender al evitar la duplicación de código y el uso de lógica condicional para determinar el tipo de jugador.

### Ejemplo
Imaginemos un juego de Monopoly con "variaciones protegidas":

#### El Tablero
- **Casillas de propiedades**: Cada casilla representa una propiedad con características únicas, como su valor, tipo (residencial, comercial, etc.) y alquiler.
- **Casillas de acción**: Estas casillas desencadenan eventos que afectan a los jugadores, como ir a la cárcel, pagar impuestos o recibir dinero.

#### Los Jugadores
- **Jugador estándar**: Un jugador típico que compra propiedades, construye casas y hoteles, y cobra alquiler a otros jugadores.
- **Jugador inversor**: Un jugador que se enfoca en comprar propiedades estratégicas y negociar acuerdos con otros jugadores para obtener beneficios.
- **Jugador constructor**: Un jugador que se centra en construir casas y hoteles para aumentar el valor de sus propiedades y maximizar el alquiler.

#### Las Acciones
- **Comprar una propiedad**: El jugador paga el precio de la propiedad al banco y pasa a ser su dueño.
- **Construir casas y hoteles**: El jugador paga una cantidad de dinero para construir casas o hoteles en sus propiedades, lo que aumenta el alquiler.
- **Cobrar alquiler**: Cuando un jugador cae en una propiedad de otro jugador, debe pagar el alquiler correspondiente.

#### Implementación con "Variaciones Protegidas"
- **Clase abstracta `Jugador`**: Define las acciones básicas que puede realizar cualquier jugador, como comprar propiedades, construir y cobrar alquiler.
- **Clases derivadas `JugadorEstandar`, `JugadorInversor` y `JugadorConstructor`**: Heredan de la clase `Jugador` y sobrescriben el método `cobrarAlquiler()` para implementar la lógica específica de cada tipo de jugador.

##### Ejemplo
- `JugadorEstandar.cobrarAlquiler()`: Calcula el alquiler base de la propiedad y lo cobra al jugador que cayó en ella.
- `JugadorInversor.cobrarAlquiler()`: Además del alquiler base, el jugador inversor puede aplicar un recargo adicional a la renta según la estrategia de inversión.
- `JugadorConstructor.cobrarAlquiler()`: El jugador constructor aumenta el alquiler base en función del número de casas y hoteles que haya construido en la propiedad.

### Resumen
Las "variaciones protegidas" permiten organizar el código del juego de Monopoly de manera eficiente y modular, aprovechando el polimorfismo para implementar comportamientos diferentes para cada tipo de jugador. Esto hace que el código sea más flexible, reutilizable, legible y fácil de mantener.

## Conclusiones
These are some of the key GRASP principles. Following them helps developers create well-structured, maintainable, and reusable object-oriented software.

### Diferencias
- **Indirección**: Útil para reducir el acoplamiento entre clases.
- **Fabricación Pura**: Para mejorar la cohesión de las clases existentes.
- **Patrón de Controlador**: Para centralizar la lógica de negocio y facilitar la separación de preocupaciones.
- **Variaciones Protegidas**: Para implementar comportamientos diferentes en clases derivadas.
```

Puedes copiar y pegar este texto en Obsidian para tener tus apuntes organizados y bien formateados. Si necesitas hacer alguna modificación o agregar más contenido, házmelo saber.