
## Formas comunes de organizar la arquitectura de un sistema distribuido:

### Arquitectura Maestro/Esclavo

En esta arquitectura, un **proceso maestro** coordina el sistema, mientras que los **procesos esclavos** realizan tareas específicas.

- **Proceso Maestro**: Se encarga del cálculo, la coordinación y la comunicación, controlando los procesos esclavos.
- **Procesos Esclavos**: Se dedican a tareas específicas como la adquisición de datos o el procesamiento computacional intensivo, como el procesamiento de señales.

Esta arquitectura es adecuada para sistemas en tiempo real donde se requieren tiempos de respuesta garantizados, como en la **replicación de bases de datos** y el procesamiento distribuido.

Los procesos esclavos suelen manejar las tareas más exigentes computacionalmente, lo que permite una distribución eficiente de las cargas de trabajo.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcJlcGh8HNDCcfoQix9FjJD_92zYyJgqRwY8hec8nmQxAQmZM0sP93V7f3WDPW-tIMFo3LoRWZWzquWgPveY301fRPGY9O3BcNsHnoCksO-d-qu4I5NDb6odLAuymUR2EKC_U1u3njX8Wtge8wK25EXqRjn?key=VReuh94fGGpJZLGsXsGdUQ)

### Arquitectura Cliente-Servidor

En esta arquitectura, la aplicación se organiza en torno a **clientes** y **servidores** que interactúan entre sí:

- **Clientes**: Solicitan servicios a los servidores.
- **Servidores**: Proporcionan servicios a los clientes.

Los clientes y servidores pueden estar en la misma máquina o en máquinas diferentes. Los clientes conocen a los servidores, pero los servidores no conocen a los clientes.

- Los servidores pueden ser centralizados o distribuidos.
- Los clientes no necesitan conocer entre sí, solo a los servidores.

En la web, **HTTP** actúa como el protocolo para la comunicación entre **navegadores (clientes)** y **servidores de internet**.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXegDFVtG_ubIKFYwqyVyWF9zRBY7_4DbU8-KehbhOu-JaaKoQWtHfiQC1qblx9A7MknRmHTLr8DTEWfDOJxyQ_24UdXTr1XMdq2X_UApngqfmt3qb9r29OcnT4MCXgVoQqImAYhHGPjp6LaUDVhYvr9MUY_?key=VReuh94fGGpJZLGsXsGdUQ)

En esta arquitectura, el servidor provee servicios utilizados por los clientes, siendo internet un ejemplo claro, donde el navegador actúa como cliente y los servidores de internet como los proveedores de servicios.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdBTE-QYRiY1xft7DCmUUEdmAnHWHLpa4z2Z52t9Gg_ZFMjS3aeOSXTAFY0XZFG8qPn4-84NHi_JzyeSW8sCII4AJt-xf-CYxHInlzv6VT9_Q2ngoVOQlCUjF_p2xUdxQAGQXXCTFqqlzZQZzmybfTNnZs?key=VReuh94fGGpJZLGsXsGdUQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeDnX-EV8M-t5WeLyW6oG8ifdI3-w-RhN0caGtFqv5OHy97qHF5uGWA1R_0P-idJ8RkyUZhY568f8Uz-0ZWXu7yW8MC6M77yyNOT0EDkudXEB97bPmpywsGgxs3n-bGAxS9xcitlCaHlFYqqpgQJgFRr_YU?key=VReuh94fGGpJZLGsXsGdUQ)


---

### Arquitectura C/S (Cliente-Servidor) de dos niveles (2-tier)

En una **arquitectura cliente-servidor de dos niveles**, el sistema se organiza en torno a un único servidor lógico y un número indefinido de clientes que utilizan ese servidor para acceder a los servicios.

Hay dos enfoques principales:

#### 1. **Cliente Liviano** (Thin Client):
En este modelo, la **capa de presentación** se implementa en el cliente, mientras que todas las demás capas (gestión de datos, procesamiento de aplicaciones y base de datos) se implementan en el servidor.

- **Ventajas**:
  - **Fácil gestión de clientes**: No es necesario realizar muchas modificaciones o instalaciones en el cliente.
  
- **Desventajas**:
  - **Gran carga de procesamiento en el servidor**: El servidor se encarga de todo el procesamiento, lo que puede generar cuellos de botella si no está bien dimensionado.
  - **Gran carga en la red**: Dado que el cliente solo envía solicitudes y el servidor maneja casi toda la carga, el tráfico de la red puede aumentar significativamente.

