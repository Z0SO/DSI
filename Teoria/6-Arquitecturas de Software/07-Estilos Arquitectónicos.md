## **Estilos Arquitectónicos**

Un estilo arquitectónico define cómo se organiza y estructura un sistema de software, utilizando un patrón probado y abstracto de buenas prácticas. Los componentes y conectores de cada estilo son específicos y están probados en diferentes contextos.

## **Patrones de Arquitectura (Centralizados)**

### **En Capas (Layered)**

Este patrón organiza el software en capas, donde cada capa contiene un conjunto de servicios relacionados. Cada capa depende de la capa inferior y es independiente de las superiores.

**Ventajas**:
- **Desarrollo modular**: Facilita el desarrollo e integración de nuevas funcionalidades.
- **Modificable y portátil**: Se pueden reemplazar capas sin cambiar las interfaces.
- **Separación de preocupaciones**: Las capas están separadas por roles y responsabilidades.

**Desventajas**:
- **Rendimiento**: A veces, la estructura de capas puede generar sobrecarga en el rendimiento.
- **Dificultad en la separación**: No siempre es fácil dividir un sistema en capas perfectamente.

**Ejemplo**: El Modelo OSI de redes.

![Modelo OSI](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcYB1KAdBiHDoY8u4-uWceCw5mdHW_6_IFOBsCRKf7-svmhzsf2HgJPgISx0qY_qvBY4BqpD2J4dbfoRBkh6pEfjnvDULM87GAmWFEMMap6PoLSrC69umgi4oYEp8Jl4n0vxe5a0HrWa2hMFCOBLQsO8c8_?key=VReuh94fGGpJZLGsXsGdUQ)

En un sistema en capas, la comunicación entre capas es rigurosa: una capa solo puede comunicarse con la capa superior e inferior.

