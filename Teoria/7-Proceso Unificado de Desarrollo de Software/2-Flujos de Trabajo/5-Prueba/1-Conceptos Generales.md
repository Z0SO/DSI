## PRUEBAS

### **Propósitos de la Prueba**

Los objetivos principales de las pruebas son:

1. **Planificación de pruebas**:
   - Determinar qué pruebas realizar en cada iteración.
   - Incluir pruebas de integración en cada construcción y pruebas de sistema al final de la iteración.

2. **Diseño e implementación de pruebas**:
   - Crear casos y procedimientos de prueba.
   - Desarrollar componentes de prueba automatizables siempre que sea posible.

3. **Ejecución y gestión de resultados**:
   - Ejecutar las pruebas.
   - Registrar resultados.
   - Repetir pruebas en construcciones defectuosas, enviándolas a diseño o implementación para su corrección (enfoque iterativo e incremental).
   - ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXemWsOVaLg2NOGB6KYMdyMWlSRw3G5MoouHeN0yH7IghRURb6alrBzhw0bXFM-0LnR-G3jqUjkJuenGmnY1X00i8mXN2G2tSXYNmVYoi5fXcYhHUMW4YnNc5gwFTVywc3m_HF_Ms-aWLaGdrCLsWkIJut6o?key=VReuh94fGGpJZLGsXsGdUQ)

**Evolución del modelo de pruebas durante el ciclo de desarrollo**:
- En la fase de **inicio**, se planifican pruebas iniciales.
- En la fase de **construcción**, se prueba la línea base de arquitectura y las construcciones posteriores.
- En la **transición**, se realizan pruebas de regresión y depuración de defectos.

El modelo de pruebas evoluciona con:
- **Eliminación** de casos obsoletos.
- **Refinamiento** de casos existentes.
- **Creación** de nuevos casos.

---

### **Trabajadores y artefactos**

Los actores y artefactos clave en el proceso de pruebas se representan visualmente:
- ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfsCV87QXuPnGz9M0if5E1ulYHHWPy0M8DDuGTRNIVQ7JcQ81Qy8C9lTQ2lRArBJsrNyfZvV0wWz3urmodgsGSkx7ov3ESXEkv7NL6RYh-SUhX67vONYESBhBHBNkqJuq0YPIaklA?key=VReuh94fGGpJZLGsXsGdUQ)
- ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfAD0cBz13THQOSQGPO56I9fzTNhJLyg6Dd_Mm1mSOz-G3pMALvBLpMd8xxfxIYigtqOAhXyZJMdeP7T4QfLfLB47ZMCnSfHwruE6pnIE4DVyaI2j_Os1rQlWCBFCZcXHVb9to5z0Y8egRMbsyMl5i5BzY?key=VReuh94fGGpJZLGsXsGdUQ)

---

### **Artefactos principales**

1. **Modelo de Pruebas**:
   - Define cómo se realizan las pruebas en cada etapa.
   - Incluye:
     - Casos.
     - Procedimientos.
     - Componentes de prueba.
   - En sistemas complejos, se organiza en paquetes.
   - ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfz0N3fVyesgOlSnzZnRwI3zvvwdKg4wwsoQ-XiuxY66Tt4zV4MIEJUE70FZeP9rtEz2l0T-TclAUjTa5A3wVM2u5YL7mVqE6OuGbAkx-A_3qaWq53czYVXgAT4-HMZYZn4Q4LaV82BOYKxPgna7xfvF5Mv?key=VReuh94fGGpJZLGsXsGdUQ)

2. **Caso de Prueba**:
   - Evalúa un aspecto del sistema, basado en uno o varios requisitos.
   - Define:
     - Entradas.
     - Resultados esperados.
     - Condiciones de ejecución.
   - Tipos:
     - **Caja Negra**: Evalúa el comportamiento externo, basado en casos de uso.
     - **Caja Blanca**: Prueba interna de una realización del diseño.
   - También incluye pruebas:
     - De instalación.
     - De configuración.
     - Negativas (verificar fallos).
     - De estrés.
   - ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeR3abOS3aaWwUiCxhUCNyUh-CB2UZE3TelP1-2iXlpGcYaX00k2uFWcAf0r6jD5OwXjaqwUDRZFmbWjAoEqED4LKV4sVWHnXKN8NkaTbd6zW6jG1GokP556tye4oyqReSReemaKZrR7Uk0rnMdkNCJ6FE9?key=VReuh94fGGpJZLGsXsGdUQ)

