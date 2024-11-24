# PUDS (Proceso Unificado de Desarrollo de Software)

## Descripción del Problema

En la actualidad, los proyectos de desarrollo de software se están haciendo cada vez más grandes y complejos. Surge la pregunta: **¿Cómo organizar eficientemente este proceso de desarrollo?**

## Qué es PUDS

El **Proceso Unificado de Desarrollo de Software (PUDS)** es un **marco de trabajo genérico** que establece un conjunto de actividades clave para llevar a cabo el desarrollo de software. 

- Proporciona una **plantilla base** para el proceso, pero cada equipo debe **adaptarlo** a su propia realidad y necesidades específicas.
- Utiliza el lenguaje **UML (Unified Modeling Language)** para la representación de los componentes y sus interacciones.

## Objetivo de PUDS

El objetivo principal del PUDS es **transformar los requisitos del usuario** en un software funcional, a través de un proceso bien estructurado y organizado.

## Enfoque de PUDS

PUDS se basa en **componentes conectados por interfaces**. Estos componentes pueden ser módulos, subsistemas, o servicios que interactúan entre sí a través de interfaces definidas.

![Representación de PUDS](https://lh7-rt.googleusercontent.com/docsz/AD_4nXefTHJtYothXnDjcbZiaXHTlKQE4vSdpnm7siSkK1v8urYR5QPRq4S1dVpsV6WpGj5IJr5NA5kOkaa3k3Uvq9a1DNM73Vf_5VtrLfqCJrQ8ky8qZoHFMXD83CXPa3UUgqi9ebon7jkG0nofBTCEgN2JCZ7p?key=VReuh94fGGpJZLGsXsGdUQ)

## Características Clave de PUDS

1. **Plantilla base**: PUDS ofrece una estructura genérica que puede adaptarse a las necesidades específicas de cada proyecto y equipo.
2. **Uso de UML**: La representación gráfica y la modelización de los componentes y sus relaciones se realizan utilizando UML, lo que permite una comprensión visual y clara de la arquitectura del sistema.
3. **Enfoque modular**: PUDS está basado en la creación de componentes autónomos que se comunican entre sí a través de interfaces bien definidas.

---

## Conclusión

El **Proceso Unificado de Desarrollo de Software (PUDS)** ofrece un marco flexible y estructurado que ayuda a organizar y gestionar el desarrollo de proyectos grandes de software. Utilizando UML para la representación y la modularización de los componentes, PUDS facilita la creación de sistemas escalables y funcionales, adaptados a las necesidades del equipo y el proyecto.

  

### CENTRADO EN LA ARQUITECTURA

Arquitectura: Conjunto de decisiones significativas acerca de la organización de un sistema software, la selección de los elementos estructurales a partir de los cuales se compone el sistema, las interfaces entre ellos, su comportamiento, sus colaboraciones, y su composición.

Se describe mediante diferentes vistas.

Incluye los aspectos estáticos y dinámicos más significativos.

La arquitectura nos da una perspectiva del sistema completo, se basa en los elementos más importantes (arquitectónicamente).

La arquitectura software abarca decisiones importantes sobre:

- La organización del sistema software.
    
- Los elementos estructurales que compondrán el sistema y sus interfaces, junto con sus comportamientos, tal y como se especifican en las colaboraciones entre estos elementos.
    
- La composición de los elementos estructurales y del comportamiento en subsistemas progresivamente más grandes.
    
- EI estilo de Ia arquitectura que guía esta organización: los elementos y sus interfaces, sus colaboraciones y su composición.
    

Sin embargo, la arquitectura software está afectada no sólo por la estructura y el comportamiento, sino también por el uso, la funcionalidad, el rendimiento, la flexibilidad, la reutilización, la facilidad de comprensión, las restricciones y compromisos económicos y tecnológicos, y la estética.

Se necesita una arquitectura para:![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXct-3Hg9gfiK1qBYV1h-VyR0m_r0IqhlIplwfNzxoSQKxkdbmUgUft806EX7fx6KLmlF8Sru69hM6TLd9dFUUyLu7zJ_W936rzXksNvjV1bVLPFurhoq1djU3HglVwpK9Rz3baIxW_bOz_cKtrGaYEWMze7?key=VReuh94fGGpJZLGsXsGdUQ)

- Comprender el sistema.
    
- Organizar el desarrollo.
    
- Fomentar la reutilización.
    
- Hacer evolucionar el sistema.
    

Una buena arquitectura es algo que nos permite obtener los casos de uso correctos, de manera económica, hoy y en el futuro.

La arquitectura queda definida al establecer la línea base al final de la elaboración, desde ahí los cambios no deben ser tan significativos.

  

La descripción de Ia arquitectura debe mantenerse actualizada a lo largo de la vida del sistema para reflejar los cambios y las adiciones que son relevantes para la arquitectura. Estos cambios son normalmente secundarios y pueden incluir:

- La identificación de nuevas clases abstractas e interfaces.
    
- La adición de nueva funcionalidad a los subsistemas existentes.
    
- La actualización a nuevas versiones de los componentes reutilizables.
    
- La reordenación de la estructura de procesos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdZun_CTqu_F0ZQwNOk6zP_2Tc74e3zZiPYL_qFyVTkGYaxE65mwmc3TzcVALpLtow2EtfjQqVT-uZwEeniqnNgHHchdv-MfYj35HOu7bU1L6m7PlbgpDrP-X6YT_kL2Hy1drMDKtSco0eikAurwwcLJDQ?key=VReuh94fGGpJZLGsXsGdUQ)
    

