ARQUITECTURA

# Concepto

Es un esquema general de lo que va a tener el futuro sistema. Es algo abstracto compuesto por elementos y relaciones. Todos los sistemas modernos presentan algún tipo de arquitectura.

La arquitectura no lo es todo, todo el ciclo de vida determina la calidad del sistema.

# Arquitectura de Software

## ¿Por qué se necesita definir la Arquitectura de Software?

- Permite potenciar los atributos de calidad de un sistema. → Parte no funcional (seguridad, performance, modificabilidad, usabilidad, reusabildiad).
    

Básicamente según lo que nuestro sistema hará, se define la arquitectura. Por ej, si nuestro sistema debe ser seguro, se definen los elementos de tal manera que se resguarde el acceso a la información.

- Permite razonar y gestionar el cambio. → Modificabilidad.
    

Se habla de cambios en tres categorías:

- Local: Se cambia solo un elemento.
    
- No local: Múltiples cambios.
    
- A nivel arquitectura: Se debe cambiar todo el sistema.
    

- Su documentación mejora la comunicación entre las partes interesadas (Stakeholders).
    

La arquitectura es tan abstracta que cualquier parte lo puede entender. Es decir, el arquitecto escuchando los reclamos de los clientes, manager, etc. puede determinar la arquitectura.

- Contiene las decisiones de diseño más tempranas y difíciles de cambiar. 
    

Analogía: Después de armar una casa no puedo decidir cambiar la base porque debería tirar todo abajo.

  
  
  

- Define un conjunto de restricciones para su implementación.
    

Básicamente el arquitecto define un atributo de calidad a cumplirse, y se asigna x cantidad de recursos. Siempre y cuando cada parte no pase de ese umbral, el sistema cumple con la restricción impuesta por la arquitectura.

- Influye en la estructura organizacional o viceversa
    

Como es la base del sistema, todo se divide y se asigna la responsabilidad de cada grupo de trabajo.

Viceversa. Los grupos influyen en la decisión de arquitectura (ej experiencia de cada grupo).

- Para proporcionar la base para un desarrollo incremental.
    

En práctica es la realización de caso de uso parte del desarrollo iterativo e incremental.

Una vez definida la arquitectura, se puede hacer un sistema esqueleto, desde el cual se aplica el desarrollo iterativo incremental.

- Artefacto clave que permite razonar sobre el coste y el calendario.
    

Según la arquitectura, los costos y tiempo varían. Se pueden determinar por equipos, o el mejor arquitecto, project manager y devs.

- Puede crearse como modelo transferible y reutilizable que constituye el núcleo de una línea de productos.
    

Arquitecturas son modelos reusables, se pueden desarrollar múltiples sistemas con la misma arq

- Centra la atención en el ensamblaje de componentes, en lugar de simplemente en su creación.
    

Se pueden desarrollar componentes por separado, de forma dependiente o independiente, siempre y cuando cumpla lo que dice la arquitectura (restricciones).

- Canaliza la creatividad de los desarrolladores, reduciendo la complejidad del diseño y del sistema.
    

Aplicar restricciones en el desarrollo del sistema según el patrón de arquitectura, para simplificar el diseño.

- Puede ser la base para la formación de un nuevo miembro del equipo.
    

Referido al punto de mejorar comunicación. Cualquiera puede entender la arq.

  

# ¿Qué es la Arquitectura de SW?

Conjunto de estructuras necesarias para razonar sobre el sistema. Estas estructuras comprenden los elementos de sw, las relaciones entre ellos y las propiedades de ambos.

Arquitectura: Subconjunto de modelos.

Una estructura es un conjunto de elementos que se mantienen unidos por una relación. Una vista es la representación de una estructura

Un SW está compuesto por muchas estructuras y ninguna por sí sola es la arquitectura.

Todo SW tiene una arquitectura por detrás.

La arquitectura es abstracta. Los elementos no tienen una definición como tal, sino simplemente como se relacionan entre ellos y su comportamiento

Referido a la primera parte de la definición -> 

# Categorías de estructuras (vistas):

## 1ra Vista: Estructura de Componentes y Conectores

Son parecidos a los nodos de UML.

Se centra en la forma en que los elementos interactúan entre sí en tiempo de ejecución para llevar a cabo las funciones del sistema.

Los componentes son las unidades principales de cálculo (comportamiento en tiempo de ejecución). Ej: Servicios, peers, clientes, servidores, etc.

→ Es algo físico. Algo compilado.

Conectores son los mensajes en UML.

Los conectores son los vehículos de comunicación entre componentes (devolución de llamadas, operadores de sincronización de personal, etc.)

Publish-Subscribe = Publicador-Subscriptor: Es un patron.

Client-Server request/reply w/automatic failover: Esquema de cliente servidor con conmutación automática ante el fallo. Esto significa que se tiene un sistema principal y un backup.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeQYQH9Mm6h7W1boZQRn8r33EkudxnNdyD3utKzXCYzwsfZwMwNaXQHar7OUmUTqitWGVi9FbQBkwNWMnjoJ-n_2Q32pUINXowlwgNjSrHlvlOeb0Ksyb3SEkNCtm7QDMJy0HsMut4nR70t_UweOoP48Ntg?key=VReuh94fGGpJZLGsXsGdUQ)

## 2da vista: Estructuras de Módulos

Equiparable a vista de paquetes en UML

Muestra cómo se estructura un sistema como un conjunto de unidades de código o de datos que deben construirse o adquirirse.

Elementos -> Modulus. Tienen asignada una funcionalidad en específico

No hay interés del tiempo de ejecución.

  
  
  
  
  
  
  

A la izquierda una estructura y a la derecha una estructura de capas (layer).

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdCSdbyqTL7OWW6Zbh5nBFDeRg38flP0HuojTp4pNd7D6Gk50l3jOuRNnIM5GC7n28UEeIs1AT8bwifrMCdKjrKxC_uYCzof9B4c2Z976aIdSK99I0Jc2ui_rYH4vmzXZPDEACVNPXRpAHrALouvySi0WB1?key=VReuh94fGGpJZLGsXsGdUQ)