Este modelo se utiliza a menudo cuando se **migran sistemas viejos** a arquitecturas cliente-servidor. En este caso, el sistema antiguo funciona como servidor y una **interfaz gráfica** se implementa en el cliente.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbnL1ctWIt5bReegKxMn5i96O7EPC9VpOKgy7xJqs3tKeYBo5G71HRNM7E5Slb1e0mONFXlsgdMjhrQJKjJu4POfduft-RvpZUfl5je0e-54AlO8gACQE4VvfReFMwOlg_XJXdELlHt83objdXb8bCuDQ?key=VReuh94fGGpJZLGsXsGdUQ)

#### 2. **Cliente Pesado** (Fat Client):
En este modelo, tanto la **capa de presentación** como la **aplicación** se ejecutan en el cliente, mientras que los datos y la gestión de la base de datos se mantienen en el servidor. Una parte o la totalidad del procesamiento de la aplicación se realiza en el cliente.

- **Ventajas**:
  - **Uso de la potencia de procesamiento disponible en el cliente**: El cliente asume más carga de procesamiento, reduciendo la demanda en el servidor y la red.
  
- **Desventajas**:
  - **Necesidad de desplegar y mantener el software en cada cliente**: Hay que instalar y actualizar la aplicación en todos los clientes de forma periódica.
  
Este modelo es más adecuado para **nuevos sistemas cliente-servidor** en los que las capacidades del cliente se conocen de antemano y el cliente tiene suficiente potencia de procesamiento. Es más complejo de gestionar, ya que se requiere mantener el software actualizado en todos los dispositivos.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfp-zHCBvFKdMfLZ5OIN5bRH56D_s9gwTEshXpkAMJ-cOm_WkyZbH2YTt_KwRwlVxpISGWDOJeptiZ20d_6dVAXdVclnb6vCPUJJ9ZBgRbY2tijf6nOtC-LyYthce_e9pztoLdJq4QROfEFGKn8BH5wIwXQ?key=VReuh94fGGpJZLGsXsGdUQ)


---

### Arquitectura Cliente/Servidor Multinivel (Multitier)

En una arquitectura cliente-servidor multinivel, el sistema está dividido en diferentes capas, como presentación, gestión de datos, procesamiento de aplicaciones y base de datos. Cada capa puede estar en un procesador separado, lo que mejora el rendimiento y escalabilidad en comparación con un modelo de dos capas, como el cliente grueso (fat-client).

#### Desventajas:
- **Costo y complejidad:** Implementar este tipo de arquitectura puede ser costoso y complejo, especialmente en sistemas pequeños, donde las ventajas no justifican el gasto en hardware, software y diseño.

#### Conceptos clave:
- **Niveles:** Son agrupaciones lógicas de componentes, no componentes físicos. 
- **Capas vs. Niveles:** Las capas son unidades de implementación (como módulos de software), mientras que los niveles se refieren a la estructura de los componentes en tiempo de ejecución.

### Componentes Distribuidos

En una arquitectura de componentes distribuidos, no hay distinción entre cliente y servidor. Cada componente es independiente y puede recibir o prestar servicios a otros componentes a través de un sistema de comunicación, conocido como middleware.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeGlbN4pxxsFtmewq5wQuM77r7PRobQrBiqP1pF291m4YMMEtL2Gn4KgXZ497yax-CKxr5cgUocWftbuBWOd3GVLAy3iSUuRyPGmMtNQXRFyisphcVqCNPsBSr_ZOkd1sm5sWlYqKVWFmbLY7DGMrAzkVbd?key=VReuh94fGGpJZLGsXsGdUQ)

#### Ventajas:
- **Flexibilidad:** Se pueden tomar decisiones sobre el lugar y forma de prestar los servicios más tarde.
- **Escalabilidad:** El sistema es fácil de expandir.
- **Reconfiguración dinámica:** Los objetos pueden migrar a través de la red según sea necesario, lo que facilita la reconfiguración en tiempo real.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSoEX3MNsFS03O224j-4xuRuTPOIwL713aRjLUFXCs8AMfQEhll9W2SbseGzPF2WJktlveSLns6U6NAZSKsW9SRUSd1AltCImOe0sF1VylYtkVWqYiIdxa6J5jtrQGeGcE_IJR-VNPdgv_BLS6HNybkCrT?key=VReuh94fGGpJZLGsXsGdUQ)