Aunque está detallada en lo necesario, la descripción de la arquitectura es aún una vista de alto nivel. No se pretende que cubra todo. Debe representar lo que cada participante necesita.

Descripción de la Arq = Vista de todos los modelos del sistema en ese momento determinado.

  
  
  
  
  

### DESARROLLO ITERATIVO INCREMENTAL![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcFWcYWifX1YMYNaqZqgLw1INDBU15OR5MwYQa35Vn5NMLBNpTG9sh3D4OVx-SkfYMkn6UaZ4dgJJoY8wdOY4JYeyh2a36mGCTYrqUIGS1t9KiykpxKyguFHJbG8c1a3vXR1532FdWG9Ujsw2zr_VZ_n_7v?key=VReuh94fGGpJZLGsXsGdUQ)

Es práctico dividir el esfuerzo de desarrollo de un proyecto de software en partes más pequeñas o mini proyectos.

Cada mini proyecto es una iteración que resulta en un incremento, “artefactos del modelo”. Al finalizar una iteración el conjunto de modelos que representa al sistema queda en un estado concreto, llamado línea base. El nuevo incremento se integrará con el resultado de la anterior iteración, obteniendo una nueva versión del conjunto de modelos.

Las iteraciones hacen referencia a pasos en el flujo de trabajo fundamental, y los incrementos a crecimientos en el producto.

Las iteraciones deben estar controladas. Esto significa que deben seleccionarse y ejecutarse de una forma planificada.

Los desarrolladores basan la selección de lo que implementarán en cada iteración en dos cosas:

- El conjunto de casos de uso que amplían la funcionalidad.
    
- En los riesgos más importantes que deben mitigarse.
    

En cada iteración los desarrolladores identifican y especifican los casos de uso relevantes, crean un diseño utilizando la arquitectura seleccionada como guía, para implementar dichos casos de uso. Si la iteración cumple sus objetivos, se continúa con la siguiente. Sino deben revisarse las decisiones previas y probar un nuevo enfoque (prueba de regresión). En un caso extremo, si la iteración fue mala, puede llegar a la cancelación del proyecto.

Prueba de Regresión: Es especialmente importante en un ciclo de vida iterativo e incremental, debido a que cada iteración produce una adición significativa al incremento previo, al mismo tiempo que una cantidad importante de cambios. Es un control de versiones.

  
  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXekOSbTFujyQStoAgel4B7_Mxa-cA2ekGnyupuRwvKMT2YtZRYXYNHugm2ZIUKzoMTuTkjqm19lXCLiX86OaalQC5Hrpj6u6gLGOiWWGwcPlhvloYxl78bQZNHM-cw_KisRIqRtafZd-AuwMbFVHUWQ4dVN?key=VReuh94fGGpJZLGsXsGdUQ)

