
----

# Ciclo de Vida del Desarrollo de Software

## Definición

**Según IEEE**
- **Ciclo de Desarrollo de Software**: Abarca desde el inicio hasta la entrega del software.
- **Ciclo de Vida del Desarrollo**: Abarca desde el inicio hasta el final del software, incluyendo su entrega y eventual desuso.

#### Modelo de Procesos de Software
- **Presentación Simplificada**: Representa el ciclo de vida del software sin detallar actividades específicas.
- **Adaptabilidad**: Permite la adaptación o extensión según el modelo elegido.
- **Tipos de Modelos**:
  - **Cascada**
  - **Prototipo**
  - **Espiral**
  - **Iterativo e Incremental**

#### Modelos de Proceso según Pressman

**Flujo de Proceso**
- Organización secuencial y temporal de actividades en los modelos de desarrollo.
- **Tipos**:
  - **Lineal**: Actividades realizadas en secuencia.
  - **Iterativo**: Repetición de actividades con mejoras en cada iteración.
  - **Evolutivo**: Desarrollo en etapas con prototipos y refinamientos sucesivos.
  - **Paralelo**: Actividades realizadas simultáneamente para acelerar el desarrollo.

**Prescriptividad**
- Define elementos de proceso y flujo de trabajo.
- **Alta Prescriptividad**: Detalle minucioso de actividades y tareas, útil para entornos con requisitos estables.
- **Baja Prescriptividad**: Mayor flexibilidad y adaptación, útil para entornos cambiantes.


----
# Modelos Clásicos de Desarrollo de Software

##### Cuadro Comparativo

| **Modelo**                  | **Características**                                                                                                                                                                                                                                                                    | **Ventajas**                                                                                              | **Desventajas**                                                                                                                            |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **Cascada**                 | - Actividades secuenciales claras.<br>- Etapas bien definidas: requisitos, diseño, implementación, pruebas, mantenimiento.                                                                                                                                                             | - Claridad y simplicidad en la gestión del proyecto.                                                      | - Dificultad para gestionar cambios y retrocesos.<br>- Rigidez en la adaptación a requisitos cambiantes.                                   |
| **Prototipos**              | - Iterativo, con prototipos presentados al cliente.<br>- Combina bien con otros modelos de desarrollo.                                                                                                                                                                                 | - Reducción del rechazo del producto por parte del cliente.<br>- Mejora en la comunicación de requisitos. | - Posible pérdida de trabajo en prototipos desechables.<br>- Dificultad en la planificación precisa del proyecto.                          |
| **Espiral**                 | - Dirigido por riesgos.<br>- Iterativo, con prototipos en cada vuelta del espiral.                                                                                                                                                                                                     | - Reducción de riesgos en el desarrollo.<br>- Flexibilidad y adaptabilidad.                               | - Complejidad en la gestión del proyecto.<br>- Requiere experiencia en la identificación y gestión de riesgos.                             |
| **Iterativo e Incremental** | - Incremental: Construcción de subsistemas que se integran en el sistema completo.<br>- Iterativo: Mejora y refinamiento continuo de la funcionalidad.<br>- Iterativo e Incremental: Combina ambos enfoques, permitiendo la entrega de versiones con nuevas funcionalidades y mejoras. | - Adaptabilidad a cambios.<br>- Entregas frecuentes y manejables.                                         | - Requiere una gestión eficiente para coordinar iteraciones e incrementos.<br>- Puede complicar la planificación y estimación de recursos. |

## Cuadro Comparativo (Enfoques de Desarrollo)

| **Plan Driven** | - Dirigido por un plan detallado.<br>- Alta prescriptividad.                                          | - Claridad y control en la gestión del proyecto.<br>- Previsibilidad y consistencia en los resultados. | - Rigidez ante cambios.<br>- Puede ser ineficiente en entornos dinámicos y cambiantes.                             |
| --------------- | ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| **Agile**       | - Enfoque incremental y adaptable.<br>- Baja prescriptividad, flexibilidad en el plan y el resultado. | - Adaptabilidad y respuesta rápida a cambios.<br>- Mayor colaboración y comunicación con el cliente.   | - Requiere una alta disciplina y coordinación.<br>- Puede ser difícil de escalar en proyectos grandes y complejos. |


