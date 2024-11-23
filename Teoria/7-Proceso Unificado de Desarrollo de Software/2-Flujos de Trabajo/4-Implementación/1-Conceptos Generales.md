# IMPLEMENTACIÓN

## Propósitos de la Implementación

1. **Planificación Incremental**  
   La implementación se organiza en iteraciones con pasos pequeños y manejables. Esto permite:
   - Integrar componentes gradualmente.
   - Facilitar el seguimiento del progreso y la corrección de errores.

2. **Asociación de Componentes con el Diseño**  
   - Los componentes ejecutables se asignan a nodos de despliegue basándose en lo definido durante el diseño.
   - Cada componente (archivos de código fuente) corresponde a clases o subsistemas identificados previamente.

3. **Pruebas y Validación**  
   - Los componentes se prueban individualmente antes de integrarlos en ejecutables.
   - Se realizan pruebas de integración y sistema para garantizar funcionalidad y robustez.

4. **Fase de Construcción**  
   - La implementación es la etapa de programación intensa, donde se escriben y prueban las piezas del sistema.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXflA-1j4GnGa7U5maD4MZ7bW-s4fC-bdUnQX5H0LbXgBCC0d7w3NbjvQuW7g2p4I5dPU-CsuZ0xohn54Gt0pFeCTa0Hw3xHANuDU-Ie6iFAM8Cohl8grR01bj1YN5bcXejvXDtuUTm0Y1SVe1UcWYpPdY9u?key=VReuh94fGGpJZLGsXsGdUQ)

---

## Trabajadores y Artefactos

- **Artefacto: Modelo de Implementación**  
  Describe cómo los elementos del diseño (como clases) se transforman en componentes ejecutables.  
  Organización jerárquica:
  - Subsistemas de nivel superior dividen el modelo en partes manejables.  
  - Los componentes (archivos, librerías, tablas) implementan clases del diseño.  

  ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXem3HRgg9YOq0nWk6uFK5kTlHhoD03ptOYQWjFqcPE8J3rHIoEaLdBx2uh2TUXarzws7PttOLHPfs6gECfuGcCCrfgc0F6fEAi_tJyNIqNknYJhCUv76Hep-hhc75KMvq5GKS0N-7Bq0IEN6OaZEz4N5h4?key=VReuh94fGGpJZLGsXsGdUQ)

### Componentes

- **Definición**  
  Un componente empaqueta elementos del modelo (como clases) y puede ser:
  - Ejecutable.
  - Archivo de código fuente.
  - Librería.
  - Tabla o documento.

- **Características**  
  - Relación de traza con el modelo de diseño.  
  - Implementan clases múltiples y exponen interfaces correspondientes al diseño.

  ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfdvUL49d_u7pgyfG33ATv9OdlxJPcmM8vSZO7lLekSBo2LMJYd7LvwgUNivAVvNX5mOW3cs46C_-3onIVWkOhpVPAuN3ksunetF-mH0kJ_tVTOKxBKyL04mdhqj5BxOCGqAJOY9Qzl5QqFn5QmcZQvuu0?key=VReuh94fGGpJZLGsXsGdUQ)

- **Dependencias de Compilación**  
  - Indican qué componentes son necesarios para compilar otros.
  - Los stubs (implementaciones mínimas) permiten pruebas y desarrollo inicial.

---

### Subsistemas de Implementación

- **Definición**  
  Agrupan componentes e interfaces en estructuras manejables.

- **Relación con el Diseño**  
  - Mantienen trazabilidad con los subsistemas de diseño.  
  - Conservan las interfaces y dependencias especificadas.  

  ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXetgmMQaYqRmUTFa7RNfGkTcCPBxm7jhHEW2Xw6Et7Zofc7-aG06xrkGQZbCqCRO5-AkCHt451mL4J7XTeVxx8AI9kp9721wGU360SLYs3qjtY6bRub6fMgRdh0MVYb4VVa4YELzEA4JSTSf4bI_bEfMtI?key=VReuh94fGGpJZLGsXsGdUQ)