3. **Procedimiento de Prueba**:
   - Detalla cómo ejecutar los casos de prueba.
   - Puede ser:
     - **Manual**.
     - **Automatizado**.
   - Secuencia de pasos con entradas y salidas esperadas.
   - ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeW-bV90vEXyoFkhUWJxbuW2TEbjW7obdEusWYQI7lxC04P-rt_umARM1RZn_7vJtLSE4PUP2sZ7gKhI0N6cveRqD9z-2EyqZc0O5wqYGpeL2qLnWPKBrYwZ5PEAg2XXQAmWr11O8UTN78LUvyuWOEf-KnF?key=VReuh94fGGpJZLGsXsGdUQ)

4. **Componente de Prueba**:
   - Automatiza procedimientos, proporcionando entradas y monitoreando la ejecución.
   - Conocidos como "drivers" o "test harnesses".
   - ![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIJKEk6NOxouPUq-QMUytsaFJLEoCx-tMjn77_6grwQ3M4prIgPKVrHRTIVoJKXzHL426coDJNlGh0htxNt4rSuiGewb8HDVP3_SpNGhuUAmw8KP0huwWHBxs3rVZnZV7AWRYtghy-xZZZFjPERbmi0W4?key=VReuh94fGGpJZLGsXsGdUQ)

5. **Plan de Prueba**:
   - Establece estrategias, recursos y planificación de las pruebas.
   - Define:
     - Tipos de pruebas.
     - Objetivos.
     - Cobertura esperada.
     - Resultados deseados.

6. **Defecto**:
   - Anomalía detectada que debe corregirse.
   - Puede ser:
     - Error de software.
     - Problema identificado en revisiones.

7. **Evaluación de Prueba**:
   - Analiza la efectividad del proceso de pruebas.
   - Revisa:
     - Cobertura lograda.
     - Estado de los defectos detectados.
# Pruebas de Software

## **Trabajadores**

### **Diseñador de Pruebas**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfCezEUqKliiUFrPBOlst8i65jFRdncQTbaxPo1eGQmxYwFDHo7UoRyL1YNB55ZGXb5IWRPKLOhFZi1mvpP7INXSiddXS5SBwTSLDPl48Tj3epfSRsmpglBqrGIUA1BDxR4Z68Pv8yWb8bKcREO87crT9bZ?key=VReuh94fGGpJZLGsXsGdUQ)

- **Responsabilidad**: Garantizar la integridad del modelo de pruebas. **Solo planifica y evalúa.**
- **Funciones**:
  - Planificación de objetivos y procedimientos de prueba.
  - Selección y descripción de casos de prueba.
  - Evaluación de pruebas de integración y sistema.

---

### **Ingeniero de Componentes**
- **Responsabilidad**: Crear componentes de prueba que automatizan procedimientos.
- **Habilidades requeridas**: Conocimientos avanzados en programación.

---

### **Ingeniero de Pruebas de Integración**
- **Responsabilidad**: Realizar pruebas de integración para verificar el funcionamiento de los componentes.
- **Funciones**:
  - Documentar los defectos encontrados.
  - Basarse en casos de prueba derivados del diseño de casos de uso.

---

### **Ingeniero de Pruebas de Sistema**
- **Responsabilidad**: Realizar pruebas de sistema sobre el resultado ejecutable de una iteración.
- **Funciones**:
  - Verificar interacciones entre actores y el sistema.
  - Documentar defectos encontrados.
  - **Nota**: Usualmente requiere conocimiento interno de la estructura del sistema.

---

## **Flujo de Trabajo**
El objetivo es **realizar y evaluar pruebas** siguiendo un modelo estructurado. Las etapas principales incluyen:

1. **Planificación de Pruebas**: Los ingenieros de prueba organizan el esfuerzo en cada iteración.
2. **Descripción de Casos de Prueba**: Se identifican los casos y procedimientos necesarios.
3. **Creación de Componentes de Prueba**: Los componentes automatizan procesos donde sea posible.
4. **Ejecución en Construcciones**: Este ciclo se repite para cada nueva construcción.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdlFisDXbxJ1eTgF7zeNbfIbwn2-KWB2PetAZhP1SscT2EhO5NcFuNty-W7XypunWJuBoIJCxyISpl9B19HzchPzXO54kyvcRoltAMRYB1nSWG1YkHZxOh0MXzfyW1ELThrXW4JnqI7AEKSsG9L4xnKe-M?key=VReuh94fGGpJZLGsXsGdUQ)

