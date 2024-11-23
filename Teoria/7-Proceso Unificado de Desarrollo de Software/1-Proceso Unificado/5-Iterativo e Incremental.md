
---

## Desarrollo Iterativo Incremental

### Concepto
- Es práctico dividir el esfuerzo de desarrollo de un proyecto en partes más pequeñas o **mini proyectos**.
- Cada mini proyecto es una **iteración** que produce un **incremento** (artefactos del modelo).  
- Al finalizar una iteración, el conjunto de modelos del sistema alcanza un estado concreto llamado **línea base**.
- El nuevo incremento se integra con los resultados de iteraciones anteriores, generando una nueva versión del sistema.

### Diferencia entre Iteración e Incremento
- **Iteraciones**: Pasos en el flujo de trabajo fundamental.
- **Incrementos**: Crecimientos en el producto.

### Control de Iteraciones
- Las iteraciones deben estar controladas y planificadas.
- Selección de objetivos de iteración basada en:
  - **Casos de uso**: Aquellos que amplían la funcionalidad.
  - **Riesgos críticos**: Los que deben mitigarse primero.

### Proceso de Iteración
1. **Identificación y especificación de casos de uso relevantes**.
2. **Creación del diseño**: Basado en la arquitectura seleccionada.
3. **Implementación de los casos de uso identificados**.
4. **Evaluación de resultados**:
   - Si cumple los objetivos → Continuar con la siguiente iteración.
   - Si no cumple los objetivos → Revisar decisiones previas y probar un nuevo enfoque.

#### En casos extremos:
- Si una iteración es insatisfactoria, puede llevar a la cancelación del proyecto.

---

### Prueba de Regresión
- **Importancia**:  
  En ciclos iterativos e incrementales, cada iteración añade incrementos significativos y genera cambios importantes.
- **Función principal**:  
  Actuar como control de versiones, asegurando que los cambios y adiciones no rompan funcionalidades previas.

![[Pasted image 20241123172927.png]]

---

## ¿Que se pretende en cada fase?

![[Pasted image 20241123173106.png]]![[Pasted image 20241123173124.png]]![[Pasted image 20241123173156.png]]

### Flujos de trabajo
![[Pasted image 20241123173218.png]]
### Comparacion con el modelo en cascada

![[Pasted image 20241123173249.png]]
![[Pasted image 20241123173257.png]]

#### Beneficios del enfoque iterativo
- La iteración controlada reduce el riesgo a los costes de un solo incremento.
- **Reduce el riesgo** de retrasos en el calendario atacando los riesgos más importantes primero.
- **Acelera el desarrollo**. Los trabajadores trabajan de manera más eficiente al obtener resultados a corto plazo.
- Tiene un **enfoque más realista** al reconocer que los requisitos no pueden definirse completamente al principio.
- ![[Pasted image 20241123173500.png]]