Que se pretende en cada fase  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXczTLKeuxgpnjXsV61QOkBm-5Fky2dEpesMGYqzcnODFkI8P1hHWXlgDfK-MOfaAWbFmHikavoszN9sdSxgldH3mqPILHDnCr7YhByDclQoOzIwV2hn_gjCFAIbBmRTa8u-ulL8d59OeqxrpMLA05L1zrIa?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdHGKx6BcyMvoKZ6LMwduUdAedKQ1OwOA8XsB4YVkVzFMfBklYofdI361kWDydHYnCGNa5g4NcuxFw8EGioQSf_MjTIvs28YMf7oVVgJC97Y2owNE6mGErHt-3vj2iTbrWqzztCgpwOCziKbD0FeF8WLMw?key=VReuh94fGGpJZLGsXsGdUQ)

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfDxRb7H7coC6KCDcMMqEoKkoItvDm9R5Rvtz6emQBdppRMp9f0fqy9HwAibJpFKU7KIb-8yGnYRnMlusEYyrFcl3LMKeXgKg7TJbZi1E5TEHAhM0w5gqDuvg4CRc8mgjgjjOl-uL1S5vcyPxRAhy49ziU?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd8RhAcsYDBrHGTvyz5L1XDeyUcnaNPslj1Myf2PdnC1-HxTwpE8frdb_LBt17xc6v7-Z2yBVKaSQuKSkkmM3YD9I8vHlkqqAf1KoYTk8RB_6ZFbisb8WyyxHUHmPc1-g7FGubV6k0zy8KZ2oyrFRVZtJv6?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf9T94AysFY4IQwGhysJTuBw4CU0UkCBiuHORmRA8YVk59UEiUQvg9bW1mquwUjdM3n1reCt6HgwIRuR5uWVrwmuCGcjrzwOV8FlWHJ4mzLyYKwZwnX11Kf7u5C50yQ6_my_zIkbwqEQthsuN4cecy9oYE?key=VReuh94fGGpJZLGsXsGdUQ)

Comparación con Modelo en Cascada

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdnR_jIAx8OwehmwnY-zbjeKzkfd86c36iQtzqaePnI_lkJ90WXHrQODC7P03n2gS4sxuS_OiFKPHU-PbSh_Rm98S31Cl2M4fcEUZmH7ToqCKSn25HrEoXziC59B9HYVuweBmfZqoRWPhqHtSo5VWfPllqE?key=VReuh94fGGpJZLGsXsGdUQ)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfSQk5FkG0R9a9g8Kx5GQt1WYyHpCgqxIKUe7_UGJRlka1oFd_42nNLUy7mgPEDdeOn7ezVn4wUbo9NEFPWqm31QADRnd7oPxJTOFdZFu_MgsHc7aXRg6m1_w_SS998ds2sqtYWI3GTeRklsaYbcnr1yk_N?key=VReuh94fGGpJZLGsXsGdUQ)  

Beneficios del enfoque iterativo

- La iteración controlada reduce el riesgo a los costes de un solo incremento.

- Reduce el riesgo de retrasos en el calendario atacando los riesgos más importantes primero.

- Acelera el desarrollo. Los trabajadores trabajan de manera más eficiente al obtener resultados a corto plazo.

- Tiene un enfoque más realista al reconocer que los requisitos no pueden definirse completamente al principio.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeKqqxB_C2Jd6dgcQCYFJd-XlmtkGJ8uj84V9eZVcRdJ2C_jD_4zsrOGHEdww7cbbSsf0Q_PsjZG0VFq01TR7L0roq6Kf3F7qRHo0c3k-odaIfd27c1lpl-V_iZzsPvLFrDj06lc9SIPq1OUIMfrvkGJadu?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  
  
  
  
  
  
  

## CICLO DE VIDA

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfFZ4RFTvDQT8ug8ZWPTh7TtrGzCHPttu7dBc6-dTy5XOUwJwIOkWMePhO9W1s39tO3x5RoYlUUCQQuBE7x952M1U-jrSPTNu1KSvBmkWHsYlMu6ASA9KCWN50w-kS2QK5_8RUKu2bTRf7JohuBi9x0eZ8?key=VReuh94fGGpJZLGsXsGdUQ)