- Direccion de las flechas: Acceso de uso.
    
- En blanco: Capa a nivel de usuario.
    
- En gris: Capa a nivel de núcleo del sistema.
    

## 3ra vista: Estructuras de Asignación

Equiparable a vista de despliegue en UML.

Establecen la asignación de las estructuras de sw a las estructuras no relacionadas con el sw del sistema, como su organización o sus entornos de desarrollo, prueba y ejecución.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcVOvapcWTLfFxsHSnxIIEt2BKkcMMdSHgIXicgyZI8olEIT5JChfV7gYWQNNbc3sUqiuZNQHfMc3bWilF0bCgL_JRn6ia6R30JpxfK1NW49KVqVR3tfwX4Cqqg9FPeXv9jM1kXxODUTkDJXOXC37lbupm4?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  
  
  
  
  
  
  
  
  

Modulos

Se aplican a la vista según el atributo de calidad que se quiere conseguir.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdOTdA4hU4tbPQFGnBlSCkxIrilFq-L1SoOFy6leNlETbXZmegtSP7TL1PecOCPl1A_Ei0jhgg9LIHtDky1wvpG3p1sLC4PwflmET8Z6k-azx4LYsm3FCpX-B0EigO7RNLYvzrEkDITfdRqbMrNsJhhhkb_?key=VReuh94fGGpJZLGsXsGdUQ)

## ¿Cómo se relacionan las vistas?

Cada una de estas estructuras ofrece una perspectiva y un control del diseño de un sistema diferentes, y cada una es válida y útil por derecho propio. Aunque las estructuras ofrecen distintas perspectivas del sistema, no son independientes. Los elementos de una estructura se relacionan con los de otras y es necesario razonar sobre esas relaciones. Por ejemplo, un módulo en una estructura de descomposición puede manifestarse como uno, parte de uno o varios componentes en una de las estructuras de componentes y conectores, reflejando su alter ego en tiempo de ejecución. En general, las correspondencias entre estructuras son de muchos a muchos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfWxs4jthmqPCw4m4NnmAe8tY5wZ2_uKy6UbDoF7H9ILTFZqS1RQC_gyjZLBnj-G51GGi_C3Tl1_R2YApA1nytMcxCdxuRom4ggsBZT2OHYAFeDZrk1e29ddMhRrsiKHEvAEs_WgQ?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  
  
  

Ejemplo: Dos vistas para un mismo sistema de tipo cliente-servidor: A izquierda estructura de módulos (descomposición) y a derecha estructura de componente-conector.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd4E-MEJuq4O9rZgwROhm0eIEG5-U5_StZ2Dlirj2flWBX5oUrWXzgCBgK1Qo78O7rIg4D1nrSbq6MWEi7lDRzmQVc7HSqB1oCRxKz3UZ9qILg36p5NKuwKaeUKHa_V9K2l-XJi_vg5uqOJLJwMfscIBJ--?key=VReuh94fGGpJZLGsXsGdUQ)

# Diseño Arquitectónico

Se ocupa de comprender cómo debe organizarse un sistema de sw y diseñar la estructura general de ese sistema. nexo crítico entre el diseño y la ingeniería de requisitos, ya que identifica los principales elementos estructurales de un sistema y las relaciones entre ellos.

La funcionalidad no determina la arquitectura.

Diseñamos nuestro sistema como conjuntos estructurados de elementos arquitectónicos que cooperan (módulos, capas, clases, etc) para hacerlos comprensibles y admitir una variedad de otros atributos de calidad. (DEV COMPONENTES)

La arq en lo pequeño se ocupa de la arquitectura de SW de los programas individuales.

La arq en lo grande se ocupa de sistemas distribuidos, sistemas empresariales complejos.

  
  
  
  
  

## Flujo del Diseño Arquitectónico

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe8yQPGOv0DQ0E8B5OcqDAiRvffwXkuKmxAF0fGZ2Xc3IHXPx5JiimagSZSCkHkqPjiudRb4PeOh9GtKegfRONQR_1Wxg_Q8TnlSBbX2K_pFzFp1ukCxlOvCFPqti84vYBdxPSYrKQOeSur32FMeXVxBxc?key=VReuh94fGGpJZLGsXsGdUQ)

## Decisiones de Diseño

Ver a la arquitectura como un conjunto de decisiones. Preguntas clave para elegir y sobre todo diseñar la arquitectura.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcXW2FoX_JeE_v4Fh5rRRMEqZ3f2NSZboCP4-GLSz5cQGwdmL1gB0r2qCNtkQPpme8KKxmnn08GJKdszMsXBSNtROI_LXgIXrfjzeu-S4tCSo6W8vX2a5upd25k7mLVrLcUVPs9_rJOeapUf3PsuoqiqRNp?key=VReuh94fGGpJZLGsXsGdUQ)

## Vista 4+1 (Krutchen)

Modelo diseñado para describir la arquitectura de sistemas software, basado en el uso de múltiples vistas concurrentes. Las vistas suelen describir el sistema desde el punto de vista de diferentes interesados, tales como usuarios finales, desarrolladores o directores de proyecto. Y el más uno sería la vista central que describe la arquitectura mediante la vista de casos de uso.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfVDUcErSuex7uo4TI6nUm3nG_NmIvoHxCyiGVNxSD6NrOWUVZfMzUZ0bm-YsxjCTQlLj7eqTyAFEg52ZV_p52RkR_i5QNcLZGgHXjRUgeT6o0tgk97MU2OqoJSB496Ps2-hmrfDE5L8T_Nj4S1vRYouBSg?key=VReuh94fGGpJZLGsXsGdUQ)

