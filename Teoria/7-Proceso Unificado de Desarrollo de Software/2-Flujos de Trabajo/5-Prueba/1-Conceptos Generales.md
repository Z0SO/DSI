## PRUEBAS

### Propósitos de la Prueba

Los objetivos de las pruebas son:

- Planificación de pruebas: Determinar las pruebas necesarias en cada iteración, incluyendo pruebas de integración en cada construcción y pruebas de sistema al final(al final de la iteración).
    
- Diseño e implementación de pruebas: Crear casos y procedimientos de prueba, y desarrollar componentes de prueba automatizables cuando sea posible.
    
- Ejecución y gestión de resultados: Realizar pruebas, registrar resultados y volver a probar las construcciones con defectos, remitiéndolas a diseño o implementación si requieren corrección(enfoque iterativo incremental).![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXemWsOVaLg2NOGB6KYMdyMWlSRw3G5MoouHeN0yH7IghRURb6alrBzhw0bXFM-0LnR-G3jqUjkJuenGmnY1X00i8mXN2G2tSXYNmVYoi5fXcYhHUMW4YnNc5gwFTVywc3m_HF_Ms-aWLaGdrCLsWkIJut6o?key=VReuh94fGGpJZLGsXsGdUQ)
    

Durante la fase de inicio se pueden planificar las pruebas, aunque el grueso se lleva a cabo cuando se prueba la línea base de arquitectura, y luego las construcciones e integraciones realizadas en la fase de construcción. En la transición más que nada se depuran defectos, y se hacen pruebas de regresión.

Es natural que se mantenga el modelo de pruebas a lo largo de todo el ciclo, pero este cambia debido a:

- Eliminación de casos de prueba
    
- Refinamiento de casos de prueba
    
- Creación de nuevos casos de prueba
    

  

### TRABAJADORES Y ARTEFACTOS![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfsCV87QXuPnGz9M0if5E1ulYHHWPy0M8DDuGTRNIVQ7JcQ81Qy8C9lTQ2lRArBJsrNyfZvV0wWz3urmodgsGSkx7ov3ESXEkv7NL6RYh-SUhX67vONYESBhBHBNkqJuq0YPIaklA?key=VReuh94fGGpJZLGsXsGdUQ)

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfAD0cBz13THQOSQGPO56I9fzTNhJLyg6Dd_Mm1mSOz-G3pMALvBLpMd8xxfxIYigtqOAhXyZJMdeP7T4QfLfLB47ZMCnSfHwruE6pnIE4DVyaI2j_Os1rQlWCBFCZcXHVb9to5z0Y8egRMbsyMl5i5BzY?key=VReuh94fGGpJZLGsXsGdUQ)

  
  
  
  
  

### ARTEFACTOS

- Artefacto: Modelo de Pruebas
    

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfz0N3fVyesgOlSnzZnRwI3zvvwdKg4wwsoQ-XiuxY66Tt4zV4MIEJUE70FZeP9rtEz2l0T-TclAUjTa5A3wVM2u5YL7mVqE6OuGbAkx-A_3qaWq53czYVXgAT4-HMZYZn4Q4LaV82BOYKxPgna7xfvF5Mv?key=VReuh94fGGpJZLGsXsGdUQ)

Define cómo se prueban los componentes en el modelo de implementación mediante pruebas de integración y de sistema. Incluye casos, procedimientos, y componentes de prueba. En sistemas complejos, puede organizarse en paquetes para facilitar su gestión.

  

- Artefacto: Caso de Prueba![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeR3abOS3aaWwUiCxhUCNyUh-CB2UZE3TelP1-2iXlpGcYaX00k2uFWcAf0r6jD5OwXjaqwUDRZFmbWjAoEqED4LKV4sVWHnXKN8NkaTbd6zW6jG1GokP556tye4oyqReSReemaKZrR7Uk0rnMdkNCJ6FE9?key=VReuh94fGGpJZLGsXsGdUQ)
    