Cada ciclo tiene una version del sistema

Cada ciclo esta compuesto por 4 fases

Cada fase se realiza mediante iteraciones

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfUXI9D75hgvSSEhmtvLEwl2t1oOLNUmm5bmIvs-KYRGow5wn1wUcK1tlcuG5SrywgHxdozxvIp7IlViX59egruyTqViw2t2EDQ6Up-tiGPJ_dVmQB3MtTlOcV702bGsAVNo-87xOpuV_BUoZ71tm-u58Q?key=VReuh94fGGpJZLGsXsGdUQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdQ0dm0EB8Kvsd-cKoSzWjkoeTkhqcJEigEz0lzBxM_TrWwtQDkv1Bg-pwOh-oWcvTKjIG_3RIvaFRDIYMLMgzUtMwNP63enzVFt_OnDcd-kDvylEFb6U7-pfsY_QqZEsZRtA_XoOvAjwzbzZ3Pf2YOGII?key=VReuh94fGGpJZLGsXsGdUQ)

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcLnAeuYmuwCILFqe_Houi_4GQkl_AHHKqZwrt3b5xTrRSw7Ku7Uyu1igY3wzZXClSl-rmhTdlEzSXTdmYRubMmpuhLeYBRfnwwuJUK9hri6maKgf7nKyDth2OBM62FOtjS2j_aOMOwZfaLBXeGEWcr_CYQ?key=VReuh94fGGpJZLGsXsGdUQ)

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf-l_gRpTEeSaJZLEZ7k38LLpKmfy2P1sBqaneqMY9-c2WGsE5P51lYUrhmct4xC0hch3VVdm9m1E9el0NdGKG3Akcxkylr6KX3IhLW6kbgBHxNgUV-sdWh6si8DSK95OXPFl8pQ_d43Ys9tjt7p58k5KNW?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  
  
  
  

## CONCEPTOS CLAVES (LAS 4 P DE PUDS)

Flujo de Trabajo Fundamental![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdImgOOTqppvIvAF3bvQDoeLekqTYqEDX3XhNFnH-wR3iPyrCg_xlva7K6CuyqHcjzILGESPBJAYrAAp_cbYLhGmtvsf9MqK9lRFSmxCi-U7PFdzL0FO5MDauhF9BKmafqo_dw383lnPfR88b5FgEiHO8yJ?key=VReuh94fGGpJZLGsXsGdUQ)

Actividad![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeOR8ROMURq6k4e4GiY4ylQ6oE_yI_nXXXeqET0JciSfMw3l522J1yx7Kw_0N6QTjgcV0rgus0HO7asguwbqVvY1qJRGfs08OSpJAFF0f7p-Y76eaIewyaCsghIdIM554PmMVC6o7tHd4ynmcGqqoZilLxo?key=VReuh94fGGpJZLGsXsGdUQ)

Trabajador![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfP7oSVES4QAmKws2-8dC6OI_zqCSultJ7NAv6fjej3H3cNWyui9PPXsyXpjv0NwtCn2c0KKOH3zQE4k3PX5gTLVNwoUwZQBqgloF5K7x_ZgqQGSQnnvLWq5F-3vhbJ3X7F00M14jGMqtC06QGIwkn3i-Jj?key=VReuh94fGGpJZLGsXsGdUQ)

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXekMc7R5a0OyTikg8Exd15_b5h-Gnh85MaxCgOcExanMxz-j6MC4ehCIZiv8ZJfubUDC3bOnb20Tgbag96AFl-scpHwebwtFslGyzKyygO41Afy4G2Fh7wD2fK0JnedwrEtpa9nJNjl62jg5QrYC-q-neM?key=VReuh94fGGpJZLGsXsGdUQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXefuILLqPHSxRTRDr0Ja2b6fik9ae1RBod8iR44qvb3suiuMDH-88EMeoD2XhKrWuRYnJVP9uQD01ZH_YduogDAU7GpT-KrCn2-TE5Vmuk9ew5KgspMYFdute2yQhWpUhOtCorzpMHoWJy_7NZDAZapIu0?key=VReuh94fGGpJZLGsXsGdUQ)