[https://www.youtube.com/watch?app=desktop&v=r8ucofiI8vY](https://www.youtube.com/watch?app=desktop&v=r8ucofiI8vY)

## ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeLl253f0Q0UhTwnGJZbNZQVyZhSLh_3GifQ6gOOYGQvtzJ5SbOMVWQYktTs0puWB3jYXUsKJekpdSpBjlp4l0Ce24Q7qSNOrx98DPk2MxUdRV7YMm_bsyS1bhnxCcz6hDhxouFIAA2BIzkrK5b99RsC029?key=VReuh94fGGpJZLGsXsGdUQ)  
  
  

  
  
  
  
  

## Estilos Arquitectonicos

Define una familia de sistemas en términos de un patrón de organización estructural. [Garlan y Shaw].

Determina el vocabulario de componentes y conectores que se pueden utilizar en instancias de ese estilo.

Un patrón arquitectónico es una descripción estilizada y abstracta de buenas prácticas, que ha sido probada en diferentes sistemas y entornos [Somerville].

## Patrones de Arquitectura (Centralizados)

### En Capas (Layered)

Se la considera monolítica: ensamblada en un solo bloque de código, archivo o ejecutable.

El patrón por capas divide el software en unidades llamadas capas.

Cada capa es una agrupación de módulos que ofrece un conjunto cohesivo de servicios.

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcvDXvT1Xwr7LbmksaAk6LzwUDzLLpEsEym73z-vhsTv3k674tAnAXFDOz981zIdSo1d8pTnEVUyl2s37L6vPQMDM5Dd_ZBKXBZT8UExEiBlBoQTMyBprohTS8bpPQydwSRr3KnDAiT2Z_TihqKA-iq9Yfz?key=VReuh94fGGpJZLGsXsGdUQ)

- Una forma de lograr la separación e independencia.
    
- La funcionalidad se organiza en capas separadas.
    
- Cada capa depende de la capa inmediatamente inferior.
    
- Cada capa es independiente de las capas superiores.
    
- Desarrollo incremental de sistemas.
    
- Cambiable, una nueva capa puede reemplazar una capa existente (siempre y cuando las interfaces no se modifiquen). Modificable
    
- Portable, ya que los sistemas en capas localizan las dependencias de la máquina, implementaciones multiplataforma.
    
- Una separación limpia entre capas suele ser difícil.
    
- El rendimiento puede ser un problema.
    
- RIGUROSAMENTE cada capa solo puede comunicarse con la inmediata superior e inferior NADA MÁS.
    

LAYER y TIER SE TRADUCEN COMO CAPA

- LAYER: Capa lógica.
    
- TIER: Capa física o de implementación.
    

Mensajes de abajo hacia arriba: Asincronicos, no se espera una respuesta para continuar.

Mensajes de arriba hacia abajo: Sincronicos, se espera una respuesta para continuar.

La capa vertical de la derecha indica la infraestructura (por ej. el lenguaje que se utiliza), refleja que en la realidad es imposible utilizar un modelo riguroso de capas.

Ejemplos:

- Modelo OSI.![OSI Model 7 Layers](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcYB1KAdBiHDoY8u4-uWceCw5mdHW_6_IFOBsCRKf7-svmhzsf2HgJPgISx0qY_qvBY4BqpD2J4dbfoRBkh6pEfjnvDULM87GAmWFEMMap6PoLSrC69umgi4oYEp8Jl4n0vxe5a0HrWa2hMFCOBLQsO8c8_?key=VReuh94fGGpJZLGsXsGdUQ)
    
- Un diagrama de capas sencillo con una clave sencilla que responde a la pregunta de usos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXezYHGEVSHHsxQbd5P0ln3uogQjzwVr4H9PvGmv6aLX5MADdIccY-i8N8YO7KO_OcOzCxmOgehzhOyBOvDqFVCqXkxJWWC0GtFv71-3CzC-O4SLACQl2ydQ7yYh0xXfqmuC1qhA01K-Wvdsw4FzIo53E8JF?key=VReuh94fGGpJZLGsXsGdUQ)
    

  

- Un lobo vestido de capas.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeaOIzZ_k2kXt5OB_k142eJie-gdCb6nQe4aTybL9ytf8EAMScyME3z27uqaquR0tesLhTOlLb3znOySmqsgW6n44pjzUvJ-cOob93TTSNjlTdS_3gvOSvUcKouLzxBSStcEdGatLNZSNnOLvVqxNoVPiI?key=VReuh94fGGpJZLGsXsGdUQ)
    

Esto no es un diseño por capas porque al estar todo conectado todas las capas dependen de todas y hay dependencia total.

- Capas con un lateral.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeIAPy28Frv1eYIX_MgUqLwz7zEy2-Lr8P0akeD26IThPAFB6lTgEOVfXmh8UCjyhGrdrnKZRDIvpABeH5xmbHc9DYHzibP20A_fSK5MhrJmjkj9lWwNvwTquXEcExFxZ766-rG72OW1tOqq6ZRexLCdcw?key=VReuh94fGGpJZLGsXsGdUQ)
    

La capa D contiene cosas comunes que necesitan todas las capas (manejo de errores, métodos de acceso a BD, etc.).

- Diseño de capas con capas segmentadas![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdhinKoK9Xabhnb-BXOUaXe8fiUUwrLNartrOJyWVIvdzjZGvLcgdpFtjOfK3bhQWvM1Lx6o4pGFEdLBrk5WfcVY-4NG9-Ln3crNamLW066K-fT9gr6iRzUEHgaKgr3DPX926jCzAoW3m5KCIepRBMkWrbM?key=VReuh94fGGpJZLGsXsGdUQ)
    

Los segmentos de la capa superior no pueden utilizarse entre sí, pero sí los segmentos de la capa inferior.

### Repositorio / Pizarrón (Shared-Data)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe5cKggUQQO-IwcXDSUowQt6xDW2B76eBYXW_m7DzNWMIvYU_iuz9as0jC9EIuuZ2n5OtaxkJ91hLr4EFcpUrfisQ3y-IFKloa9Urxe7RBRwSMj2QiNkZjXSMwy8xZDp_DTHkHgsTFCPCgwV13dE4MQVPvk?key=VReuh94fGGpJZLGsXsGdUQ)  
Los componentes independientes se comunican a través de un repositorio de datos central (tmb componente).

Los componentes independientes no interactúan directamente.

Todos los datos se pueden administrar de manera consistente.

