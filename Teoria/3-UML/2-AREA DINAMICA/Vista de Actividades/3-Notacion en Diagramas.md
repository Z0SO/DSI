
# Notación en Diagramas

## Elementos del Diagrama

- **Caja Redondeada**: Representa un nodo de actividad.
- **Flechas**: Indican el flujo de control.
- **Rombos**: Utilizados para condiciones de guarda en bifurcaciones.
- **Barras Gruesas**: Representan divisiones o uniones de control.
- **Particiones (Swimlanes)**: Agrupan actividades según su responsabilidad en regiones separadas por líneas.

## Relación con Otras Vistas

Los diagramas de actividad muestran el flujo de actividades pero no los objetos que las realizan. Para completar un diseño, cada actividad debe implementarse como una o más operaciones asignadas a una clase específica, resultando en el diseño de una colaboración que implementa el grafo de actividad.

### Calles y Flujo de Objetos

Es útil organizar las actividades de un modelo según su responsabilidad, agrupando todas las actividades manejadas por una organización de negocio. Esta asignación se muestra organizando las actividades en regiones (particiones) separadas por líneas en el diagrama, conocidas a veces como calles.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXehLPilBNohHj9fZGtP7w8AM8yGKLCbe-Y2-0w_P2Fe1FrgTZE6MZ6T8wg72SZeBbdgGVG1kTxxq_6lkwMZEMoFnmZmwQU2_smV8O-GVSHcOBfBM-vE0BzOv4CwmoRS2rXiiiNIQyhzrTan31cS5vKYeTBi?key=VReuh94fGGpJZLGsXsGdUQ)
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfayz4GpZjvevUEqgSPXdJ0-kepS_CoxRGik1nnyq3ULIGmjkqQX_tOJGWihs92qNadBjjOLPS-Km8qrnRd14Suig1Z7Fs9NwVtdIWCdaPN0G0_oVLaurzDp2owRCdnUQ_UefRdR02FYu4ZD0ZXeWxDp1IY?key=VReuh94fGGpJZLGsXsGdUQ)
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcW-cXVAD9eHSYSgo6bjyvmNJJddm_6l_pDXKku8Q0AGWShfVNB77I1H5e9kHavyozWDOSxZP-ugHecbJn2Bfb3G_gxX2TWQMRtcmhcH-sjanq9AXZ4c65XlS-l-jsTYAFTAmZQr_cKJ57Z5zLxTRKhXvKl?key=VReuh94fGGpJZLGsXsGdUQ)

#### Flujos de Objetos

Representa un objeto que es la entrada o salida de una actividad. Las flechas indican la dirección del flujo del objeto.