Artefacto

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfti-vQn-SrNlBqXFuR_SMK-mIFwtUhaHsJeMPfdMpmfNaYrrJvi07ftmX6-QN0Kl-ygXUFWJRG8uecPDHdC5p5hFD6Vx4ykwZVfhY-dfvvQx4hHleDXj20rAffyBaahufTyQYjy7EfkILN34FCDl98U2s?key=VReuh94fGGpJZLGsXsGdUQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXd7pAfHDO3RzUPK6o38v6WqBwXT9UQ1X5p95dnDURCrGSU4yzRJUB0TCgDoA9pPvVOglkQFs902llQG4kEJcXU62V5A7Zh5yw5gvVx71zreAl3E5nvA3jUS2lyPP2Kw_oTRK72Nr4-ikWaWRwhuYQ0Ch5bz?key=VReuh94fGGpJZLGsXsGdUQ)  
  

Notación alternativa para flujo de trabajo (seguro pregunta el ggs):

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdY7GHulx8DRBDCCbplQ2_sTJfJzZUrFL3JCzYCQYmm5Jsyry3DSqvqxNQbMNY8AskfOlr0YypGFy2l82N3d-6jeu3jPaHYLKJn_JyTUm6VxKJQ20e_iycU8smTKYqXCEIK_n_RZHFRSxaQ9oCv9vwYvXyy?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  

DIFERENCIAS CON RUP

- Workflows distintos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfAzvKL24y1k8zZnF-305THCYAfCZYeYX4-bm366pP7M42p9x0EZw9XyZqc64dBeJxKR_QFn2nZSowzg47O0QAx2xZnFL8mNC3wIW-CeWm4rNYdM-T2bwnNoJPBytgSs0bcgFKyHySPv0N01MD3fRC6rgk?key=VReuh94fGGpJZLGsXsGdUQ)
    
- En general, son lo mismo. RUP es la especialización, PUDS es generalización.
    

# FASES

Razón para que sea iterativo e incremental: manejar el tiempo, periodos cortos y manejables. Dividir el problema en periodos de tiempo para planificar mejor y mitigar los riesgos.

Fases -> primera división de tiempo que nos encontramos. Fases = periodos de tiempo.

Básico: Inicio.

Último: Transición = instalar el producto.

Nos centramos en lo que buscamos encontrar en cada fase.

  

  

  

  

  

## FASE DE INICIO

Principales Objetivos:

- Describir el producto a desarrollar - Objetivos del proyecto: Se arranca pensando que es lo que hay que hacer, objetivos a alcanzar.
    
- Análisis de negocio:  
    ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcPocQvMecCbl5x3Z0ccJX0aeEhTjiL3UeDrk1S_RyxHUKGHSmdI4a97S5epRvCK0642ApEvweJsjKu0WTJ0JIl1dcsnYgM89CnaUUS8oDtexD58iqol7KXlwBOxu40rX3MwDbe8D62Sh2_iIhQRYLnqic?key=VReuh94fGGpJZLGsXsGdUQ)
    
- Identificar riesgos más importantes: CRÍTICOS, los que ponen en peligro el proyecto entero, pueden existir riesgos que no sean del todo mitigados, pero existe un plan de contingencia.
    
- Explorar soluciones y arquitecturas posibles: CANDIDATOS posibles, se responden preguntas como: ¿Puede utilizar de forma apropiada la tecnología (bd, redes, etc.) sobre la que va a ser construida? ¿Puede ser eficiente? ¿Puede explorar los recursos existentes? ¿Puede ser fiable y tolerante a fallos? ¿Será robusta y flexible al cambio? ¿Evolucionará si se añaden requisitos?
    

Estudiar la factibilidad del proyecto. Entender las grandes funciones del sistema. Cuales son las soluciones a tener en cuenta. Bocetos preliminares, ideas, arq posibles. La idea es saber si el proyecto conviene o no desarrollarlo.

Principales Artefactos:

