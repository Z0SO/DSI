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