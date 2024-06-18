
## Actividades en UML

Una actividad en UML es un grafo de nodos y flujos que muestra el flujo de control y datos a través de los pasos de una computación. Puede incluir tanto ejecución concurrente como secuencial y utiliza constructores de sincronización y bifurcación, superando a los diagramas de flujo tradicionales.

----

### Componentes Clave

#### Nodos de Actividad

Representan la ejecución de una sentencia o un paso en un flujo de trabajo. Se conectan mediante flujos de control y datos. Un nodo empieza su ejecución cuando hay tokens en sus flujos de entrada y sigue a los nodos en sus flujos de salida tras completarse.

#### Flujos de Control

Son como transiciones que ocurren al finalizar la ejecución de un nodo.

#### Concurrencia

Un diagrama de actividad puede incluir bifurcaciones y divisiones en hilos concurrentes que pueden ejecutarse simultáneamente o en cualquier orden. Los nodos de control predefinidos soportan decisiones y fusiones.
#### Acciones

Son las hojas de un grafo de actividad y representan actividades básicas predefinidas como:
- Acceder o modificar atributos.
- Crear o destruir objetos.
- Invocar operaciones.
- Enviar señales.


----