Artefactos: Es un término general para cualquier tipo de información creada, producida, cambiada o utilizada por los trabajadores en el desarrollo del sistema. Información que se va produciendo y modificando a lo largo del proceso. Se fabrica a medida que va avanzando el proceso de desarrollo.

- Lista de características o features: Oraciones que definen funcionalidades que me dicen que es lo que se espera del futuro sistema. Son funcionalidades de alto nivel ya que se pueden subdividir en varias funcionalidades. Ej: inscripción de alumnos. Gestión de pagos.
    
- Primera versión del Modelo de Negocio. Contexto del sistema, BENEFICIOS VARIOS ETC
    
- Principales Requerimientos como Casos de Uso. (Lista detallada).
    
- Lista de riesgos, bocetos de modelos de cada flujo
    
- Boceto de la arquitectura.
    
- Descripción de los objetivos del proyecto.
    
- Plan preliminar del proyecto: Como es la fase de inicio, la mayoría de cosas son bocetos, eso incluye la lista de características. Todo es un boceto, y puede alterarse.
    

La fase finaliza con:

- Hito “Objetivo del Ciclo de Vida”: Decisión de continuar.
    

Lo que divide a las fases son los hitos. Esta fase finaliza con un hito llamado “objetivo del ciclo de vida”.

Hito: Es un punto de control. Se debe preguntar si estamos listos y si es factible continuar con el proyecto, caso contrario se cancela el mismo.

Esta fase es crítica y dura días o semanas. Ya que se decide si se va a continuar o no. La decisión es tomada por el equipo de desarrollo y por las personas que ponen la moneda en el proyecto.

La mayoría de las actividades de esta fase ocurren en los primeros flujos de trabajo (requisitos, análisis y diseño), y no tanto en los últimos dos.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc50UCKnVITtruvWiG7wFaJf2vO9OHMYegVdJ9LCizCKwcoXh_27MKLnPVSjqWlG8Txmsp8Ie7Gl9R7sct_dLlNNsCjiZvRvzp1l2giIsYGZny4dLJoC4xM5iN4-pMevl353tnjay0sB8clvOiZrTYemAw?key=VReuh94fGGpJZLGsXsGdUQ)

##   

##   

##   

  
  

## FASE DE ELABORACION

Principales Objetivos:

- Establecer una firme comprensión del problema: Se espera una arquitectura que sea ejecutable, es algo que se pueda ejecutar para mostrar al cliente. No se espera que sea algo usable, pero sí para demostrar la funcionalidad.
    
- Establecer una base de la arquitectura.
    
- Plan detallado de iteraciones.
    
- Eliminar mayores riesgos. Para el análisis del negocio, se han eliminado los peores riesgos, en caso contrario, hay un plan de contingencia.
    

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXc-wOxgmC_H_O7oIHP_zl3ai3uvey5LcIIoIrB0XK-iun0cXrBD1W4GCxWYvHYw1OOc7sESfB4XQjHvHjUSgG3rM9JkjFPgstSTPuaFopS1ETZjdwJd5t7215wz7S6GdxKvuYIbRHuBDlkWwGQPMPeBz-8?key=VReuh94fGGpJZLGsXsGdUQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfbtb4tydt4QvPol_H-LNM0E0eedZDp6fseJaqi1-LjlKi8cta92eTvTu8wnD-gacKEc7rVHO6nnw8OPr1ZRBHFBpxENUicV2jx1CvoS8hMJ4FvZlfj2jd5pPnnRiPSjokVtAAiRUeiA0nOWzpvxm9h4r0?key=VReuh94fGGpJZLGsXsGdUQ)

El arquitecto establece la prioridad de los casos de uso y realiza actividades de análisis, diseño e implementación (a nivel de la arquitectura). Otros trabajadores llevan a cabo actividades de diseño, como análisis de clases y paquetes, diseño de clases y subsistemas. Los ingenieros de pruebas se centran en construir el entorno de pruebas y en probar los componentes y la línea base completa que implementa los casos de uso significativos desde un punto de vista de la arquitectura.

Principales Artefactos:

- Línea base de la arquitectura ejecutable.
    
- Modelo de negocio completo en lo posible, contexto del sistema.
    
