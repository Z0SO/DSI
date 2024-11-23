# Transiciones

Las transiciones son arcos que conectan dos vértices (estados) en un diagrama de estado, representando el pasaje de un estado a otro en respuesta a un evento específico. Cada transición tiene cinco características esenciales:

- **Estado Origen**: El estado desde el cual se inicia la transición.
- **Evento Disparador**: El evento que desencadena la transición.
- **Condición de Guarda**: Una condición opcional que debe cumplirse para que la transición pueda ocurrir.
- **Acción (Efecto)**: Una acción opcional que se ejecuta al ocurrir la transición.
- **Estado Destino**: El estado al cual se transita después de que se completa la transición.

Una transición no es instantánea y puede tardar un tiempo en ejecutarse, siendo el evento el elemento instantáneo que la activa.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXd0kWj0MN-QOWp4cMtrxJQrcbw-XBMDoYhD-RjA11fjpa0bd31tNO9LhYfk8_PN9vAkYMlpqtJ35PEdct4uSxnDH0aXcDseCet271yyHUlTr6Vcb550aLPBZi3Ed_LaAnHjMHV1f-1QAYJzEh3_u5tFGAs?key=VReuh94fGGpJZLGsXsGdUQ)

## Tipos de Transiciones

### Externa
Es aquella que pasa de un estado a otro, incluyendo la auto transición (bucles) donde el estado origen y destino son el mismo. Se ejecuta cualquier comportamiento de salida asociado al estado origen.

### Interna
Es una transición especial que permanece dentro del mismo estado, sin salir ni entrar de él. Se activa por eventos y puede ejecutar una acción, pero no hay cambio de estado ni ejecución de comportamientos de salida o entrada.

### Local
Contrario a la transición externa, permanece dentro del estado que la contiene y no se ejecuta el comportamiento de salida de dicho estado. Sin embargo, el estado destino debe ser diferente del estado origen. Solo puede existir dentro de un estado compuesto.

### De Finalización
No requiere un evento explícito, ya que sucede como consecuencia de la finalización de una actividad en el estado origen. Es utilizada para representar la terminación de una actividad o proceso, siendo accionada por la finalización de la actividad del estado del que se sale.

---
## Ejemplo: Servir Café

1. El sistema entra en el estado "Preparando", donde calienta el agua y muele los granos de café.
2. Una vez que ambas tareas han terminado, se genera un evento de finalización.
3. Este evento provoca una transición automática al estado "Listo".
4. En el estado "Listo", se sirve el café al usuario.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXc3Z-UWMHon_-QlDrH_1_noUd4DCcjpXwin4m4hlB8FbAtInMtORiu5ITjy6A4pOne1AAs_Yk1LeAp_t6gVEj6g-5W66w6oeyJQt_2AIOG0Zn2ZWPuhXUK1QQyc3fzy7Rs-VZRkDkDKlMMueSjjcSYT1vH4?key=VReuh94fGGpJZLGsXsGdUQ)

![[Pasted image 20240805213803.png]]

Las transiciones son fundamentales para modelar el comportamiento dinámico de un sistema y definir cómo responde a eventos y condiciones específicas.

> Las transiciones en un diagrama de estado representan el pasaje de un estado a otro en respuesta a eventos específicos, definiendo el comportamiento dinámico de un sistema y cómo responde a diferentes condiciones.