---

## **Actividades**

### **Planificar Prueba**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcSYPJws297dHmPHt1RG0vP6dJ8Yr7cgpNVBx3QeSZXqqWsBKgpd2BynsGpk43u-xfg6FWKFSSikKRevHnk7Uqd_zSB56QnSM2Bkb67XFpNbRMp6NhuznJ755gulfIafHeuU0rDQW1hS7mmL331GIyprfXN?key=VReuh94fGGpJZLGsXsGdUQ)

- **Propósito**: Organizar esfuerzos de prueba mediante:
  - Definición de estrategias de prueba.
  - Estimación de recursos.
  - Priorización de casos de alto impacto y riesgo.

---

### **Diseñar Prueba**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXduJ-yiWL-3IbiVkNff_J1_frGzn_vnrnj546wV3ZWTN1hjP6MK8g1IZ3yvTnWzM1Mh18frG53UMSGfuYM7_tliZdB1cEq36axx9MxLnGsQf6tLNS-rp_FI04TWcgRBsu324SMvgRFNYNbmHKr6-e-X3cNZ?key=VReuh94fGGpJZLGsXsGdUQ)

- **Propósitos**:
  - Identificar y estructurar casos de prueba:
    - **De integración**: Validan interacción entre componentes.
    - **De sistema**: Verifican funcionamiento general.
    - **De regresión**: Aseguran que no haya retrocesos en la calidad.
  - Crear procedimientos reutilizables para casos de prueba.

---

### **Implementar Prueba**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf1Zuwmw6x7AgjhBPhxZC18vGJs0AyWMBNLlgWcEGR1CAahr-OhW7Y_b5qKXrzhtqWZfibggwYB1trovHKMmVkQs4cBvs3yB8npNgIGdJBYhJ-tEbnLs28NkIMyUsGZjDSuGK6FCr3JG1SvKa__wD1lu-pF?key=VReuh94fGGpJZLGsXsGdUQ)

- **Propósito**: Automatizar pruebas mediante herramientas o programación directa, asegurando eficiencia en la ejecución.

---

### **Realizar Pruebas de Integración**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfIkFYJTKiRuoOaIEu1usV1UPcVm8DSDCAWYBVQssQFoSrX-H4IPdMuV8EVDG21CSzXIVrrZ-_5W_WY1FJtFfsunE8nPPyTVnNvjylvnUbDcQlZsj8wJ9rgws5sWiv90tUsb0kQI1gg7duY8q6kJM9h8mul?key=VReuh94fGGpJZLGsXsGdUQ)

- **Pasos**:
  1. Ejecutar pruebas.
  2. Comparar resultados esperados con obtenidos.
  3. Reportar defectos a los responsables.

---

### **Realizar Prueba de Sistema**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcK6oO3zPY4MHt8iijvmkKZni6Z0PbJTAkiuOS5AtzolhOHcmGMS_q9aZfVsmUsF2cnwD9oDxnZGCNSBpF____yfdbvMyurUES9o39YE8V0cM7P0Y2sWxI3C6mVzsqRuHUrUBKYeEhd5K5MD_mdMeZf0hg2?key=VReuh94fGGpJZLGsXsGdUQ)

- **Propósito**: Validar el sistema como un todo, asegurando que cumple los objetivos de calidad.

---

### **Evaluar Prueba**
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeMcmJqCOQqI7hkGYKpCvzZRbYGyrWTkIEgnhn54VRWY7eYd5QIi4uMtBASg1ycAvm3To5512ycU7l-KEO8QD8hgt94Dd_7AiVzG0nSKgyHwYUtzUlKHqSHFRzzN59DbAhOkqg0?key=VReuh94fGGpJZLGsXsGdUQ)

- **Propósito**: Comparar resultados obtenidos con los objetivos del plan de pruebas, revisando:
  - **Completitud**: Proporción de código y casos de prueba cubiertos.
  - **Fiabilidad**: Cantidad y gravedad de defectos encontrados.

---

## **Resumen de Prueba**

El modelo de prueba incluye:
- **Casos de prueba**: Qué probar.
- **Procedimientos**: Cómo realizar las pruebas.
- **Componentes**: Automatización para mayor eficiencia.

Se generan:
- Un plan de prueba.
- Evaluaciones y métricas.
- Documentación de defectos que retroalimentan el proceso.

---
