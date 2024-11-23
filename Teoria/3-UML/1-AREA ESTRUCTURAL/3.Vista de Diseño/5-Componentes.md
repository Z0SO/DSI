
---

# Definición

Un **Componente** es una **unidad autónoma** que **encapsula el estado y el comportamiento** de varios Clasificadores.

Especifica un contrato formal de los servicios que proporciona a sus clientes y los que requiere de otros componentes o servicios del sistema en términos de interfaces proporcionadas y requeridas.


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXcSdMC4e0fd19tbaW_JI67DeqEOA1QlIMsqUcNNpwHHBCSrfWk_-NNllPqJQKgBY_K0Nt81ygB3RHCGGPnbFbqXsV_1n8vQ_0h84OcPkC2SROpjCVB1f6V_-P3W_ucwqE4v9w9LmvVMzgt7d2dHCswaNT6T?key=VReuh94fGGpJZLGsXsGdUQ)
![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfY-YvMIQlPADsDrytDY9pf1K2172EBw5nvAdNxdGTX5QVXO-_qBY1W29fXH_NSo30z1TEx5ENMAFKN5W3pakJ_h3rSfCH4fitJ_FR2PwClwbkKEzzqQh0pxLPEobARXF18K7G9ZZfyzoU7mR44epu4y8Df?key=VReuh94fGGpJZLGsXsGdUQ)
## Características Principales

- **Encapsulación**: Un componente encapsula estado y comportamiento, ofreciendo una abstracción clara y concisa.
- **Contrato Formal**: Define los servicios que proporciona y requiere mediante interfaces.
- **Modularidad**: Representa una pieza modular de un sistema lógico o físico.
- **Desacoplamiento**: No dependen directamente de otros componentes, sino de las interfaces compatibles con los componentes.
- **Reusabilidad y Sustitución**: Son reutilizables y sustituibles, es decir, es posible reemplazar un componente con otro que cumpla con las mismas interfaces.
- **Autocontenidos**: Un componente puede funcionar de manera independiente y contiene todo lo necesario para cumplir su propósito.

## Comparación con Clases

- **Similitud**: Muy similar a una clase en términos de encapsulación de estado y comportamiento.
- **Diferencia**: Un componente es un clasificador reusable y sustituible, totalmente acoplado al contexto.

## Comunicación

- **Interfaces**: Los componentes se comunican a través de interfaces.
  - **Interfaces Provistas**: Soportan ciertas interfaces que ofrecen servicios a otros componentes.
  - **Interfaces Requeridas**: Necesitan ciertas interfaces de otros componentes para funcionar.

## Clasificador Estructurado

Un componente conforma y proporciona la realización de un conjunto de interfaces. Aunque un componente es un clasificador estructurado, se hace una distinción a *nivel* **semántico** para resaltar su reusabilidad y capacidad de sustitución.


---

### Resumen

- **Clasificador Reusable**: Un componente es un clasificador reutilizable y sustituible.
- **Modularidad y Desacoplamiento**: Los componentes son modulares y no dependen directamente de otros componentes.
- **Interfaces**: Se comunican y funcionan mediante interfaces proporcionadas y requeridas.
- **Sustitución**: Es posible reemplazar un componente con otro que cumpla con las mismas interfaces, lo que permite una mayor flexibilidad y mantenimiento del sistema.


