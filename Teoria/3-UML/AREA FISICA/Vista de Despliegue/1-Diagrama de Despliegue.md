

## Vista de Despliegue

- **Propósito**: Muestra la disposición física de los nodos.
- **Nodo**: Es un recurso computacional de ejecución (e.g., computadoras, dispositivos). Los nodos pueden contener artefactos (e.g., archivos).
  - **Manifestación**: Vincula componentes de diseño con los artefactos que los representan.
  - **Rendimiento**: Resalta cuellos de botella en rendimiento debido a la ubicación de los artefactos en diferentes nodos.


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXd47e6m9Cc2Qm1jbxyvcQE4hUghHaZUuzL1bEtiPNtC9VRJME-vG7pQxeMgos9ntdDUk6DAKLQkCXTU_GaLysmxZsq9iNFVwKIlkW_W-_lNp2-8wqGXubQijLXIXDFJWDUytns9iIcvj_99rsralGmMIgJ4?key=VReuh94fGGpJZLGsXsGdUQ)


### Nodo

- **Definición**: Modela un recurso computacional de tiempo de ejecución.
- **Características**:
  - Generalmente tiene menos memoria y capacidad de procesamiento.
  - Pueden tener estereotipos para distintos tipos (e.g., UCP, dispositivos, memorias).
  - Representación: cubo estilizado o cadena subrayada con nombre y tipo.
- **Asociaciones**: Entre nodos representan caminos de comunicación.
- **Relaciones**: Generalización entre nodos para descripciones generales y específicas.

### Artefacto

- **Definición**: Modela una entidad física como un archivo.
- **Representación**: Rectángulo con la palabra clave «artifact».
- **Presencia en un nodo**: Símbolo del artefacto anidado dentro del símbolo del nodo.
- **Tipos**: Artefactos marcados con estereotipos (e.g., bases de datos, páginas web, ejecutables, guiones).
- **Relación de Manifestación**: Línea discontinua con la palabra clave «manifest» del artefacto al componente implementado.

### Ejemplo de Diagrama de Despliegue

- **Nodos**:
  - `servidor:ServidorDeBanco`
  - `cliente:QuioscoDeCajeroAutomático`
- **Artefactos**:
  - `transacción.jar` en el servidor: `ServidorDeBanco`
  - `CA-IGU.jar` en el cliente: `QuioscoDeCajeroAutomático`
  - `BBDDcuenta` (una base de datos) en el servidor: `ServidorDeBanco`
- **Componentes**:
  - `Transacción`, implementado por el artefacto `transacción.jar`
- **Enlace de Comunicación**:
  - Representado por una línea que conecta el servidor y el cliente, mostrando que pueden comunicarse entre sí.
- **Dependencia**:
  - Una línea discontinua con una flecha desde `CA-IGU.jar` hacia `transacción.jar`, indicando que `CA-IGU.jar` depende de `transacción.jar`.