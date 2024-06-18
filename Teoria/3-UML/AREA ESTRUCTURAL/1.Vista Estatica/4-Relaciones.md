# Definicion

Básicamente, es lo que une a los clasificadores.

| Relación       | Función                                                                                                                                   | Notación                                                                                                                                                                                                                                    |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Asociación     | Una descripción de una conexión entre instancias de clases.                                                                               | ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXd8_WpM9XqnxG6zYJIb2RftBNeHB-EFmZUj9PgaaFytKwaggieAnOwB3RkE1HY576tetO0Z3GBN_FyFY_frz7-3bOoWFWQu8Qma7qT7_Wi1xG-3gkip9Btl1vRDfVCU6ln0POi01maqDbeNF5s8Qf2qt1M?key=VReuh94fGGpJZLGsXsGdUQ)  |
| Generalización | Una relación entre una descripción más específica y una más general, utilizada para la herencia y para declaraciones de tipo polimórfico. | ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXemxBTEEJbq1D7zjEzCCLxI_id_H_ZVeVinyUIbfMqMV3ez0FeieucMYtmgqMYzPI1_lNCMgoI7JD-3GInoFDmjnT7UValdA3vHs18DW2DJibpyvuubg9ypI58kfD6bEbg0uAy3XfSokTbqTdp3tcOrZpM?key=VReuh94fGGpJZLGsXsGdUQ)  |
| Dependencia    | Una relación entre dos elementos del modelo.                                                                                              | ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXf3R67BO7xhV2am9R0ODphVMRdOHBnWHTtj7F5HpdQE7LwgeameD_mQVpfbm0gP2TehXTno4uxOOYK83x60atlTaz9TvPxX5mx3U3PfTJqfaRZhdnYZc10Qa1QdvvNG0kbDqZZVzA2l3MApmLfUJMhn-GD7?key=VReuh94fGGpJZLGsXsGdUQ) |
| Realización    | Relación entre una especificación y su implementación.                                                                                    | ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfmpe3Qh6mwswERiNrA7EpoLn-hQjr7-CTnc7X5g04I_KcdZg0r_nXv0gRKr9T33hiMeyK-t4jgOrIcmEuSoHdiRqCrvVN4vF3goQ6gLdlF6wR_d2V77vNJ6vpRvRBgM-kVp4PAjT-RbjDqdkUotdMytRfO?key=VReuh94fGGpJZLGsXsGdUQ) |
| Uso            | Una situación en la cual un elemento necesita de otro para su correcto funcionamiento.                                                    | ![](https://lh7-us.googleusercontent.com/docsz/AD_4nXebCtezQpNo-87Igx8D6T1-cNEhhONyN4gFcsg8UkRiJzHlZ44QIl0E8WDhQnjvvLD266vSn738S5H6l7mw2VMjUwP6AeNeP_btaE30imwfeb7LTQ66zLF1KtT5Yi_Bw3oUg9dTYlypQO6Er6D8mqO9ZEU?key=VReuh94fGGpJZLGsXsGdUQ)  |

----

## Descripción de las Relaciones

![[Pasted image 20240616212722.png]]
### Asociación
- **Función:** Una asociación es una descripción de una **conexión entre instancias de clases**. Puede representar una **relación entre dos o más objetos**, indicando que se comunican o colaboran entre sí.
- **Notación:** Representada por una línea sólida entre dos clasificadores.

### Generalización
- **Función:** Una generalización es una **relación** entre **una descripción más específica** y **una más general**. Se utiliza para herencia y para declaraciones de tipo polimórfico, donde **una clase hija hereda atributos y comportamientos de una clase padre.**
- **Notación:** Representada por una línea sólida con un triángulo blanco en el extremo que apunta hacia la clase general (padre).

### Dependencia
- **Función:** Una dependencia es una relación entre dos elementos del modelo. Indica que un cambio en el elemento independiente (proveedor) puede afectar al elemento dependiente (cliente).
- **Notación:** Representada por una línea discontinua con una flecha abierta apuntando hacia el proveedor.

### Realización
- **Función:** Una realización es **una relación entre una especificación y su implementación**. Se utiliza para mostrar que un componente realiza el comportamiento especificado por una interfaz.
- **Notación:** Representada por una línea discontinua con un triángulo sólido en el extremo que apunta hacia la especificación.

![[Pasted image 20240616210119.png]]
### Uso
- **Función:** Una relación de uso indica que un elemento necesita de otro para su correcto funcionamiento. Es un tipo especial de dependencia.
- **Notación:** Similar a la dependencia, representada por una línea discontinua con una flecha abierta.