Conviene cuando:

- Se generan grandes volúmenes de datos que tienen que ser almacenados durante mucho tiempo (repositorio-pasivo).
    
- La inclusión de datos en el repositorio desencadena una acción (pizarrón-activo).![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcjqT1TS2iqv3n8UnE9JlvOoiTCvcjaLAf7IFHXo66DoJilKs7fr5eOkjTuYqS_FMwaJsaSc9lduwGb54ZDq1OjzJuMLZV7OOEkhM2PDXUDyqpw7p8Y7Y0raM-V7s5G59ryrS_lC5WR_dJVX9CsFFTIZl4?key=VReuh94fGGpJZLGsXsGdUQ)
    
- Lo uso cuando tengo datos y necesito trabajarlos en conjunto.
    

Desventaja:

- Cuello de botella.
    
- El repositorio es un único punto de fallo (afecta a todo el sistema).
    

  
  
  

Ejemplo: IDE con varias herramientas y un repositorio con control de versiones.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdAStlJUAVrQ7YCsC5T8qtEfwXW0B2SbtT_ijlTZbpog9VCJ4g2ltbPMEoPL1s6lwA4GLuBYP2ncAmUQ3OwfRa8eR55Bx5qvxyabQlkUUtUVB989G_ROmxFw3Xm0tUBL6EDZ2gFT4lyDzHceBOO7De3PF4?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfoDLAc4LIldd9LfpRJqRkhXQ_WQZtuYelVOC72hYu7wIEtr6OPvhEMBXDBNC6PCNcCQHRhzHEhPEM9flEiBmcMVCxUaJRzFPMwLmc3LgJmSVAfLHEboRPU1nC1_oEXjGJfk-fx1uB1QW_ma_9QsNrxlp4?key=VReuh94fGGpJZLGsXsGdUQ)

### Pipes and Filters  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdts2MCUFfcb47IAS3BhkkUDdMC3V_GpMxuMWGu-8Ua55XtsVrSr7bRMpZEJblUsr2-2frW0sIbmRli91AO34tRWLZSaksNeuX4nwoACbEF73WQp4dN8QEsZ_mOiHL9O4cE3xl_7mwNFRAFOOg-LY-jDOVk?key=VReuh94fGGpJZLGsXsGdUQ)

Arquitecturas de tuberías o filtros o canalizaciones → PIPELINES.

Voy a usarla cuando necesite funcionalidades o transformaciones sucesivas sobre un conjunto de datos.

Cada componente tiene un conjunto de entradas y de salidas.

Filtro: Produce un resultado aplicando una transformación local a los flujos de entrada y calculando de forma incremental (usualmente) para que la salida comience antes de que se consuma la entrada.

Tubería: Es un conector entre filtros, conducto para los flujos de datos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXequw2ocNINL63a2kbJRtIHuA_xF95GVD7Z5kFGbXfzj1zdwfsl5TgSYpREd2OCcQxPGj_s1vMsUdD9YYv3kJRPJKL2uzzQnpgnwGILDe9qBiwpLAkCGhHD036F0yQORktMBRoKVh_Q98-IKfEEovRZo7uu?key=VReuh94fGGpJZLGsXsGdUQ)

d![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfBfAgGn8ylTeTp6FrsT2Dvx5T1RO1as5zSDtpqsEKQCigkwc0ID2a-cmHuqQUihhQERIPTap9xPZ4_OhlH9EPRjhvB366mLbs7T82I7aTRL3uwYubB6i8XyDUJS1PUzucpuS7K0FNCtkMBX0jvps-OBXGi?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  

### Microkernel / Plug-in

Consta de un sistema central y plug-in’s que proporcionan extensibilidad, adaptabilidad y aislamiento de las características de la aplicación y la lógica de procesamiento personalizada.

Sistema Central: Componente con la funcionalidad mínima requerida para ejecutar el sistema.

Plug-ins: Componentes independientes y autónomos que contienen procesamiento especializado, características adicionales y código personalizado destinado a mejorar o ampliar el sistema central.

La comunicación suele ser punto a punto.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe40Q8tAAHgXvucrGEeyuRbQAALCe1vky9OV3iHuKwCcxsOXcrnFJ7ucQpezeI_XQATcENbun3ZoLAuH97iQnEV_N182L3in-BV5SanynOGM8Ax7LyLob9cDC_l6wPpJDbqnSgfKiRkdXfPOrUu7k__7QZo?key=VReuh94fGGpJZLGsXsGdUQ)

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe74dBfHe8w0dTOaNueRTnBdZcBvyJc8vJf3lstrmJSIOKdQXAloHziXE67QGBqEPmxr2vf6y3dstFg7DcMylQRoO5Zkia4Po-Nn-vUM51ZRSWfUPGrOaOY9W7saBYFSCc5mRRZnCxcLHrkfh97-6HuVjo?key=VReuh94fGGpJZLGsXsGdUQ)

- El estilo de arquitectura de microkernel es flexible y extensible, permitiendo agregar fácilmente funcionalidad y características adicionales a una aplicación existente.
    
- Los módulos complementarios son componentes independientes que contienen lógica de procesamiento especializada, características adicionales, lógica de adaptador o código personalizado que mejora o extiende el sistema principal.
    
- El sistema principal necesita saber qué módulos complementarios están disponibles y cómo acceder a ellos, a menudo a través de un registro de módulos complementarios.
    
- Los módulos complementarios se pueden implementar de varias maneras, ya sea como bibliotecas/módulos separados, dentro de un solo conjunto de código consolidado o como servicios remotos.
    
- Se basa en iterativo incremental.
    
- Bajo costo, simple de entender.
    
- Se presentan cuellos de botella. No es muy apto para sistemas que requieren alta escalabilidad o elásticos.
    
- El core es el punto de entrada, por lo tanto también es un vector de fallo bastante grande.
    
- Si siempre se modifica el core, este patrón no es el apto.
    

Resumen: La funcionalidad del CORE es extendida mediante los Plug-ins. La idea principal es definir el Core de manera tal de no volver a modificarlo.

