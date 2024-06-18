
# Tipos de Relaciones en Casos de Uso

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdFfHJBrFS2vraOd7F_CtPCYb1w67Pi4uPAAIJRJI3u308Z1roiyQ4JBUwnVv_iGP0x1RxMVgHCR2m-F_gjrVXyuRC9fGfXL3dOQLB_1AxvxHMAAPsFc9LIclqxoA3fujVvLRVS3JpWipKSEQFnlHbdd7sB?key=VReuh94fGGpJZLGsXsGdUQ)

## Relación de Inclusión
Un caso de uso puede incorporar el comportamiento de otros casos de uso como fragmentos de su propio comportamiento. Esto se denomina **relación de inclusión**.

- **Ejemplo**: Si tenemos un caso de uso "Realizar Compra" y otro "Procesar Pago", "Realizar Compra" puede incluir "Procesar Pago" para completar su funcionalidad.

## Relación de Extensión
Un caso de uso también puede ser definido como una extensión incremental de un caso de uso base. Esto se denomina **relación de extensión**.

- **Ejemplo**: El caso de uso "Realizar Compra" podría tener una extensión "Aplicar Descuento", que se ejecuta solo en ciertas condiciones.



----

## ¿Extend o Camino Alternativo?

- **Extend**: Se utiliza cuando es opcional y suele involucrar caminos largos.
- **Camino Alternativo**: Puede reemplazarse con un camino alternativo, a menos que el caso de uso sea muy complejo o estemos intentando separar funcionalidades que correspondan a diferentes versiones del producto.

- **Ejemplo de Extensión**: Si el proceso de compra incluye la opción de agregar un seguro adicional, esto se puede modelar como una extensión para mantener la claridad y modularidad del diagrama.

- **Ejemplo de Camino Alternativo**: Si hay una verificación de tarjeta de crédito fallida, en lugar de modelar esto como una extensión, podría ser un camino alternativo dentro del caso de uso "Procesar Pago".

Usar estas relaciones de manera adecuada ayuda a mantener los diagramas de casos de uso claros, modulares y fáciles de entender.
