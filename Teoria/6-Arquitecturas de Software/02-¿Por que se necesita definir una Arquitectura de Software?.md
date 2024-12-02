
## Arquitectura de Software

### ¿Por qué es importante definir la Arquitectura de Software?

1. **Potencia los atributos de calidad del sistema**  
   - Se enfoca en aspectos no funcionales: seguridad, rendimiento, modificabilidad, usabilidad, reutilización, etc.  
   - Ejemplo: Si el sistema debe ser seguro, la arquitectura definirá elementos que resguarden el acceso a la información.

2. **Facilita el razonamiento y la gestión de cambios**  
   - Los cambios pueden clasificarse en:  
     - **Local**: Afectan solo un elemento.  
     - **No local**: Involucran múltiples elementos.  
     - **A nivel de arquitectura**: Requieren modificar todo el sistema.

3. **Mejora la comunicación entre las partes interesadas (stakeholders)**  
   - La arquitectura es abstracta y comprensible para todos: clientes, gerentes, desarrolladores, etc.  
   - Permite que el arquitecto tome decisiones basadas en los requerimientos de las partes interesadas.

4. **Incluye decisiones de diseño tempranas y difíciles de cambiar**  
   - Analogía: Cambiar la base de una casa construida implica derribarla completamente.

5. **Define restricciones para la implementación**  
   - El arquitecto establece atributos de calidad y recursos asignados (ejemplo: límites de tiempo o memoria).  
   - Si cada parte cumple con estas restricciones, el sistema respeta la arquitectura.

6. **Influye en la estructura organizacional (y viceversa)**  
   - La arquitectura divide responsabilidades entre los equipos de trabajo.  
   - La experiencia de los equipos también puede influir en las decisiones arquitectónicas.

7. **Permite un desarrollo incremental**  
   - Una vez definida, se crea un "esqueleto" del sistema que se expande iterativamente.  
   - Cada iteración implementa casos de uso específicos.

8. **Ayuda a razonar sobre costos y tiempos de desarrollo**  
   - Según la arquitectura, se pueden estimar costos y plazos con más precisión.  
   - Requiere la colaboración del arquitecto, project managers y desarrolladores.

9. **Promueve la reutilización a través de modelos transferibles**  
   - Una buena arquitectura puede ser la base para desarrollar múltiples sistemas similares.

10. **Se enfoca en ensamblar componentes, no solo crearlos**  
    - Los componentes pueden desarrollarse de manera independiente, respetando las restricciones de la arquitectura.

11. **Reduce la complejidad del diseño y del sistema**  
    - Al imponer restricciones claras, se simplifica el diseño general.

12. **Sirve como base para la incorporación de nuevos miembros al equipo**  
    - Como la arquitectura mejora la comunicación, los nuevos integrantes pueden entenderla rápidamente.