![Ejemplo de Capas](https://lh7-rt.googleusercontent.com/docsz/AD_4nXezYHGEVSHHsxQbd5P0ln3uogQjzwVr4H9PvGmv6aLX5MADdIccY-i8N8YO7KO_OcOzCxmOgehzhOyBOvDqFVCqXkxJWWC0GtFv71-3CzC-O4SLACQl2ydQ7yYh0xXfqmuC1qhA01K-Wvdsw4FzIo53E8JF?key=VReuh94fGGpJZLGsXsGdUQ)

### **Repositorios / Pizarrón (Shared-Data)**

En este patrón, los componentes no interactúan directamente entre sí. En cambio, se comunican a través de un repositorio central de datos.

**Ventajas**:
- **Almacenamiento centralizado**: Facilita la gestión de grandes volúmenes de datos.
- **Control de versiones**: Ideal para sistemas con control de versiones o datos que cambian frecuentemente.

**Desventajas**:
- **Cuello de botella**: El repositorio central puede convertirse en un punto de fallo, afectando todo el sistema.

**Ejemplo**: Un IDE con herramientas conectadas a un repositorio de datos central, como el control de versiones.

![Ejemplo de Repositorio](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdAStlJUAVrQ7YCsC5T8qtEfwXW0B2SbtT_ijlTZbpog9VCJ4g2ltbPMEoPL1s6lwA4GLuBYP2ncAmUQ3OwfRa8eR55Bx5qvxyabQlkUUtUVB989G_ROmxFw3Xm0tUBL6EDZ2gFT4lyDzHceBOO7De3PF4?key=VReuh94fGGpJZLGsXsGdUQ)

### **Pipes and Filters (Pipes y Filtros)**

Este patrón se utiliza cuando necesitas realizar transformaciones sucesivas sobre un conjunto de datos.

- **Filtro**: Procesa la entrada y genera una salida, realizando transformaciones sobre los datos.
- **Pipes**: Son conductos que conectan los filtros entre sí.

**Ventajas**:
- Permite procesar los datos de forma incremental, comenzando a procesar la salida antes de que la entrada esté completamente disponible.

![Pipes y Filtros](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdts2MCUFfcb47IAS3BhkkUDdMC3V_GpMxuMWGu-8Ua55XtsVrSr7bRMpZEJblUsr2-2frW0sIbmRli91AO34tRWLZSaksNeuX4nwoACbEF73WQp4dN8QEsZ_mOiHL9O4cE3xl_7mwNFRAFOOg-LY-jDOVk?key=VReuh94fGGpJZLGsXsGdUQ)

### **Microkernel / Plug-in**

Este patrón tiene un sistema central básico con plugins que pueden ser añadidos para extender la funcionalidad del sistema. Los plugins son componentes independientes que ofrecen características adicionales.

**Ventajas**:
- **Extensibilidad**: Se pueden agregar nuevas funcionalidades sin afectar el sistema central.
- **Aislamiento**: El sistema central permanece pequeño y eficiente.

**Desventajas**:
- **Complejidad de integración**: La gestión de plugins puede ser compleja en sistemas grandes.

---
### Microkernel / Plug-in Architecture

La arquitectura de **microkernel** es un modelo que consta de un sistema central (core) y **plug-ins** o módulos adicionales. Este patrón permite la **extensibilidad**, **adaptabilidad** y el **aislamiento** de las características y funcionalidades de la aplicación.

#### Componentes Principales:

1. **Sistema Central (Core)**: 
   - Es el componente central que provee la funcionalidad mínima necesaria para operar el sistema.
   - Está diseñado para ser **ligero** y **escalable**, manteniendo solo las funciones esenciales.

2. **Plug-ins**:
   - Son componentes **independientes y autónomos** que añaden funcionalidades adicionales o especializadas al sistema central.
   - Los **plug-ins** permiten extender las capacidades del sistema sin modificar el núcleo.
   - Pueden contener **procesamiento especializado**, lógica personalizada, adaptadores o características adicionales.

#### Características:

- **Comunicación punto a punto**: Los plug-ins interactúan con el sistema central y entre ellos, generalmente, de manera directa y aislada.
  
- **Extensibilidad y Adaptabilidad**: 
   - Los plug-ins se pueden agregar fácilmente para mejorar o personalizar el sistema central sin afectar su funcionalidad básica.
   - Son ideales para aplicaciones que requieren agregar nuevas características sin cambiar el sistema base.

- **Independencia de los Módulos**: Los plug-ins son modulares y pueden implementarse de diversas formas, como bibliotecas o servicios remotos, lo que facilita su integración en sistemas diversos.

- **Iterativo e Incremental**: El modelo de microkernel permite una evolución incremental de la aplicación, añadiendo nuevas funcionalidades a medida que sea necesario.

#### Ventajas:

- **Bajo costo y simplicidad**: Es fácil de entender y más económico en términos de desarrollo y mantenimiento.
- **Escalabilidad en función de las necesidades**: Al agregar o quitar plug-ins según sea necesario, se puede adaptar el sistema rápidamente.

#### Desventajas:

- **Cuello de botella en el Core**: Si el sistema central se vuelve un punto de fallo, afectará toda la estructura. La dependiencia del core es un riesgo importante.
- **Limitada escalabilidad en sistemas complejos**: Este modelo puede no ser adecuado para sistemas que requieren alta escalabilidad o elasticidad.
- **Modificación constante del core**: Si se requieren modificaciones frecuentes en el sistema central, este patrón puede no ser el más adecuado.

#### Ejemplo:

Un ejemplo clásico de este patrón es **Google Chrome**. El núcleo del navegador proporciona funcionalidades básicas como la navegación y la gestión de pestañas. Sin embargo, las **extensiones** agregan características adicionales, como bloqueadores de anuncios o herramientas de productividad, sin modificar el sistema central del navegador.

En resumen, la **arquitectura de microkernel** permite que el **core** se mantenga lo más estable y simple posible, mientras que las funcionalidades adicionales son proporcionadas por los **plug-ins**, que pueden ser fácilmente integrados o modificados según sea necesario.

---

Espero que ahora esté más claro. Las imágenes ayudan a visualizar los conceptos, y he simplificado las explicaciones manteniendo los puntos clave de cada patrón. Si necesitas más detalles sobre algún punto, no dudes en preguntar.