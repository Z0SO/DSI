
### Dependencias

#### Definición
Una **dependencia** es una relación entre dos elementos en un sistema, donde uno es el cliente y el otro es el proveedor. Los cambios en el proveedor pueden afectar al cliente. Las dependencias pueden tener estereotipos para indicar el tipo específico de relación.

### Tipos de Dependencias
- Aqui **Creacion es el mas importante**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeemsBONSU9h8stwZ4TFP4b0OFdJXNkgRYOceJzhqQrfwdlyIqf6UYEL4MyI0FkKucYnwvzg7hcyPh-xV39fqPSaF-5U1dSLXRgZKuujhenxUnQ86jEf66RV0DrEwS0m0t4L7L4ZTGomLnPkzU6iAzSTNdc?key=VReuh94fGGpJZLGsXsGdUQ)

#### Representación en UML

- **Dependencias de Uso**: Indican que una **clase necesita algo de otra clase,** como utilizar un método o acceder a una propiedad. Se representan con una línea discontinua y una flecha abierta.
- **Dependencias de Abstracciones**: Relacionan una **clase con una interfaz** o un componente abstracto. Se representan con una línea discontinua y una flecha cerrada.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdeaIaO33C4GyL8FcaUIbjvrewnSZSEnVQeZXJJ-KFGK3ghOst-h5Pgr9uf7HvsuQk2O7eW2Nk84_EF6wbwmtOHvlRwQy7uNvVrB3sR8ptiobxmg5KVFvEOEf6RnYeDnEM21LYdAVFieM2h9uMOgpPNTEkP?key=VReuh94fGGpJZLGsXsGdUQ)


#### Comparación entre Dependencias y Asociaciones
 **Dependencias**:
  - Relación **temporal** y **circunstancial**.
  - Los cambios en el proveedor pueden afectar al cliente.
  - No implica una **referencia continua** entre los objetos.
  - Se activa en situaciones específicas, como pasar un objeto como parámetro o crear un objeto temporalmente.

**Asociaciones**:
  - Relación permanente y siempre activa.
  - Implica una referencia constante y continua entre los objetos.
  - Ejemplo: una clase Pedido tiene una asociación con una clase Cliente, donde cada Pedido tiene un Cliente asociado en todo momento.

#### Dependencia de Interfaz
Opcionalmente, se pueden mostrar símbolos de Bola y Zócalo (Ball & Socket) o Lollipop para indicar las interfaces proporcionadas y requeridas por una parte, utilizando la notación estándar para la definición de tipos de parte.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdm1ROtRgFNgT6q-OV3xFmw9kLsFF8rtCMaCjfnzkqczpnJEFUNN3_ZauGvKIxr0wUkuAblpnfXu3N_ARvXkfZtEShWIC-AT7P3To48YtxgHPVoM4YO50Ayp74HQ27s-M1NHrCgilfYaXk1oneOmpgrSU8T?key=VReuh94fGGpJZLGsXsGdUQ)


### Conclusión
Las dependencias y asociaciones son conceptos fundamentales en la modelización de sistemas orientados a objetos. Mientras que las dependencias representan relaciones temporales y circunstanciales, las asociaciones indican relaciones permanentes y continuas. La correcta representación de estas relaciones en diagramas UML es crucial para entender y comunicar la estructura y el comportamiento del sistema.