Ejemplo: Google Chrome tiene funcionalidad básica y las extensiones agregan funcionalidad.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfy0GieYQau9IJ6TH9JcYjDuwoKVIm_N04IhvsPxHJCZjwWnfIVh0FIY_mHjaMagEG55e4o4QRfZVHRO0ICnsi6WTTgLTmkmuY2YYVmbApIsmaV65jeYR6JfzhLojN6l7QEZohNId4RcY0lcxRfbn0s71dQ?key=VReuh94fGGpJZLGsXsGdUQ)

## Sistemas distribuidos (CONCEPTO)

Un sistema distribuido es un conjunto de ordenadores independientes que aparece ante sus usuarios como un único sistema coherente. ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcWz93LGfYyNKyE8t7TXIv82fXFcff_IPDLD1tb209MASrB6ywwlVLHJufyOorAExwV75uWELCjeHwgi1PtNa9zYN45Wo6kBq7wrr_sg47rNcriYn5WZTCuGt3y64cInxGq4l_Pxwq-hYZHR720lIqhuYhe?key=VReuh94fGGpJZLGsXsGdUQ)

La idea es separar al sistema en varios nodos o componentes (computadores), solucionando el problema de cuello de botella o tolerancia a fallos que tenían algunas arquitecturas. Además, el usuario nunca se debe enterar, solo debe ver el sistema como tal.

Objetivos de los Sistemas Distribuidos (Ventajas):

- Recursos compartidos: Lo principal es que reduce costos, pero a medida que crece, también hay que ver la seguridad.
    
- Transparencia: Es ocultar el hecho de que sus procesos y recursos están físicamente distribuidos en varios ordenadores.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVCKmHjzUyJmhfzfbXFEFVtB9ZCw_JK3QXHMwGRIqeZ0mVhFvE7hgW5mfISEDKkDJljPt6F0X_A_g-9VJEkj-TBBnfHmQKPE2z4rl45J-nOVeA_i5UktMCtlzLTJRa0hYah0D2ivKQLNRUQKrPtiDVfTU?key=VReuh94fGGpJZLGsXsGdUQ)
    

La transparencia nunca se puede conseguir al 100%, incluso en algunos casos no conviene conseguirla.

- Apertura: Es un sistema que ofrece servicios de acuerdo con reglas estándar (Lenguaje de definición de interfaces) que describen la sintaxis y la semántica de dichos servicios. Por ejemplo, en las redes informáticas, las reglas estándar rigen el formato, el contenido y el significado de los mensajes enviados y recibidos. Estas reglas se formalizan en protocolos.  
    La interoperabilidad caracteriza el grado en que dos implantaciones de sistemas o componentes de distintos fabricantes pueden coexistir y trabajar juntos simplemente basándose en los servicios de la otra parte, tal y como especifica una norma común.
    
- Concurrencia: Los procesos pueden funcionar simultáneamente en equipos separados. Los procesos pueden comunicarse entre sí.
    
- Escalabilidad: Puede medirse en al menos tres dimensiones:
    

- Escalable con respecto a su tamaño, lo que significa que podemos añadir fácilmente más usuarios y recursos al sistema.
    
- Escalable geográficamente es aquel en el que los usuarios y los recursos pueden estar muy alejados.
    
- Administrativamente escalable, lo que significa que puede seguir siendo fácil de gestionar aunque abarque muchas organizaciones administrativas independientes.
    

Desgraciadamente, un sistema escalable en una o varias de estas dimensiones suele presentar cierta pérdida de rendimiento a medida que se amplía. (más datos a manejar, peor rendimiento)

La vinculación de red (conectar todo para tener el sistema) limita la escalabilidad. Al conectar las computadoras, depende como se haga, la escalabilidad que tendrá el sistema va a ser una.

- Tolerancia a fallos: Disponibilidad de varios equipos y posibilidad de replicar información (redundancia).
    

Algunas Desventajas:

- Complejidad: Difícil de entender sus propiedades emergentes y de probar, p. ej., el rendimiento dependiente de un procesador vs dependencia del ancho de banda de la red y de varios procesadores.
    

- Seguridad: Acceso desde varios ordenadores diferentes, espionaje del tráfico de red. Es difícil garantizar la integridad de los datos. Degradación por ataques de denegación de servicio.
    
- Manejabilidad: Diferentes tipos de computadoras, diferentes versiones del sistema operativo. Los fallos pueden propagarse a otras máquinas. Se requiere más esfuerzo para mantener el sistema en funcionamiento.
    
- Imprevisibilidad: La respuesta depende de la carga global del sistema, de su organización y de la carga de la red.
    

  
  
  

Formas muy utilizadas de organizar la arquitectura de un sistema distribuido:

### Arquitectura Maestro/Esclavo

Las arquitecturas maestro-esclavo se utilizan habitualmente en los sistemas en tiempo real con plazos de procesamiento, en los que puede haber procesadores independientes asociados a la adquisición de datos del entorno del sistema, al tratamiento de los datos y a la gestión de los cálculos y los actuadores. También se utilizan en replicación de BD.

Arquitectura maestro-esclavo, que se utiliza en sistemas en tiempo real en los que se requieren tiempos de respuesta de interacción garantizados.

Proceso Maestro: Responsable del cálculo, la coordinación y las comunicaciones, y controla los procesos «esclavos».

Procesos Esclavos: Dedicados a acciones específicas, como la adquisición de datos.

Adecuado para el procesamiento distribuido predecible, requisitos de alto rendimiento, tolerancia a fallos o precisión.

Los procesadores esclavos se encargan de las operaciones computacionalmente intensivas, como el procesamiento de señales y la gestión de equipos.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcJlcGh8HNDCcfoQix9FjJD_92zYyJgqRwY8hec8nmQxAQmZM0sP93V7f3WDPW-tIMFo3LoRWZWzquWgPveY301fRPGY9O3BcNsHnoCksO-d-qu4I5NDb6odLAuymUR2EKC_U1u3njX8Wtge8wK25EXqRjn?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  

