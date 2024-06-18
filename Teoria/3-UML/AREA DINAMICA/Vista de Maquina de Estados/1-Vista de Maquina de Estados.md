# Vista de Máquina de Estados

La vista de máquina de estados describe el comportamiento dinámico de los objetos, **modelando su ciclo de vida a través de autómatas finitos con estados y transiciones.** 

Cada objeto se trata de forma aislada, detectando eventos y respondiendo a ellos, comunicándose con el resto del mundo.

## Utilidad

Es útil modelar el **comportamiento estado-dependiente** de **objetos específicos**, centrándose en su **ciclo de vida** y **cómo su estado afecta su comportamiento.**

## Diagramas de Estado

Los diagramas de estado son la representación gráfica principal en esta vista. Pueden ser instancias de clase, casos de uso o sistemas completos, y se centran en una clase en particular, no en la relación entre objetos.


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXc2RNDqM3Og1JR0J91VoqSa3lPvNAwMYUxjYhoaKhJc1AU6ZhaMli78UlwUuw4UUROyEfoBl1_sMmix3FA3zVnxiWNLJGu9EGL8npSG5Q-DvSR2rpnCE7n9CFe-QkqiDWSEud1dslmi3Mh71ssUjJSJK2p1?key=VReuh94fGGpJZLGsXsGdUQ)

## Elementos

- **Estado**: Condición o situación en la vida de un objeto durante la cual satisface alguna condición, realiza alguna actividad o espera algún evento. Representado gráficamente como un rectángulo con las esquinas redondeadas.
- **Evento**: Especificación de un acontecimiento significativo situado en el tiempo y en el espacio que puede disparar una transición de estados.
- **Transición**: Relación entre dos estados que indica que un objeto realizará ciertas acciones y entrará en el segundo estado cuando ocurra un evento especificado y se satisfagan unas condiciones especificadas. Representada como una línea continua dirigida desde el estado origen al nuevo estado.
- **Actividad**: Ejecución no atómica en curso dentro de una máquina de estados.
- **Acción**: Computación atómica ejecutable que produce un cambio en el estado del modelo o devuelve un valor.

## Cuándo Modelar con Máquinas de Estados

Conviene modelar a través de una máquina de estados cuando hay una dependencia muy grande del estado de un objeto, que afecta su comportamiento y es necesario entender cómo funciona en diferentes situaciones.

---

> La vista de máquina de estados es fundamental para comprender el comportamiento dinámico de los objetos en un sistema, permitiendo modelar su ciclo de vida y las transiciones entre diferentes estados en respuesta a eventos significativos.