Define cómo evaluar un aspecto del sistema, basado en un requisito o conjunto de requisitos. Se definen entradas, resultado esperado, condiciones. Usualmente dos escenarios:

- Caja Negra: Caso de uso o un escenario específico de un CU. (Comportamiento observable externamente).
    
- Caja Blanca: De una realización de caso de uso del DISEÑO, o un escenario específico. (Se prueba de forma interna).
    

También se incluyen pruebas especiales, como pruebas de instalación (PC del cliente), configuración (redes), pruebas negativas (para verificar fallos), y pruebas de estrés (para evaluar el rendimiento bajo carga).

  

- Artefacto: Procedimiento de Prueba![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeW-bV90vEXyoFkhUWJxbuW2TEbjW7obdEusWYQI7lxC04P-rt_umARM1RZn_7vJtLSE4PUP2sZ7gKhI0N6cveRqD9z-2EyqZc0O5wqYGpeL2qLnWPKBrYwZ5PEAg2XXQAmWr11O8UTN78LUvyuWOEf-KnF?key=VReuh94fGGpJZLGsXsGdUQ)
    

Describe cómo ejecutar uno o varios casos de prueba. Puede ser manual o automatizado, y es reutilizable entre casos similares. Literalmente secuencia de pasos, puede coincidir con la descripción del caso de uso, pero se incluyen entradas y salidas esperadas

  

- Artefacto: Componente de Prueba
    

Automatiza procedimientos de prueba, proporcionando entradas y monitoreando la ejecución. Pueden implementarse en lenguajes de guiones o programación y son conocidos como “drivers” o “test harnesses”.![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIJKEk6NOxouPUq-QMUytsaFJLEoCx-tMjn77_6grwQ3M4prIgPKVrHRTIVoJKXzHL426coDJNlGh0htxNt4rSuiGewb8HDVP3_SpNGhuUAmw8KP0huwWHBxs3rVZnZV7AWRYtghy-xZZZFjPERbmi0W4?key=VReuh94fGGpJZLGsXsGdUQ)

  

- Artefacto: Plan de Prueba
    

Establece estrategias, recursos y planificación de las pruebas, definiendo los tipos de pruebas, objetivos, cobertura esperada y resultados deseados.

  
  

- Artefacto: Defecto
    

Es una anomalía en el sistema que debe registrarse y corregirse, como un fallo de software o un problema encontrado en una revisión. ERROR

  

- Artefacto: Evaluación de Prueba
    

Analiza la efectividad del proceso de pruebas, revisando la cobertura y el estado de los defectos detectados.

  

### TRABAJADORES

- Trabajador: Diseñador de Pruebas![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfCezEUqKliiUFrPBOlst8i65jFRdncQTbaxPo1eGQmxYwFDHo7UoRyL1YNB55ZGXb5IWRPKLOhFZi1mvpP7INXSiddXS5SBwTSLDPl48Tj3epfSRsmpglBqrGIUA1BDxR4Z68Pv8yWb8bKcREO87crT9bZ?key=VReuh94fGGpJZLGsXsGdUQ)
    

Responsabilidad: Garantiza la integridad del modelo de pruebas. SOLO PLANIFICA Y EVALÚA.

Funciones:

- Planifica objetivos y procedimientos de prueba.
    
- Selecciona y describe casos de prueba.
    
- Evalúa pruebas de integración y sistema.
    

  

- Trabajador: Ingeniero de Componentes
    

Responsabilidad: Crea componentes de prueba que automatizan procedimientos.

Habilidades: Requiere habilidades avanzadas en programación.

  

- Trabajador: Ingeniero de Pruebas de Integración
    

Responsabilidad: Realiza pruebas de integración para verificar el funcionamiento de componentes. De cada construcción de la implementación

Funciones:

- Documenta los defectos en las pruebas.
    