### Arquitectura Cliente Servidor

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXegDFVtG_ubIKFYwqyVyWF9zRBY7_4DbU8-KehbhOu-JaaKoQWtHfiQC1qblx9A7MknRmHTLr8DTEWfDOJxyQ_24UdXTr1XMdq2X_UApngqfmt3qb9r29OcnT4MCXgVoQqImAYhHGPjp6LaUDVhYvr9MUY_?key=VReuh94fGGpJZLGsXsGdUQ)

- La aplicación se modela como:
    

- Un conjunto de servicios proporcionados por servidores.
    
- Los clientes pueden acceder a estos servicios.
    

- Los clientes conocen a los servidores, pero no se conocen entre sí.
    
- Algún mecanismo de descubrimiento de los servidores.
    
- Los servidores no conocen a los clientes (a priori).
    
- Los servidores pueden o no tener estados.
    
- Los clientes y los servidores son procesos separados, en la misma máquina o en máquinas diferentes.
    

Los clientes interactúan solicitando servicios a los servidores, que proporcionan un conjunto de servicios. Algunos componentes pueden actuar como clientes y servidores. Puede haber un servidor central o varios distribuidos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdBTE-QYRiY1xft7DCmUUEdmAnHWHLpa4z2Z52t9Gg_ZFMjS3aeOSXTAFY0XZFG8qPn4-84NHi_JzyeSW8sCII4AJt-xf-CYxHInlzv6VT9_Q2ngoVOQlCUjF_p2xUdxQAGQXXCTFqqlzZQZzmybfTNnZs?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeDnX-EV8M-t5WeLyW6oG8ifdI3-w-RhN0caGtFqv5OHy97qHF5uGWA1R_0P-idJ8RkyUZhY568f8Uz-0ZWXu7yW8MC6M77yyNOT0EDkudXEB97bPmpywsGgxs3n-bGAxS9xcitlCaHlFYqqpgQJgFRr_YU?key=VReuh94fGGpJZLGsXsGdUQ)

Servidores tiene servicios usados por clientes

Internet es el ejemplo más facil, HTTP seria el conector, cliente el navegador, servidores de internet  
  

### Arquitectura C/S (Cliente-Servidor) de dos niveles (2-tier)

En una arquitectura cliente-servidor de dos niveles, el sistema se implementa como un único servidor lógico más un número indefinido de clientes que utilizan ese servidor.

Dos formas:

Cliente liviano: Capa de presentación en cliente, el resto en el servidor. La capa de presentación se implementa en el cliente y todas las demás capas (gestión de datos, procesamiento de aplicaciones y base de datos) se implementan en un servidor.

- Fácil gestión de clientes.
    
- Gran carga de procesamiento en el servidor y en la red.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbnL1ctWIt5bReegKxMn5i96O7EPC9VpOKgy7xJqs3tKeYBo5G71HRNM7E5Slb1e0mONFXlsgdMjhrQJKjJu4POfduft-RvpZUfl5je0e-54AlO8gACQE4VvfReFMwOlg_XJXdELlHt83objdXb8bCuDQ?key=VReuh94fGGpJZLGsXsGdUQ)
    

Se utiliza cuando los sistemas viejos se migran a arquitecturas cliente-servidor. El sistema viejo actúa como un servidor en sí mismo con una interfaz gráfica implementada en un cliente.

Su principal desventaja es que supone una gran carga de procesamiento tanto para el servidor como para la red.

Cliente Pesado: Capa de presentación + aplicación en cliente. datos en servidor. Una parte o la totalidad del procesamiento de la aplicación se realiza en el cliente. Las funciones de gestión de datos y bases de datos se implementan en el servidor.

- Hace uso de la potencia de procesamiento disponible en el cliente.
    
- Se necesita desplegar y mantener el software en el cliente.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfp-zHCBvFKdMfLZ5OIN5bRH56D_s9gwTEshXpkAMJ-cOm_WkyZbH2YTt_KwRwlVxpISGWDOJeptiZ20d_6dVAXdVclnb6vCPUJJ9ZBgRbY2tijf6nOtC-LyYthce_e9pztoLdJq4QROfEFGKn8BH5wIwXQ?key=VReuh94fGGpJZLGsXsGdUQ)
    

Se delega más procesamiento en el cliente, ya que el procesamiento de la aplicación se ejecuta localmente.

Más adecuado para nuevos sistemas C/S en los que las capacidades del sistema cliente se conocen de antemano.

Más complejo que un modelo de cliente ligero, especialmente para la gestión. Hay que instalar nuevas versiones de la aplicación en todos los clientes.

###   Arquitectura C/S multinivel (multitier)

En una arquitectura cliente-servidor multinivel, las distintas capas del sistema, a saber, presentación, gestión de datos, procesamiento de aplicaciones y base de datos, son procesos separados que pueden ejecutarse en distintos procesadores.

De este modo se evitan problemas de escalabilidad y rendimiento si se opta por un modelo thin-client de dos capas, o problemas de gestión del sistema si se utiliza un modelo fat-client.

Desventajas: su coste y complejidad. En sistemas sencillos, las ventajas de la arquitectura multinivel pueden no justificar sus costes iniciales y continuos, en términos de hardware, software y complejidad de diseño e implementación.

Los niveles no son componentes, sino agrupaciones lógicas de componentes. Tampoco hay que confundir niveles con capas. Las capas son un patrón de módulos (una unidad de implementación), mientras que los niveles sólo se aplican a las entidades en tiempo de ejecución.