- Modelos de casos de uso y análisis (hasta 80%), diseño 10%. Esto último se necesita para definir la arquitectura, que es el objetivo principal.
    
- Plan de proyecto para las fases de construcción y transición.
    
- Lista de riesgos actualizada (con respecto a la fase anterior).
    
- Análisis de negocio completo
    

La fase finaliza con:

- Hito “Arquitectura del Ciclo de Vida”: Definición de la arquitectura.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdv4ZHTfFGjH9GyPzBHWhy-0Uw9YWBxYNuX1cE58oQHYwkuKB4DL_T24Q1nIDEEs8cDS-k2keboIf6ObY3HeeTEDe0oWKEtbRMo-cV9gXntMJR2QQmhh67BEUCwtGnclRkpiP2fnPVmKMA1ZHW9njY2M7ug?key=VReuh94fGGpJZLGsXsGdUQ)
    

ANÁLISIS DE NEGOCIO

La razón subyacente para mitigar los riesgos y desarrollar la línea base de la arquitectura es el llevar el proyecto hasta un punto del desarrollo en el cual el equipo pueda empezar la fase de construcción con plena confianza de que puede construir el producto dentro de los límites del negocio. Fundamentalmente, existen dos límites del negocio. Uno es la planificación, esfuerzo y coste estimados para una calidad dada. El otro es la recuperación de la inversión (o alguna métrica comparable) indicando que el sistema propuesto será económicamente un éxito.

Al final de la fase de inicio, la organización software podía juzgar las virtudes del análisis de negocio con unos márgenes de error muy amplios al menos, en el caso de proyectos grandes, difíciles o novedosos. Al final de la fase de elaboración, se ha avanzado en el conocimiento del proyecto hasta el punto de haber estrechado notablemente estos márgenes. De esta forma, se puede preparar una apuesta económica y desarrollar el análisis de negocio dentro de los márgenes mucho más estrechos de la práctica empresarial.

  

## FASE DE CONSTRUCCIÓN 

A medida que el proyecto pasa de la fase de elaboración a la de construcción, se produce un cambio de enfoque. Mientras que la fase de inicio y elaboración son consideradas como investigación, donde se acumula el conocimiento básico para la construcción del proyecto, la fase de construcción es análoga al desarrollo, es decir, se construye un sistema o producto dentro de unos parámetros de coste, esfuerzo y agenda. 

Esta fase va más allá de la arquitectura, se desarrolla todo lo demás. La arquitectura se deja como está, y solo se actualiza.

Las fases anteriores han investigado y mitigado los riesgos críticos y significativos, pero habrá aún muchos riesgos en la lista de riesgos. Además, pueden aparecer nuevos riesgos a medida que los desarrollas realicen construcciones e iteraciones y que los usuarios prueben nuevos incrementos.

PRINCIPALES OBJETIVOS

- Desarrollar el Producto (Versión BETA).
    
- Desarrollo de todos los casos de uso.
    

ASIGNACIÓN DE TRABAJO

La línea base de la arquitectura con su representación de subsistemas e interfaces es la base de la que parte el jefe de proyecto para dividir el trabajo. Cada subsistema se convierte en responsabilidad de un desarrollador, que actuará como ingeniero de componentes. Normalmente, como dijimos en el Capítulo 9, el desarrollador responsable de un subsistema es también responsable de las clases de dicho subsistema.

PRINCIPALES ARTEFACTOS

- Software ejecutable (capacidad operativa inicial)
    
- Casos de Prueba
    
- Manuales del usuario (suficiente para la BETA)
    
- Plan de la fase de transición. 
    
- Modelos “completos” (Pueden agregarse cosas en la fase posterior)
    
- Descripción ARQ.
    
- Análisis de negocio actual.
    

FINALIZA CON

- Hito Capacidad Operativa Inicial → Versión Beta, se consigue luego de evaluar los resultados de las pruebas del sistema al final de la última iteración
    

  

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdeyhK4jjesqfaLRvR5NAvf1tsccZ_w2vsJrlY2S0jDoxGxMdDuBjlJyZyaDQDVp2GXpnpHj-YYmuuzVsYnNrhclvaIH_buPCPnOw1oAgmmBpoVY9Eme-53RgFdSN-3LUlqJDUL7QcvemWirpPwnK2pou8?key=VReuh94fGGpJZLGsXsGdUQ)