---

### Interfaces

- **Propósito**  
  - Especifican operaciones que los componentes o subsistemas implementan.  
  - Aseguran consistencia entre diseño e implementación.

  ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXexZQ6MN5_zOh5F0uzCr8i0UcQwD6LHd0KCVx9VemQcFlxTJDzL_PHY9S1yHxNDNZH2pwomXr_jIHZqwZFs-TSmpbLwYsRMmK03KQuTkvq3NAylQNkXx4M5xefMJuv36t1HgDJjkfSiAw4pX5X9kKNNOHA_?key=VReuh94fGGpJZLGsXsGdUQ)

---

### Descripción de Arquitectura

- **Contenido**  
  - Detalla la estructura de subsistemas y componentes clave.  
  - Enfatiza subsistemas trazables a diseño.

  ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeblgyXP1rMBgarXwv6IxrgmkSftsX0KggCEfSS7GO3Loi6tDtRaaDt0h53SEx0DHaR9GZzLfrPNyH7WZPzAknhaZiSYXHpcVtiWadPT06Nexi-rO1vnQJdKtslFRZzVGSeH1XkmlWQMLo1b2L8UvonkZGM?key=VReuh94fGGpJZLGsXsGdUQ)

---

### Plan de Integración de Construcciones

- **Objetivo**  
  Crear software incrementalmente mediante versiones funcionales probadas.

- **Beneficios**  
  - Permite pruebas tempranas.  
  - Facilita detección y corrección de errores.  
  - Asegura que cada paso del desarrollo añade funcionalidad estable.

---


### TRABAJADORES

#### Arquitecto 
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfsKQpip1khZVTGcQ7pnP52SMvIzxpWIexV_ez2N_G3kV47mHJurANibbAqKAVto6xYj9m5hVMS_jjpki6AfTIyltF07VlYgFBblS6MsnSaORn6rJLw26oBHHZt_VyF3tUtKXQ-z0DW1xQtYheSy1xTbFNZ?key=VReuh94fGGpJZLGsXsGdUQ)

- Supervisa la arquitectura del modelo.
- Asigna componentes a nodos para el despliegue.
- No realiza desarrollo continuo; eso es tarea del ingeniero de componentes.

#### Ingeniero de Componentes  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfhOUwc1EA7iFtwDbGFWZRsdVPbcySzmpLWs1hUDTQOyc7lKUFb_gv-YcbVv8W9fUbaZMBXZ3xj9YZf_xiLA0pC-7C_1iMJHn9SUBZpdHH51kl4ZPI41w5QFb3Rn_QVZqapXgXV5wcIESKO6iKgV7xcwBJ9?key=VReuh94fGGpJZLGsXsGdUQ)

- Implementa y mantiene el código de componentes y subsistemas.
- Garantiza que las clases cumplan con el diseño y funcionalidad.

#### Integrador de Sistemas  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdLiBs8pJg8hbVhUoy7nu3MkF-mzMUJBgiN4k1LrrD4ladSvTiqw6ZiONfjOh-1KudpqbJ92pd6sQo5u-trFAOzrZKYAh41GoDNL74syifNxv482MF54vhmGMieTlt95Ns9Y3Xi6qhb6o1ZW60SGBfmHbBt?key=VReuh94fGGpJZLGsXsGdUQ)

- Planifica y organiza la integración de componentes.
- Garantiza que el sistema funcione como un todo tras cada iteración.

---

### FLUJO DE TRABAJO DE IMPLEMENTACIÓN  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeRnvkEbVfOb2JmFdRF3wUYO2nQmfrh4VDNo0o5TnxkO3xzYfxMnVwx8f-dh_dihXCmw6ohoaKVJOW7bDDiosXcZTkqC34A0SOFEeSSr6gJ20g4gcNwRNkwltEDpTDBiPsc_y0QlwGXxgjdDEDwnyZ8QkF7?key=VReuh94fGGpJZLGsXsGdUQ)