###   Componentes distribuidos![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeGlbN4pxxsFtmewq5wQuM77r7PRobQrBiqP1pF291m4YMMEtL2Gn4KgXZ497yax-CKxr5cgUocWftbuBWOd3GVLAy3iSUuRyPGmMtNQXRFyisphcVqCNPsBSr_ZOkd1sm5sWlYqKVWFmbLY7DGMrAzkVbd?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdSoEX3MNsFS03O224j-4xuRuTPOIwL713aRjLUFXCs8AMfQEhll9W2SbseGzPF2WJktlveSLns6U6NAZSKsW9SRUSd1AltCImOe0sF1VylYtkVWqYiIdxa6J5jtrQGeGcE_IJR-VNPdgv_BLS6HNybkCrT?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeb1YoyzlGMO3HkEvz_Ms95unBi5IhtgFOvbkm4kd-PTn5xPStgXAJxGdfVQQANaJZ0_7dSFFc3fmepdkc__td1sOp53gST0LEylnTSLIvHdA61X-guLZDwyoU_TzPth0tW6RWC9MmqV-h080eEJZSvnu4K?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfvXX_qvztM3UzWjL92r2k2S8Tz4X-kfJlqSE8E8uJGUBmzsyi804ScqE2PpJKDXX1MQ-oHBWsKLSryNTxIC4UvFmrKcSP9EcNfKZsrLtELT-UfrP0eOrpopDnrNmu2hGKGIk4LhzfZXhVZ9Sacb7Q0v-M?key=VReuh94fGGpJZLGsXsGdUQ)

En una arquitectura de componentes distribuidos no hay distinción entre clientes y servidores.

Cada entidad distribuible es un componente independiente que presta servicios a otros componentes y recibe servicios de otros componentes.

La comunicación entre componentes se realiza a través de un sistema middleware.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLf7Qv07SUV9iHKOr3jLthdHKRG9TZb-laGgpim2cOA1i79TBWy3VJxd2QAxark5xLpeTCWYNa2QuTMTpC59BpMOslPjZQQQXc6j3RLuuCqc4clKitUpxqUAGL9x_vL6SAKdGLnmKANrGm6ch-4sAVM9an?key=VReuh94fGGpJZLGsXsGdUQ)

Ventajas:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdjiGS9YRdPkuE7jQ1vfk-gV8YzbgJrMddQ3GTqCaBewUDf-s7XL7ENpRC-_WIdOSJC4TWzNMvLcymNjU5NH1iqoiQNl2m6MOhTOHp-iLmLFy62NMzSWnPw3mz9N604xtnchgpuId0l9ylrmgGdaeppymiC?key=VReuh94fGGpJZLGsXsGdUQ)

- Permite al diseñador del sistema retrasar las decisiones sobre dónde y cómo deben prestarse los servicios.
    
- Es una arquitectura de sistema muy abierta que permite añadir nuevos recursos según las necesidades.
    
- El sistema es flexible y escalable.
    
- Es posible reconfigurar el sistema dinámicamente con objetos que migran a través de la red según sea necesario.
    

Desventajas:

Las arquitecturas de componentes distribuidos adolecen de dos grandes desventajas:

- Son más complejas de diseñar que los sistemas cliente-servidor. Las arquitecturas de componentes distribuidos son difíciles de visualizar y comprender.
    
- El middleware estandarizado para sistemas de componentes distribuidos nunca ha sido aceptado por la comunidad. Diferentes proveedores, como Microsoft y Sun, han desarrollado middleware diferente e incompatible.
    

Como consecuencia de estos problemas, las arquitecturas orientadas a servicios están sustituyendo a las arquitecturas de componentes distribuidos en muchas situaciones.

### Peer to peer (P2P)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd6HLgXjYJ7pXBxi2aXHBz2hp_9aF_RybcZKSk3QmFov6xvnDUwY6FOzxlU0XUAbJjTXfCkeb-CgJWi2JYJl3RWwCIsN4hVfm07O6pvj1PW79unz_OVMTQN4g_Sq7sLlp0JrK7tk-7XTqSjlfJUhvzed1tJ?key=VReuh94fGGpJZLGsXsGdUQ)

Los sistemas peer to peer (p2p) son sistemas descentralizados en los que cualquier nodo de la red puede realizar cálculos.

El sistema en su conjunto está diseñado para aprovechar la capacidad de cálculo y almacenamiento de un gran número de ordenadores conectados en red.

La mayoría de los sistemas p2p han sido sistemas personales, pero cada vez es mayor el uso empresarial de esta tecnología.

Sistemas Peer-to-peer

- Sistemas de intercambio de archivos basados en el protocolo BitTorrent
    
- Sistemas de mensajería como Jabber
    
- Sistemas de pago - Bitcoin
    
- Bases de datos - Freenet es una base de datos descentralizada 
    
- Sistemas de telefonía - Viber
    
- Sistemas de computación - SETI@home
    

  

Modelos arquitectónicos Peer-to-peer

- La arquitectura lógica de la red.
    

- Arquitecturas descentralizadas.
    
- Arquitecturas semicentralizadas.
    

- La arquitectura de las aplicaciones.
    

- Organización genérica de los componentes de una aplicación p2p.
    

- Se centra en las arquitecturas de red.
    

Arquitectura p2p descentralizada                                            Arquitectura p2p semicentralizada![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcF7Xck6GdXlbZOYaoizHiGEm9O1Yg-JAEb3HDWUQy65h2c8cF2hxcQc1umbwI4Q3c_6rKC-RRcjxnwdrbKjq4s4pBep-Kg6-dKwZaG3p64ZPP6LRQzATeCkvEqwixxaHeqUrv1K2qRjvYWY0uVRi1adFzn?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXccCY-LhxEYkFvienS_tlx6RvJNbJ1j0cQblROrlIy-HPLzbuH_iY3cUknUdQhFneO6d0SFzvYtUcGm3HT2eF7VV3IOU2IwEW7y_3GLuRLbXXHnlRvN4ZzR4oWr8vehONbgZLHmT8tbTyfAvL-h6oz8bnQ?key=VReuh94fGGpJZLGsXsGdUQ)

Cuando se usa una arquitectura p2p

- Cuando un sistema es intensivo desde el punto de vista computacional y es posible separar el procesamiento necesario en un gran número de cálculos independientes.
    
- Cuando un sistema implica principalmente el intercambio de información entre ordenadores individuales de una red y no hay necesidad de que esta información se almacene o gestione de forma centralizada.
    

Problemas de seguridad en el sistema p2p

- Los problemas de seguridad son la principal razón por la que las arquitecturas p2p no se utilizan de forma generalizada.
    
