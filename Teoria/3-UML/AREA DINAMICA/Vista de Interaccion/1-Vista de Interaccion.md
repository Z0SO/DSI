#### Definición
La vista de interacción en UML **modela de forma dinámica una colaboración**

> Una colaboración es un conjunto de clases agrupadas para cumplir un objetivo específico

 Esta vista **permite visualizar el intercambio de mensajes entre objetos** (también llamados partes) en un sistema.

#### Elementos Principales

1. **Interacción**: Es el conjunto de mensajes intercambiados entre objetos en el contexto de la realización de un objetivo. Una interacción describe las secuencias de mensajes de una clase estructurada o colaboración.
   
2. **Objetos/Partes**: Los objetos que participan en la interacción, también llamados partes, son instancias de clasificadores estructurados.

3. **Mensajes**: Son las unidades de comunicación entre los objetos. Los mensajes pueden ser sincrónicos o asincrónicos, indicando llamadas a métodos, retornos de métodos, señales, etc.

4. **Enlace**: Es la conexión entre los objetos que permite el intercambio de mensajes.

#### Diagramas Utilizados

1. **Diagrama de Secuencia**: Muestra la secuencia de mensajes intercambiados entre los objetos a lo largo del tiempo. Es útil para modelar el flujo de control y la sincronización entre los objetos.

2. **Diagrama de Comunicación**: Anteriormente llamado diagrama de colaboración, muestra la estructura de los objetos y los enlaces entre ellos, así como los mensajes que se intercambian. Es útil para visualizar las relaciones y la topología de la interacción.

#### Interacción a Nivel Estático y a Nivel de Clase

- **Interacción a Nivel Estático**: Describe la secuencia de mensajes en el contexto de una colaboración estática, donde los objetos y enlaces son conocidos de antemano y no cambian durante la interacción.

- **Interacción a Nivel de Clase**: Describe la secuencia de mensajes entre roles de clase en un contexto más abstracto. Aquí, los mensajes son intercambiados entre instancias de roles que representan las clases.

#### Ejemplo de Diagramas

- **Diagrama de Secuencia**:
  ```plantuml
  @startuml
  actor Usuario
  participant Sistema
  participant BaseDatos

  Usuario -> Sistema : solicitarDatos()
  Sistema -> BaseDatos : obtenerDatos()
  BaseDatos --> Sistema : devolverDatos()
  Sistema --> Usuario : mostrarDatos()
  @enduml
  ```


#### Instancias de Interacción
Una instancia de una interacción corresponde a una instancia en su contexto, donde los objetos están ligados a roles que intercambian instancias de mensajes a través de enlaces ligados a conectores.
