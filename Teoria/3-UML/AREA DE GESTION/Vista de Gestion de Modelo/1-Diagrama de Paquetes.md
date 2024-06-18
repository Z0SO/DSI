
---
## Diagrama de Paquetes

- **Gestión del Modelo**: Consiste en paquetes (incluyendo tipos especiales de paquetes) y relaciones de dependencia entre ellos.
  - Debe seguir algún principio racional, como **funcionalidad** **común**, **implementación** **fuertemente** **acoplada** y un punto de **vista común**.

### ¿Qué es un paquete?

- **Definición**: Es una unidad de organización del modelo.
  - Cada parte de un modelo debe pertenecer a un paquete.
  - Los paquetes contienen elementos de alto nivel del modelo, como clases y sus relaciones, máquinas de estados, diagramas de casos de uso, interacciones y colaboraciones.
  - Pueden ser organizados por la vista, la funcionalidad o por cualquier otra base que elija el modelador.
  - Se pueden utilizar para almacenamiento, control de acceso, gestión de la configuración y construcción de bibliotecas que contienen fragmentos reutilizables del modelo.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeKT9o7Mm52kkCu4DWhTcdDm7KSMGy7HXDxc_8KDmqQohVUK6CXiGhc-i2X2CNd-qq4neNAZqwcQq10UxwmQOG4QGSi-BLth1-Fuk2GlmC1X5tyPjmDALbQWIrTsXDBKKbjS0el7V6ia7FeAAOb_I6fxz6K?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-us.googleusercontent.com/docsz/AD_4nXe84D1nLeP3uoW3mD-OqdKsFFJUOhG_muTa2qhb60mo36eArcf7tujVih44pu9AiLltsUa4_6nmg3C-mSHGTpDiklC8sBrxczZ6cFHair6i0PjowiP4M7TKLFrUxP0R79-mEo1gVW4bTyfhIByDgsrswVre?key=VReuh94fGGpJZLGsXsGdUQ)
### Nombres

- **Nombre Simple**: El nombre solo se denomina nombre simple.
- **Nombre Calificado**: Consta del nombre del paquete precedido por el nombre del paquete en el que se encuentra.
- **Organización de Modelos**: Los paquetes ofrecen un mecanismo general para la organización de los modelos/subsistemas.

### Criterios de Organización

- **Por la Vista**
- **Por Subsistema**
- **Por Etapa del Ciclo de Desarrollo**

Una buena organización refleja la arquitectura de alto nivel del sistema.

### Dependencia de Importación

**Visibilidad**
  - **Público (+)**: Constituye la interfaz del paquete.
  - **Privado (-)**: No son visibles para nadie fuera del paquete.
  - **Protegido (#)**: Solo son visibles para los paquetes que heredan de otro paquete.
- **Operador `::`**: Permite designar una clase definida en un contexto distinto del actual. Se denomina nombre totalmente calificado.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcjtxqxyUybZkp3Tl-hXhrSTI2kbUv5-TgkeLJhCxv7q-ao7qQTit4iWraSpCinEGvZwFUehVWsbBmEN-XiQO6zL1_tcf7C3rqdxzXAhhhmbD3XqYpjfI0XeLBFYL6D6ROruCA907vMEB5rFVIDmfKBEm8?key=VReuh94fGGpJZLGsXsGdUQ)

**Import**
  - Evita escribir el nombre completo.
  - Aplica dos estereotipos (import y access) y ambos especifican que el paquete origen tiene acceso al contenido del destino.
  - `Import` añade el contenido del destino al espacio de nombres público del origen, evitando la necesidad de calificar los nombres. Esto implica la posibilidad de colisión de nombres que hay que evitar para tener un modelo bien formado.
  - `Access` añade el contenido del paquete destino al espacio de nombres privados del origen. La diferencia es que no se pueden reexportar los elementos importados si un tercer paquete importa el paquete origen inicial.
  - La mayoría de las veces se usará `import`.

### Modelo y Subsistema

- **Modelo**: Es un paquete que abarca una descripción completa de una vista particular de un sistema. Proporciona una descripción cerrada de un sistema a partir de un punto de vista.
- **Subsistema**: Paquete que tiene piezas separadas de especificación y de realización. Representa una partición del sistema.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXe08R-8s0PI7WiO6-ooyT8BRDTQd5HXlAiPwxdm-6FTbE5ztRrX0bf8xftQX_rD_ZGYtwWDZ0UKRLg75xIJkIsSexabstVEaGA4AltTNMfGQuiXhQirYUujq7muySvpLm29maVqMBz4dPlk0xXf2ubRM4E?key=VReuh94fGGpJZLGsXsGdUQ)