- La falta de una gestión centralizada permite a los nodos maliciosos enviar spam y malware a otros nodos de la red.
    
- Las comunicaciones P2P requieren una cuidadosa configuración para proteger la información local y, si no se hace correctamente, ésta queda expuesta a los demás usuarios.
    

### Orientada a Servicios (SOA)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeo20qJBaQn_pchg0ngstvRrmCk8QKjfAhIMKS2CPSQPZOv3I2dekmuceLZV31Ts_v9zQP73poaObqZ0vCpdC6ZrOMfEqzYUnr5SyDNncWUu6BRFc_Lnd1-ReGUq8S9pR6foGCK9vPvxHTa8_SaFHLRTzfd?key=VReuh94fGGpJZLGsXsGdUQ)

La arquitectura orientada a servicios es un enfoque para estructurar un sistema de software como un conjunto de servicios separados y sin estado, que pueden ser proporcionados por múltiples proveedores y pueden estar distribuidos.

Normalmente, las transacciones son cortas: se llama a un servicio, éste hace algo y devuelve un resultado.

La computación se consigue mediante un conjunto de componentes que cooperan y que proporcionan y/o consumen servicios a través de una red. El cálculo suele describirse mediante un lenguaje de flujo de trabajo.

Elementos:

Componentes:

- Proveedores de servicios que proporcionan uno o más servicios a través de interfaces publicadas. Las preocupaciones suelen estar vinculadas a la tecnología de implementación elegida e incluyen el rendimiento, las restricciones de autorización, la disponibilidad y el coste. En algunos casos, estas propiedades se especifican en un acuerdo de nivel de servicio.
    
- Consumidores de servicios, que invocan los servicios directamente o a través de un intermediario.
    

Los proveedores de servicios también pueden ser consumidores de servicios.

- ESB, que es un elemento intermediario que puede enrutar y transformar mensajes entre proveedores y consumidores de servicios.
    
- Registro de servicios, que puede ser utilizado por los proveedores para registrar sus servicios y por los consumidores para descubrir servicios en tiempo de ejecución.
    
- Servidor de orquestación, que coordina las interacciones entre consumidores y proveedores de servicios basándose en lenguajes de procesos empresariales y flujos de trabajo.
    

Conectores:

- Conector SOAP, que utiliza el protocolo SOAP para la comunicación síncrona entre servicios web, normalmente a través de HTTP.
    
- Conector REST, que se basa en las operaciones básicas de solicitud/respuesta del protocolo HTTP.
    
- Conector de mensajería asíncrona, que utiliza un sistema de mensajería para ofrecer intercambios de mensajes asíncronos punto a punto o publicar suscribir.
    

Relaciones:

- Fijación de los distintos tipos de componentes disponibles a los respectivos conectores.
    

Restricciones:

- Los consumidores de servicios están conectados a los proveedores de servicios, pero pueden utilizarse componentes intermediarios (por ejemplo, ESB, registro, servidor de orquestación).
    

Desventajas:

- Los sistemas basados en SOA suelen ser complejos de construir. No se controla la evolución de los servicios independientes. Hay una sobrecarga de rendimiento asociada al middleware, y los servicios pueden ser cuellos de botella de rendimiento, y normalmente no ofrecen garantías de rendimiento.
    

  

### ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfx111oMvCq8cc8aERNlpTGroKs__eZseW9lvtb5hd7RUrpEsqGJfrWTMJynqrvJMBBlD8eAba_1LgiuQTjmxYHGVOC8g8z6wSbhsvnT2yk_sTVJizer5CbikI5Dbs10x1bCtt65lvA0wZ73zbvvj70L9M?key=VReuh94fGGpJZLGsXsGdUQ)

### Microservicios

Este estilo de arquitectura se utiliza para implementar arquitecturas lógicas cliente-servidor donde el servidor se implementa como un conjunto de microservicios que interactúan.

Los microservicios son servicios a pequeña escala que se pueden combinar para crear aplicaciones.

Los microservicios son:

- Autónomos: no tienen dependencias externas. Gestionan sus propios datos e implementan su propia interfaz de usuario.
    
- Ligero: comunícate mediante protocolos ligeros, de modo que los gastos generales de comunicación del servicio sean bajos.
    
- Independiente de la implementación: pueden implementarse utilizando diferentes lenguajes de programación y pueden utilizar diferentes tecnologías (por ejemplo, diferentes tipos de bases de datos) en su implementación,
    
- Desplegable de forma independiente: Cada uno se ejecuta en su propio proceso y se puede desplegar de forma independiente, utilizando sistemas automatizados.
    
- Orientado al negocio: debe implementar las capacidades y necesidades del negocio, en lugar de simplemente proporcionar un servicio técnico.
    

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd7xxppIy4jRP8WlfB-ysoGRA-0jE6hIgIMFtdGX2AxDkH282RyOEsgvLNVB3AO3ATQqxwvp_IAQ1251SMKYxemJ9SUBTRoF8aVpsUmxSML_Ehg8PbEwvLWS9CvBR2osxZAEDy3MH77r2aKExqB7cyLdAw?key=VReuh94fGGpJZLGsXsGdUQ)  
  
  

Aplicacion Monolitica vs Arquitectura de Microservicios

Ejemplo: Servicio de impresión de fotos![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfiZQ1HNXZZuILaajp0t_N4a4vqCFE4kVa-MypmQ6lCMLL1hmE-NZpSjCPGhfZ1KyzlCItcU6Oi5pKnBialuuY0tc6JU18CV4VM4lfT_VYAyrK2EoIB8Ivkh7m6kCsSuc02W6JOfMW-Z1VxSRxWUMD5mFo?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfR79iKIwXSfgNR1rJt7T8uYcyGeKw-6pu8jU7HfYZCOXO-WIZUj7-hGAfz-V_M-3ncMTas1aQ_hC7pnAiJAGKI2DUPdw0FAflYzV-W1xiAW_TV1todkHgaNqDJMdJhy0tFJ7ptDpmMnd5uXxOnXS8mnQ_7?key=VReuh94fGGpJZLGsXsGdUQ)