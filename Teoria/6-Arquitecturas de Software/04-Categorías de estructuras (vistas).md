# Categorías de Estructuras (Vistas)

## 1. Vista: **Estructura de Componentes y Conectores**  
- **Parecida a los nodos de UML**.  
- Se centra en cómo los elementos interactúan en tiempo de ejecución para realizar las funciones del sistema.  

### **Elementos principales**  
1. **Componentes**:  
   - Unidades principales de cálculo en tiempo de ejecución (ejemplo: servicios, clientes, servidores, etc.).  
   - **Ejemplo**: Algo físico, como un binario compilado.  

2. **Conectores**:  
   - Vehículos de comunicación entre componentes (mensajes, callbacks, sincronización, etc.).  
   - Ejemplo de patrones:  
     - **Publish-Subscribe**: Publicador-Suscriptor.  
     - **Client-Server con failover automático**: Un esquema donde hay un sistema principal y un respaldo en caso de fallos.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeQYQH9Mm6h7W1boZQRn8r33EkudxnNdyD3utKzXCYzwsfZwMwNaXQHar7OUmUTqitWGVi9FbQBkwNWMnjoJ-n_2Q32pUINXowlwgNjSrHlvlOeb0Ksyb3SEkNCtm7QDMJy0HsMut4nR70t_UweOoP48Ntg?key=VReuh94fGGpJZLGsXsGdUQ)

---

## 2. Vista: **Estructuras de Módulos**  
- **Equivalente a la vista de paquetes en UML.**  
- Muestra cómo el sistema se organiza en unidades de código o datos específicas (módulos).  

### **Características**  
- Cada **módulo** tiene asignada una funcionalidad específica.  
- No se enfoca en el comportamiento en tiempo de ejecución.  

### Ejemplo:  
- **Izquierda**: Representación de módulos.  
- **Derecha**: Estructura en capas (layers).  
  - Flechas: Indican acceso o uso.  
  - **Blanco**: Capa a nivel de usuario.  
  - **Gris**: Capa a nivel de núcleo del sistema.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdCSdbyqTL7OWW6Zbh5nBFDeRg38flP0HuojTp4pNd7D6Gk50l3jOuRNnIM5GC7n28UEeIs1AT8bwifrMCdKjrKxC_uYCzof9B4c2Z976aIdSK99I0Jc2ui_rYH4vmzXZPDEACVNPXRpAHrALouvySi0WB1?key=VReuh94fGGpJZLGsXsGdUQ)

---

## 3. Vista: **Estructuras de Asignación**  
- **Equivalente a la vista de despliegue en UML.**  
- Relaciona las estructuras de software con elementos no relacionados al software (ejemplo: entornos de desarrollo, pruebas o ejecución).  

### Ejemplo:
- Asignación de módulos y componentes según atributos de calidad deseados.

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcVOvapcWTLfFxsHSnxIIEt2BKkcMMdSHgIXicgyZI8olEIT5JChfV7gYWQNNbc3sUqiuZNQHfMc3bWilF0bCgL_JRn6ia6R30JpxfK1NW49KVqVR3tfwX4Cqqg9FPeXv9jM1kXxODUTkDJXOXC37lbupm4?key=VReuh94fGGpJZLGsXsGdUQ)

---

### **Módulos y calidad**  
- Los módulos se ajustan a los atributos de calidad que se deseen cumplir (ejemplo: rendimiento, seguridad, etc.).

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdOTdA4hU4tbPQFGnBlSCkxIrilFq-L1SoOFy6leNlETbXZmegtSP7TL1PecOCPl1A_Ei0jhgg9LIHtDky1wvpG3p1sLC4PwflmET8Z6k-azx4LYsm3FCpX-B0EigO7RNLYvzrEkDITfdRqbMrNsJhhhkb_?key=VReuh94fGGpJZLGsXsGdUQ)