- Se basa en casos de prueba derivados de los casos de uso-diseño.
    

  

- Trabajador: Ingeniero de Pruebas de Sistema
    

Responsabilidad: Realiza pruebas de sistema sobre el resultado ejecutable de una iteración.

Funciones:

- Verifica interacciones entre actores y el sistema.
    
- Documenta los defectos encontrados.
    
- Usualmente se requiere conocimiento de estructura interna, se puede hacer en conjunto con los especificadores de CU, etc.
    

  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

### Flujo de Trabajo

El objetivo principal de la prueba es realizar y evaluar las pruebas según el modelo de pruebas. El flujo de trabajo se desarrolla de la siguiente manera:

- Planificación de Pruebas: Los ingenieros de pruebas planifican el esfuerzo de prueba en cada iteración.
    
- Descripción de Casos de Prueba: Se describen los casos de prueba necesarios y los procedimientos correspondientes.
    
- Creación de Componentes de Prueba: Los ingenieros de componentes desarrollan componentes de prueba para automatizar algunos procedimientos, cuando es posible.
    
- Ejecución en Construcciones: Este proceso se repite para cada construcción entregada en el flujo de trabajo de implementación.
    

Este flujo garantiza que las pruebas se realicen de manera estructurada y eficiente en cada iteración del desarrollo.

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdlFisDXbxJ1eTgF7zeNbfIbwn2-KWB2PetAZhP1SscT2EhO5NcFuNty-W7XypunWJuBoIJCxyISpl9B19HzchPzXO54kyvcRoltAMRYB1nSWG1YkHZxOh0MXzfyW1ELThrXW4JnqI7AEKSsG9L4xnKe-M?key=VReuh94fGGpJZLGsXsGdUQ)  
  

#### Actividad: Planificar Prueba![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcSYPJws297dHmPHt1RG0vP6dJ8Yr7cgpNVBx3QeSZXqqWsBKgpd2BynsGpk43u-xfg6FWKFSSikKRevHnk7Uqd_zSB56QnSM2Bkb67XFpNbRMp6NhuznJ755gulfIafHeuU0rDQW1hS7mmL331GIyprfXN?key=VReuh94fGGpJZLGsXsGdUQ)

Propósito: Planificar los esfuerzos de prueba en una iteración mediante:

- Descripción de una estrategia de prueba.
    
- Estimación de recursos necesarios.
    
- Planificación del esfuerzo de prueba.
    

Los ingenieros de prueba utilizan modelos de casos de uso y otros artefactos para definir el tipo de pruebas y estimar el esfuerzo requerido, priorizando casos y procedimientos con mayor retorno de inversión en calidad y que tengan mayores riesgos asociados. Solo Pruebas de cosas importantes

  
  
  
  
  
  
  
  

#### Actividad: Diseñar Prueba![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXduJ-yiWL-3IbiVkNff_J1_frGzn_vnrnj546wV3ZWTN1hjP6MK8g1IZ3yvTnWzM1Mh18frG53UMSGfuYM7_tliZdB1cEq36axx9MxLnGsQf6tLNS-rp_FI04TWcgRBsu324SMvgRFNYNbmHKr6-e-X3cNZ?key=VReuh94fGGpJZLGsXsGdUQ)

Propósitos:

- Identificar y describir casos de prueba para cada construcción.
    
- Estructurar procedimientos de prueba.
    

Diseño de Casos de Prueba de Integración: Los casos de prueba de integración verifican la interacción adecuada de componentes. Se derivan de realizaciones de casos de uso y deben ser eficientes, buscando un solapamiento mínimo para cubrir escenarios relevantes.

Diseño de Casos de Prueba de Sistema: Las pruebas de sistema aseguran que el sistema funcione correctamente en su conjunto, considerando diversas configuraciones y condiciones. Se priorizan combinaciones de casos de uso que puedan influenciarse mutuamente.