1. **Definición de componentes clave por el arquitecto.**
2. **Planificación de integraciones por el integrador de sistemas:**
   - Establece funcionalidad y subsistemas para cada iteración.
3. **Implementación y pruebas por ingenieros de componentes.**
4. **Verificación final y análisis de defectos antes de la siguiente fase.**

---

#### Actividades de Implementación

**1. Implementación de la Arquitectura**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcZTItSf-q6O8sp8EWm4QaKgr6BNIEj-MobRL6rfU90zlpHW4GjIj08jJ9A_bo41zLkYw5ZYErN1BUzvX8IHYc_ItXB1_Oatbnx0VN18PUqALY0yVHYekD7kkae-KwtZeZegZ00c-wLr7uI4lawAsODZw1p?key=VReuh94fGGpJZLGsXsGdUQ)

- **Identificación de componentes clave:**
  - Seleccionar componentes significativos y evitar crear detalles irrelevantes.
- **Asignación de componentes a nodos:**
  - Basarse en el diseño y organizar la estructura de despliegue.

---

**2. Integración del Sistema**  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe2UctoNoVvDAajviRymQGBxIkKwyI3IpKVvUUMmM6l8T9OtZaIYJn6g4qKp1js5LUtVSn7B6O0Tx4WXblmB3uzLGjx4thBlXu2YozYjAHifrjQ8RiRAy-Dg_kKkNBOJ-csynQLa-aIlpHUm2gCvSe0ZcHg?key=VReuh94fGGpJZLGsXsGdUQ)

- **Planificación de construcción:**
  - Organizar integración para facilitar pruebas y evitar dependencias cruzadas.
  - Uso de *stubs* para simular partes incompletas.
- **Integración de una construcción:**
  - Compilación respetando la jerarquía y evitando problemas de dependencias.

---

**3. Implementación de Subsistemas**  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe0OL6NRa6lF1dsYwzdGBXr2dk6bKgzSKZiO7f_2XEOkRLTgtirmICAj7R023QVI8kyo_Y0OBgidofFLYK0ClcqRNdaWxuSXTHYWjkJ2708HVZzVgm86rsZ3Dt4jhJMUKtAkxb4fQ?key=VReuh94fGGpJZLGsXsGdUQ)

- **Mantenimiento de contenidos:**
  - Implementar clases y refinar componentes según necesidades.
- **Implementación de interfaces especificadas.**

---

**4. Implementación de Clases**  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcKm4mHkZno-becSfaQX1NYspUBotTW98Gcj7XgS1IGq3AmzgKS-gM1T1mRIPNi1ixt7S4ATeQRgrqbDX1GZdbGlWTDhmdZs3kkpTv3rndh64MjoyUZNDHTIfzORQQg8vk_YPPRlWiz839dBdr_jpdsgKNF?key=VReuh94fGGpJZLGsXsGdUQ)

- Generar código a partir de clases de diseño.
- Implementar métodos, atributos y relaciones respetando convenciones del lenguaje.

---

**5. Realización de Pruebas Unitarias**  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcmtKU_W5RlY03Fj5a0Ap0n7JsvYXVBPjl1M9IqIMZPjLBW6VAjHeyb5IUc2Cds1JC7I5zTm74NeYR4UMXltOCwKqGM1wvQ4nX_3Q8KSHUit44dQ6cKeix92z0reyILfHr7DoQvMr6zBocRKjQnDbDr8WlB?key=VReuh94fGGpJZLGsXsGdUQ)

- **Caja negra:** Verifica comportamiento externo.  
- **Caja blanca:** Evalúa implementación interna.
- Complementar con pruebas de rendimiento e integración.

---

### Resumen
El modelo de implementación debe incluir:
- Subsistemas diseñados e implementados.
- Pruebas completas para garantizar funcionamiento.