#### Desventajas:
- **Complejidad:** Son más difíciles de diseñar y comprender que los sistemas cliente-servidor.
- **Incompatibilidad de middleware:** No existe un estándar único para el middleware que permita la comunicación entre los componentes, lo que crea problemas de compatibilidad entre diferentes tecnologías.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeb1YoyzlGMO3HkEvz_Ms95unBi5IhtgFOvbkm4kd-PTn5xPStgXAJxGdfVQQANaJZ0_7dSFFc3fmepdkc__td1sOp53gST0LEylnTSLIvHdA61X-guLZDwyoU_TzPth0tW6RWC9MmqV-h080eEJZSvnu4K?key=VReuh94fGGpJZLGsXsGdUQ)

Como resultado, las **arquitecturas orientadas a servicios (SOA)** están reemplazando cada vez más las arquitecturas de componentes distribuidos debido a estos problemas.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfvXX_qvztM3UzWjL92r2k2S8Tz4X-kfJlqSE8E8uJGUBmzsyi804ScqE2PpJKDXX1MQ-oHBWsKLSryNTxIC4UvFmrKcSP9EcNfKZsrLtELT-UfrP0eOrpopDnrNmu2hGKGIk4LhzfZXhVZ9Sacb7Q0v-M?key=VReuh94fGGpJZLGsXsGdUQ)


---

### Peer to Peer (P2P)

Los sistemas Peer to Peer (P2P) son descentralizados, donde cualquier nodo de la red puede realizar cálculos. Estos sistemas aprovechan la capacidad de procesamiento y almacenamiento de muchos ordenadores conectados.

**Ejemplos:**
- **Intercambio de archivos:** BitTorrent
- **Mensajería:** Jabber
- **Pago:** Bitcoin
- **Bases de datos descentralizadas:** Freenet
- **Telefonía:** Viber
- **Computación distribuida:** SETI@home

**Modelos arquitectónicos P2P:**
- **Descentralizados**: Sin un servidor central.
- **Semicentralizados**: Con algunos servidores centrales.

**Usos comunes:**
- Cuando un sistema es intensivo computacionalmente y se pueden separar los cálculos en tareas pequeñas.
- Cuando no se necesita almacenar información de manera centralizada.

**Problemas de seguridad:**
- Los nodos maliciosos pueden enviar spam o malware.
- La falta de gestión centralizada puede exponer la información.

### Orientada a Servicios (SOA)

La arquitectura orientada a servicios (SOA) estructura un sistema como un conjunto de servicios distribuidos y sin estado, gestionados por diferentes proveedores.

**Componentes clave:**
- **Proveedores de servicios:** Ofrecen servicios a través de interfaces.
- **Consumidores de servicios:** Usan estos servicios.
- **ESB (Enterprise Service Bus):** Enruta y transforma mensajes entre proveedores y consumidores.
- **Registro de servicios:** Permite registrar y descubrir servicios en tiempo de ejecución.
- **Servidor de orquestación:** Coordina interacciones entre consumidores y proveedores.

**Conectores comunes:**
- **SOAP:** Comunicación síncrona basada en HTTP.
- **REST:** Utiliza solicitudes HTTP.
- **Mensajería asíncrona:** Permite intercambios de mensajes sincrónicos o tipo publicar/suscribir.

**Desventajas:**
- Sistemas complejos y difíciles de construir.
- Hay sobrecarga de rendimiento debido al middleware.
  
### Microservicios

Los microservicios son servicios pequeños, autónomos, ligeros y escalables que se combinan para formar aplicaciones completas.

**Características:**
- **Autónomos:** Sin dependencias externas.
- **Ligero:** Usan protocolos de comunicación simples.
- **Independientes:** Se implementan con diferentes lenguajes y tecnologías.
- **Desplegables independientemente:** Cada microservicio puede ser desplegado de forma independiente.

**Ventajas:**
- Flexibilidad y escalabilidad.
- Cada microservicio gestiona su propia base de datos y lógica.


## Aplicación Monolítica vs Microservicios

**Ejemplo: Servicio de impresión de fotos**

- **Monolítica:** Un solo bloque de código maneja todas las funciones.
- **Microservicios:** Cada función (como procesar fotos, gestionar pagos, etc.) es un servicio independiente, comunicándose entre sí.

Esta estructura modular permite actualizar y escalar los microservicios de manera más eficiente sin afectar al sistema completo.
