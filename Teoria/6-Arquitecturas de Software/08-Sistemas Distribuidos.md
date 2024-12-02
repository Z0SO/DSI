
## Sistemas Distribuidos (CONCEPTO)

Un **sistema distribuido** es un conjunto de computadoras independientes que funcionan juntas y se presentan como un único sistema ante el usuario.  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXcWz93LGfYyNKyE8t7TXIv82fXFcff_IPDLD1tb209MASrB6ywwlVLHJufyOorAExwV75uWELCjeHwgi1PtNa9zYN45Wo6kBq7wrr_sg47rNcriYn5WZTCuGt3y64cInxGq4l_Pxwq-hYZHR720lIqhuYhe?key=VReuh94fGGpJZLGsXsGdUQ)

La idea es dividir el sistema en varios nodos o computadoras para resolver problemas como la sobrecarga de un solo sistema o la falla de equipos. El usuario no debe notar que los componentes están separados; solo debe ver un sistema único.

### Ventajas de los Sistemas Distribuidos:

- **Recursos compartidos**: Ayudan a reducir costos, aunque a medida que el sistema crece, también hay que considerar la seguridad.

- **Transparencia**: Consiste en ocultar que los recursos y procesos están distribuidos en diferentes computadoras.  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeVCKmHjzUyJmhfzfbXFEFVtB9ZCw_JK3QXHMwGRIqeZ0mVhFvE7hgW5mfISEDKkDJljPt6F0X_A_g-9VJEkj-TBBnfHmQKPE2z4rl45J-nOVeA_i5UktMCtlzLTJRa0hYah0D2ivKQLNRUQKrPtiDVfTU?key=VReuh94fGGpJZLGsXsGdUQ)  
Sin embargo, no siempre se puede lograr una transparencia total, y a veces no es necesario.

- **Apertura**: Los sistemas distribuidos ofrecen servicios siguiendo normas y protocolos estándar, lo que facilita la interoperabilidad entre sistemas diferentes.

- **Concurrencia**: Los procesos pueden ejecutarse de manera simultánea en distintos equipos y comunicarse entre sí.

- **Escalabilidad**: Un sistema distribuido puede crecer de varias maneras:
    - **Escalabilidad por tamaño**: Se pueden agregar fácilmente más usuarios y recursos.
    - **Escalabilidad geográfica**: Los usuarios y recursos pueden estar ubicados a grandes distancias.
    - **Escalabilidad administrativa**: Se mantiene fácil de gestionar aunque abarque múltiples organizaciones.

Aunque la escalabilidad es una ventaja, a medida que el sistema crece, el rendimiento puede disminuir, especialmente si se manejan muchos datos.

- **Tolerancia a fallos**: Los sistemas distribuidos pueden seguir funcionando incluso si un equipo falla, gracias a la redundancia y la réplica de datos.

### Desventajas de los Sistemas Distribuidos:

- **Complejidad**: Es difícil entender y probar cómo funcionan todos los componentes, especialmente cuando dependen de diferentes factores, como el procesador o la red.

- **Seguridad**: Existen riesgos relacionados con el acceso a través de computadoras diferentes, el espionaje de datos y ataques, como los de denegación de servicio.

- **Manejabilidad**: Es complicado mantener un sistema distribuido porque pueden haber diferentes tipos de computadoras y versiones del sistema operativo. Los fallos en un componente pueden afectar a otros.

- **Imprevisibilidad**: La respuesta del sistema depende de varios factores, como la carga global, la organización y la red. Esto puede hacer que sea difícil prever el comportamiento del sistema.