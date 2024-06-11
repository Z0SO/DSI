
# Puertos

Un puerto es un punto de interacción entre un clasificador (como una clase o un componente) y su entorno. Los puertos pueden tener diferentes comportamientos según cómo estén configurados, y se pueden clasificar en dos tipos principales: puertos de comportamiento y puertos de delegación.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXftFUdG6kb9U5750x46OK3mtxd5OOwjvOqyH6N4Xf0MqpuE-1YpTm0dyLYTbgg2iEBYinrpD95pNOCs8ZnPHZE6x3LsGHUGhK3P1oywvf1aqxswo4vmBkelJj9dww--jFyVp2wQMEdoCBW_2Lz_1az9xryJ?key=VReuh94fGGpJZLGsXsGdUQ)

## Características Generales

- **Conceptual**: Es un punto de conexión del clasificador con el conector.
- **Punto de Interacción**: Con una interfaz bien definida.
- **Clasificadores Encapsulados**: Utilizados principalmente en componentes.
- **Tipos**: Pueden ser simples o complejos.
  - **Puerto Simple**: Con una única interfaz necesaria o proporcionada.
  - **Puerto Complejo**: Con más de una interfaz necesaria o proporcionada.

## Tipos de Puerto

### Puerto de Comportamiento

Un puerto de comportamiento es un tipo de puerto en el cual las solicitudes que se reciben son manejadas directamente por el comportamiento interno del clasificador que posee el puerto.

- **Propiedad isBehavior**: Debe estar establecida en `true` para que un puerto sea considerado de comportamiento.
- **Implementación Directa**: Las solicitudes se manejan directamente por el comportamiento del clasificador propietario, sin ser reenviadas.
- **Indicador Visual**: Representado en un diagrama mediante un puerto conectado a un pequeño símbolo de estado dentro del clasificador encapsulado.
- **Ejemplo Teléfono Inteligente**: Cuando recibes una llamada, el sistema operativo del teléfono maneja directamente la solicitud para contestar la llamada.

### Puerto de Delegación

Un puerto de delegación está conectado a uno o más puertos o partes internas del clasificador encapsulado. Las solicitudes que llegan a este puerto se transmiten a los puertos internos o partes internas para su gestión.

- **Conector de Delegación**: Vinculado mediante un conector que enlaza el puerto externo a roles o puertos internos del clasificador.
- **Reenvío de Solicitudes**: Las solicitudes no son manejadas directamente por el comportamiento del clasificador encapsulado, sino que se pasan a otros puertos internos.
- **Ejemplo Asistente de Voz (como Alexa)**: Cuando le das una orden para encender las luces, el puerto de delegación de Alexa envía la solicitud al sistema de iluminación inteligente de tu casa.

---

> En UML, los puertos son cruciales para definir cómo un clasificador interactúa con su entorno y otros clasificadores. La implementación y conexión de estos puertos pueden variar, proporcionando flexibilidad en el diseño del sistema.