ANÁLISIS DE NEGOCIO

Uno de sus propósitos es el de servir de guía al jefe de proyecto y los inversores para ejecutar la fase de construcción. El jefe de proyecto comparará el progreso real al final de cada iteración con la agenda, esfuerzo y costes planificados. Revisará los datos de productividad del proyecto, cantidad de código desarrollado, tamaño de la base de datos y otras métricas.

  

  

  

  

##   

  
  
  
  
  

## FASE DE TRANSICION

Se extiende lo que actualmente se tiene. Hay que entregar el producto final. 

PRINCIPALES OBJETIVOS

- Puesta en producción de la versión beta.
    
- Se continúan agregando casos de uso. NO FUNDAMENTALES
    
- Correcciones / adecuaciones / extensiones.
    
- Cumplir requisitos hasta la satisfacción de los usuarios. Corrección de los defectos remitidos por los usuarios en la versión beta.
    

¿Qué se hace en esta fase?

El proyecto lleva a cabo las actividades de transición según las siguientes líneas:

- Preparar la versión beta (o de pruebas de aceptación) a partir de la versión con capacidad operativa inicial producida durante la fase de transición.
    
- Instalar (o preparar la instalación de) esta versión en los lugares elegidos, junto con las actividades relacionadas en dichos lugares, tales como la migración de datos desde el sistema anterior.
    
- Actuar a partir de la información recogida en las instalaciones de pruebas.
    
- Adaptar el producto corregido a las circunstancias de los usuarios.
    
- Completar los artefactos del proyecto.
    
- Determinar cuándo se acaba el proyecto. La fase de transición no acaba cuando se completan todas las tareas y artefactos, sino cuando el cliente queda "satisfecho". La fase de transición terminará cuando el proyecto transfiera la responsabilidad del mantenimiento continuado a una organización de apoyo.
    

PRINCIPALES ARTEFACTOS

- Lo mismo que en la fase de construcción, salvo que son la versión final.
    
- El software ejecutable.
    
- Documentos legales, como contratos, licencias, renuncias de derechos y garantías.
    
- La versión completa y corregida de línea base de la versión del producto, incluyendo todos los modelos del sistema.
    
- La descripción completa y actualizada de la arquitectura.
    
- Manuales y material de formación del usuario final. del operador y del administrador del sistema.
    
- Referencias (incluyendo referencias de la Web) para la ayuda del cliente, acerca de dónde encontrar más información, cómo informar de defectos o dónde encontrar información sobre defectos y actualizaciones.
    

FINALIZA CON

- Hito “Lanzamiento del Producto”: Acuerdo con el cliente.
    

  

ANÁLISIS DEL NEGOCIO

El final de esta fase coincide con el final del proyecto en términos presupuestarios. El jefe de proyecto convocará un grupo para revisar el tiempo, personas-hora, coste, porcentajes de defectos y otras métricas que la empresa pueda utilizar para:

- Ver si el proyecto ha alcanzado los objetivos planeados.
    
- O determinar las razones por las que no lo ha hecho.
    
- Añadir las métricas del proyecto a la base de datos de métricas de la empresa para su uso futuro.
    

El proyecto recibirá información de los usuarios para:

- Determinar si el sistema hace lo que demandan sus usuarios y el negocio.
    
- Descubrir riesgos inesperados.
    
- Anotar problemas no resueltos.
    
- Encontrar fallos.
    
- Eliminar ambigüedades y lagunas en la documentación de usuario.
    
- Centrarse en áreas en las que los usuarios muestren deficiencias y necesiten información o formación.
    

  

FLUJOS DE TRABAJO

En esta fase la actividad es baja en los cinco flujos de trabajo. Como casi todo el trabajo se realizó en la fase de construcción, el nivel de actividad en esta fase es bajo, justo lo necesario para corregir los problemas encontrados durante las pruebas en el entorno del usuario o para efectuar mejoras de última hora (por lo general, menores).