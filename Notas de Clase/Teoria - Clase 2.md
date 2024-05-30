
---

- 

---

# Introduccion a Orientacion a objetos

### Breve Historia de los metodos OO

## Beneficios de la OO

- Disminución del **GAP** **semántico**. Representación consistente en todo el ciclo de vida. 

		El "gap semántico" se refiere a la discrepancia o diferencia entre el mundo del problema que se está intentando resolver y la manera en que ese problema se representa y se aborda en el software. En otras palabras, **es la brecha entre la comprensión del problema por parte de los usuarios o los expertos del dominio y la forma en que los desarrolladores implementan ese conocimiento en el software**.

	Por ejemplo, cuando los desarrolladores construyen un sistema de software basado en requisitos específicos, puede haber una desconexión entre la manera en que los usuarios entienden y hablan sobre su problema y cómo se ha traducido eso en el código o el diseño del software. Este desajuste puede llevar a malentendidos, errores y dificultades en la comunicación entre los desarrolladores y los usuarios finales.

	En el contexto de la programación orientada a objetos, el gap semántico se reduce porque **los objetos y las clases del software reflejan directamente entidades y conceptos del mundo real**, lo que *hace que el software sea más comprensible y alineado con el dominio del problema*. Esto ayuda a cerrar la brecha entre la comprensión del problema por parte de los usuarios y la implementación del software por parte de los desarrolladores.

- Reusabilidad del Software

- Mejora en la mantenibilidad y modificabilidad de SW

- Mejor interacción USUARIO-ANALISTA-DISEÑADOR 

- Más apropiado para resolver problemas complejos (GUI’s, patterns, etc.)

## Que es un sistema OO

Un sistema orientado a objetos es un sistema donde sus elementos son entidades a las que denominaremos “**objetos**” que interactúan entre sí por medio del envío y recepción de “**mensajes**”, todo esto con el fin de cumplir un "**objetivo**" claro y definido para el sistema. Cada uno de estos objetos no funciona en forma aislada sino que “**colabora**” con otros objetos del sistema conversando con los mismos por medio de “**mensajes**”, y cada objeto realiza tareas o cumple un **rol** específico en el sistema acorde a la “**responsabilidad**” que tenga asignada.

## Concepto de Objeto

##### Definición 1
Un objeto es algo real o abstracto acerca del cual almacena datos y operaciones que manipulan dichos datos (Martin/Odell). 
##### Definición 2 (Importante)
Un objeto es una entidad que tiene estado, comportamiento e identidad. La estructura y el comportamiento de objetos similares se definen en su clase común, Los términos instancias y objetos son intercambiables (Booch). Estado: valor de los atributos de un objeto en un determinado momento. Comportamiento: Que podrá hacer el objeto, que podrá ofrecer a si mismo y al resto, la parte dinámica.

- Conoce cierta informacion
- realiza ciertos servicios
- mantiene ciertas conecciones
- Toma decisiones
#### ¿Que puede ser un Objeto?

- Algo físico (un avión, un libro, una persona).
- Algo abstracto (cuenta bancaria, una fecha, un número).
- Algo del dominio del problema(una factura, un cliente).
- Algo de dominio de la solución(un formulario, una página web).


## Concepto de Mensaje
 
Los mensajes son el mecanismo por el cual se comunican los objetos para poder interactuar y colaborar unos con otros. El mensaje es un metodo.

![[Pasted image 20240408181114.png]]

### Tipos de Mensajes

## Concepto de responsabilidad
Obligacion de un clasificador
Las obligaciones que la clase o los Objetos de esa clase  deben cumplir.
Cosas que un objeto hace o conoce.
La responsabilidad debe definirse antes que los metodos y atributos.

**Hacer** refiere a metodos 
**Conocer** refiere a atributos


**Rol** -> Es un conjunto relacionado de responsabilidades que puede usarse de manera intercambiable. Sinonimo de proposito.
Es un conjunto de responsabilidades relacionadas. Lo vamos a utilizar como *Proposito* de la clase.


Estereotipos:
- Caracterizaciones de las funciones que necesita una aplicacion
- Al simplificar y caracterizar en exceso, podemos reflexionar sobre la naturaleza del papel de un objeto mas facilmente.


- Information Holder: Conoce y proporciona informacion
- Structurer: Mantiene las relaciones entere los objetos y la informacion sobre esas relaciones
- Service previder: Realiza trabajos y ofrece servicios informaticos
- Coordinator: Reacciona a los eventos delegando tareas a otros
- Controller: Toma decisiones y dirige estrechamente las acciones de los demas
- Interfacer: Transforma la informacion y las solicitudes entre distintas partes de nuestro sistema


## Concepto de Colaboracion


### Conceptos del libro

## Concepto de Clase
## Principios fundamentales
#### Abstraccion
#### Encapsulamiento
#### Herencia
[clase1] <|-- [clase 2] 
Por mas que haya herencia, la clase 2 no puede acceder a los atributos que tiene clase 1 directamente si estos son privados, Para que eso sucediera los atributos debe ser publicos o protegidos.
#### Polimorfismo

## Diseño OO

