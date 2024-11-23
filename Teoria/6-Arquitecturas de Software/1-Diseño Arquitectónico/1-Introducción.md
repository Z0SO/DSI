Es un esquema general que va a tener el futuro sistema.
![[Pasted image 20241123001221.png]]

# Arquitectura

## Concepto
La **arquitectura** es un esquema general del futuro sistema, que es abstracto y está compuesto por elementos y relaciones.  
Todos los sistemas modernos presentan algún tipo de arquitectura. Sin embargo, la arquitectura no lo es todo: **todo el ciclo de vida del sistema** determina su calidad.

---

## Arquitectura de Software

### ¿Por qué se necesita definir la Arquitectura de Software?
1. **Potencia los atributos de calidad**:  
   Se enfoca en la **parte no funcional** del sistema, como:
   - Seguridad
   - Performance
   - Modificabilidad
   - Usabilidad
   - Reusabilidad  

   Por ejemplo, si el sistema debe ser **seguro**, los elementos deben diseñarse para resguardar el acceso a la información.

2. **Permite razonar y gestionar el cambio**:  
   La modificabilidad se puede clasificar en tres niveles:
   - **Local**: Afecta solo un elemento.
   - **No local**: Involucra múltiples elementos.
   - **A nivel arquitectura**: Requiere cambiar todo el sistema.

3. **Mejora la comunicación entre las partes interesadas** (*Stakeholders*):  
   La arquitectura, al ser abstracta, puede ser entendida por cualquier interesado (clientes, managers, etc.).  
   Un arquitecto puede determinar la arquitectura escuchando los reclamos y necesidades de todas las partes.

4. **Contiene decisiones de diseño tempranas y difíciles de cambiar**:  
   - **Analogía**: Después de construir una casa, no se puede cambiar la base sin derribar todo.

5. **Define restricciones para la implementación**:  
   El arquitecto asigna recursos y define atributos de calidad. Siempre que las partes cumplan con las restricciones, el sistema respetará la arquitectura.

6. **Influye en la estructura organizacional o viceversa**:  
   - La arquitectura divide responsabilidades entre los grupos de trabajo.  
   - La experiencia de los equipos también puede influir en la decisión de arquitectura.

7. **Proporciona una base para el desarrollo incremental**:  
   - Una vez definida la arquitectura, se puede construir un **sistema esqueleto** para iterar e incrementar.

8. **Permite razonar sobre costos y tiempos**:  
   - La arquitectura influye en el costo y calendario de los proyectos.

9. **Puede ser un modelo transferible y reutilizable**:  
   - Las arquitecturas pueden ser reutilizadas para desarrollar múltiples sistemas.

10. **Enfoca la atención en el ensamblaje de componentes**:  
    - Los componentes pueden desarrollarse de manera independiente mientras cumplan con las restricciones arquitectónicas.

11. **Reduce la complejidad y canaliza la creatividad**:  
    - Aplicar restricciones según el patrón arquitectónico simplifica el diseño y el desarrollo.

12. **Es la base para formar nuevos miembros del equipo**:  
    - Al ser comprensible, facilita la integración de nuevos integrantes.

---

### ¿Qué es la Arquitectura de Software?
La arquitectura es el **conjunto de estructuras necesarias para razonar sobre el sistema**. Estas estructuras comprenden:
- Los elementos de software.
- Las relaciones entre ellos.
- Las propiedades de ambos.

#### Puntos clave:
- La **arquitectura** es un subconjunto de modelos.
- Una **estructura** es un conjunto de elementos relacionados.
- Una **vista** es la representación de una estructura.
- Un software está compuesto por muchas estructuras, pero **ninguna por sí sola es la arquitectura**.
- Todo software tiene una arquitectura detrás, aunque esta sea abstracta.
- Los elementos arquitectónicos no tienen una definición rígida, sino que se describen según sus relaciones y comportamientos.

# Categorías de estructuras (vistas)

## 1ra Vista: Estructura de Componentes y Conectores
- Similar a los **nodos de UML**.
- Se centra en cómo los elementos **interactúan entre sí en tiempo de ejecución** para realizar las funciones del sistema.

### Componentes
- Son las **unidades principales de cálculo** que representan el comportamiento en tiempo de ejecución.  
  **Ejemplos**:
  - Servicios
  - Peers
  - Clientes
  - Servidores
- **Es algo físico**, como un componente compilado.

### Conectores
- En UML se representan como **mensajes**.
- Son los **vehículos de comunicación** entre componentes.  
  **Ejemplos**:
  - Devolución de llamadas
  - Operadores de sincronización de personal

### Patrones destacados
- **Publish-Subscribe (Publicador-Subscriptor)**: Patrón de comunicación donde los emisores envían mensajes a los subscriptores interesados.  
- **Client-Server request/reply con failover automático**:  
  - Esquema cliente-servidor donde, ante un fallo, el sistema principal se cambia automáticamente por un sistema de respaldo.

**Nota**: Aquí puedes incluir una imagen.  
`<inserta tu imagen en Obsidian>`  

---

## 2da Vista: Estructura de Módulos
- Equiparable a la **vista de paquetes en UML**.
- Muestra cómo se estructura un sistema como un conjunto de **unidades de código o datos** que deben construirse o adquirirse.

### Elementos
- **Módulos**: Unidades con funcionalidades específicas asignadas.
- **Enfoque**: No se toma en cuenta el tiempo de ejecución.

### Representación
- **Izquierda**: Estructura general.  
- **Derecha**: Estructura de capas (*layer*).  
  - **Dirección de las flechas**: Indica el acceso o uso entre las capas.  
  - **Capa en blanco**: Corresponde al nivel de usuario.  
  - **Capa en gris**: Pertenece al núcleo del sistema.

**Nota**: Aquí puedes incluir otra imagen.  
`<inserta tu imagen en Obsidian>`  

---

## 3ra Vista: Estructuras de Asignación
- Equiparable a la **vista de despliegue en UML**.
- Establece la asignación de las estructuras de software a elementos no relacionados con el software, como:
  - Organización
  - Entornos de desarrollo
  - Pruebas
  - Ejecución  

**Nota**: Aquí también puedes incluir una imagen.  
`<inserta tu imagen en Obsidian>`  

---

## Módulos
- Los módulos se aplican a la vista seleccionada según el **atributo de calidad** que se desee conseguir.

**Nota**: Aquí puedes incluir una última imagen.  
`<inserta tu imagen en Obsidian>`  