### **Modelo en Cascada**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcm63ZvxMHOA1UamnvEQOtf8bRKknucCEbow7tkuZ_ylx7vJdsXpzHDAV9OHt-FSORUPWhqFc4pH-dgx-K50V9ZpgsMBH1kXmbX9E8Sna5ZY7-iQlaGZ7cYNrvunk6PsidOwjl7g8BckRZaKzgFfqJi6gEm?key=VReuh94fGGpJZLGsXsGdUQ)

- **Características**: 
  - Actividades secuenciales claras.
  - Etapas bien definidas: requisitos, diseño, implementación, pruebas, mantenimiento.
- **Ventajas**: 
  - Claridad y simplicidad en la gestión del proyecto.
- **Desventajas**: 
  - Dificultad para gestionar cambios y retrocesos.
  - Rigidez en la adaptación a requisitos cambiantes.

### **Modelo de Prototipos**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfGr5Gsni6b5rraXfBKoYJz6iOwhCreTz3dN4QyuFhUrmedPxCb4QX5HnlG9qVTERH9HdfKHV2xUn1kqkEJ5deh5TufSmuwTl9zxXO8h68IbRRg2OuWm5rbMK_Pvm6bELcXJsTGENdBcELcT8dFtOgwul3o?key=VReuh94fGGpJZLGsXsGdUQ)

- **Características**: 
  - Iterativo, con prototipos presentados al cliente.
  - Combina bien con otros modelos de desarrollo.
- **Ventajas**: 
  - Reducción del rechazo del producto por parte del cliente.
  - Mejora en la comunicación de requisitos.
- **Desventajas**: 
  - Posible pérdida de trabajo en prototipos desechables.
  - Dificultad en la planificación precisa del proyecto.

### **Modelo Espiral**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXca4lGMIx3FDN2FxZCAG6tTdJZisgQ-WZ7QUuJQfSYzSDQ8_C7rJJ7EBeNwCsr1tXHXlh94e0JjlRTC98zLGl6uYk-x04Rxs-KsUbqHkXqK2PlvmpWl7EuX30Jp8g41SHPMMGrv8JoPzPoUb7SjNSdalGKI?key=VReuh94fGGpJZLGsXsGdUQ)

- **Características**: 
  - Dirigido por riesgos.
  - Iterativo, con prototipos en cada vuelta del espiral.
- **Ventajas**: 
  - Reducción de riesgos en el desarrollo.
  - Flexibilidad y adaptabilidad.
- **Desventajas**: 
  - Complejidad en la gestión del proyecto.
  - Requiere experiencia en la identificación y gestión de riesgos.

### **Modelo Iterativo e Incremental**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcJ9YsvpnPKv5PeM_ev8MD8J6cr-YaIzPQnxmL2GG_j4kDcxTntgePcaOFSMBICtt9uRC6MRfhDI8u3YiJq0dDqOBLBq7DGtAmQbHJKx3CnS4raPJTkYkOffi2k10A21ufYKiCDKd-Ns7jgqHAeu8P_wSbi?key=VReuh94fGGpJZLGsXsGdUQ)

- **Características**: 
  - **Incremental**: Construcción de subsistemas que se integran en el sistema completo.
  - **Iterativo**: Mejora y refinamiento continuo de la funcionalidad.
  - **Iterativo e Incremental**: Combina ambos enfoques, permitiendo la entrega de versiones con nuevas funcionalidades y mejoras.
- **Ventajas**: 
  - Adaptabilidad a cambios.
  - Entregas frecuentes y manejables.
- **Desventajas**: 
  - Requiere una gestión eficiente para coordinar iteraciones e incrementos.
  - Puede complicar la planificación y estimación de recursos.



#### Enfoques de Desarrollo

**Plan Driven**
- **Características**: 
  - Dirigido por un plan detallado.
  - Alta prescriptividad.
- **Ventajas**: 
  - Claridad y control en la gestión del proyecto.
  - Previsibilidad y consistencia en los resultados.
- **Desventajas**: 
  - Rigidez ante cambios.
  - Puede ser ineficiente en entornos dinámicos y cambiantes.

**Agile**
- **Características**: 
  - Enfoque incremental y adaptable.
  - Baja prescriptividad, flexibilidad en el plan y el resultado.
- **Ventajas**: 
  - Adaptabilidad y respuesta rápida a cambios.
  - Mayor colaboración y comunicación con el cliente.
- **Desventajas**: 
  - Requiere una alta disciplina y coordinación.
  - Puede ser difícil de escalar en proyectos grandes y complejos.


---