Diseño de Casos de Prueba de Regresión: Se utilizan casos de prueba de construcciones anteriores para pruebas de regresión, asegurando que sean flexibles y resistentes a cambios en el software.

Identificación y Estructuración de Procedimientos de Prueba: Los diseñadores proponen procedimientos reutilizables para cada caso de prueba, facilitando su mantenimiento y adaptación a cambios en subsistemas.

  
  

#### Actividad: Implementar Prueba![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf1Zuwmw6x7AgjhBPhxZC18vGJs0AyWMBNLlgWcEGR1CAahr-OhW7Y_b5qKXrzhtqWZfibggwYB1trovHKMmVkQs4cBvs3yB8npNgIGdJBYhJ-tEbnLs28NkIMyUsGZjDSuGK6FCr3JG1SvKa__wD1lu-pF?key=VReuh94fGGpJZLGsXsGdUQ)

Propósito: Automatizar procedimientos de prueba mediante la creación de componentes de prueba, usando herramientas de automatización o programación directa. Esto permite manejar grandes volúmenes de datos de entrada y salida.

  
  
  
  
  
  
  
  
  
  
  
  
  

#### Actividad: Realizar Pruebas de Integración![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIkFYJTKiRuoOaIEu1usV1UPcVm8DSDCAWYBVQssQFoSrX-H4IPdMuV8EVDG21CSzXIVrrZ-_5W_WY1FJtFfsunE8nPPyTVnNvjylvnUbDcQlZsj8wJ9rgws5sWiv90tUsb0kQI1gg7duY8q6kJM9h8mul?key=VReuh94fGGpJZLGsXsGdUQ)

Pasos:

1. Ejecutar pruebas de integración manualmente o mediante componentes automatizados.
    
2. Comparar resultados con los esperados e investigar discrepancias.
    
3. Informar defectos a ingenieros de componentes y diseñadores de pruebas.
    

  

#### Actividad: Realizar Prueba de Sistema![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcK6oO3zPY4MHt8iijvmkKZni6Z0PbJTAkiuOS5AtzolhOHcmGMS_q9aZfVsmUsF2cnwD9oDxnZGCNSBpF____yfdbvMyurUES9o39YE8V0cM7P0Y2sWxI3C6mVzsqRuHUrUBKYeEhd5K5MD_mdMeZf0hg2?key=VReuh94fGGpJZLGsXsGdUQ)

Propósito: Ejecutar pruebas de sistema cuando las pruebas de integración cumplen los objetivos de calidad establecidos. El proceso es similar al de las pruebas de integración.

  

#### Actividad: Evaluar Prueba![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeMcmJqCOQqI7hkGYKpCvzZRbYGyrWTkIEgnhn54VRWY7eYd5QIi4uMtBASg1ycAvm3To5512ycU7l-KEO8QD8hgt94Dd_7AiVzG0nSKgyHwYUtzUlKHqSHFRzzN59DbAhOkqg0?key=VReuh94fGGpJZLGsXsGdUQ)

Propósito: Evaluar los esfuerzos de prueba comparando resultados con objetivos del plan de prueba. 

Se analizan métricas de: 

- Completitud: Cantidad de código y casos de prueba ejecutados.
    
- Fiabilidad: Defecto contra el resultado esperado
    

Se documentan tendencias en defectos. Las acciones sugeridas pueden incluir pruebas adicionales, ajustes en los criterios de calidad o aislar las partes del sistema que parecen tener una calidad aceptable y entregarlas como resultado de la iteración actual.

  

### Resumen de Prueba

El resultado principal es el modelo de prueba, que incluye:

- Casos de prueba: Qué probar.
    
- Procedimientos de prueba: Cómo realizar las pruebas.
    
- Componentes de prueba: Automatización de procedimientos.
    

También se generan un plan de prueba, evaluaciones y defectos que pueden retroalimentar flujos de trabajo anteriores.