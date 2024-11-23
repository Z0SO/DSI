
---
## Estereotipos

Son un **mecanismo de extensibilidad** para definir meta-clases. Pueden **ampliar la semántica**, pero no la estructura de las clases de metamodelos preexistentes
### Clases: Estereotipos

Los estereotipos son una **forma de clasificar elementos** dentro del modelo UML para **proporcionarles un propósito específico y definido**. A continuación, se describen algunos estereotipos comunes para clases en UML:

- **Entidad**: Se utiliza para clases que representan objetos del dominio que guardan o contienen información. Ejemplos típicos incluyen clases que modelan datos del sistema, como `Cliente`, `Producto`, etc.

- **Interfaz**: Clases que actúan como fronteras y se comunican con actores externos (personas, otros sistemas). Estas clases suelen manejar la interacción entre el sistema y el mundo exterior, como las interfaces de usuario o los servicios web.

- **Control**: Se encargan de gestionar el flujo de mensajes dentro de un contexto específico y a menudo **implementan la lógica de negocio**. Estas clases suelen crearse y destruirse en el contexto de un caso de uso particular.

![[Pasted image 20240616232904.png]]

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXei6c6TVJGnGNiMXJt9Ys29qGIJBBnzx5cTQzakBLR5DpioIjw-luoM1fdTjoCsGZ9v-L9cvlr4UDimD0zmrZS3Q2pKetwb3DjDRsYOhjLttFReppjCYO9QG46yTPoXkR-PcRr9aw6DFc0gb7HLjKNp0S8I?key=VReuh94fGGpJZLGsXsGdUQ)
### Mecanismo de Extensibilidad

El mecanismo de estereotipos proporciona una forma de ampliar el significado de los clasificadores en UML. Aquí hay más detalles sobre este mecanismo:

**Propósito**: Permitir que los modeladores añadan semántica adicional a los elementos del modelo sin alterar la estructura subyacente del UML.
**Capacidades**:
  - Los estereotipos pueden ampliar la semántica pero no la estructura de clases predefinidas en los metamodelos de UML.
  - Ejemplos de estereotipos comunes incluyen `derive` (derivado) y `executable` (ejecutable).
**Perfil estándar**: Los estereotipos pueden ser definidos por los usuarios para adaptarse a las necesidades específicas del proyecto o del dominio.

### Notación

Los estereotipos se representan en UML utilizando etiquetas con comillas francesas (`<<>>`). Por ejemplo, una clase que actúa como una entidad se etiquetaría como `<<entity>>`.
