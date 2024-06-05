

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXdU4alUOgzHgW55oz_qeVwAC16agsg2hDtTopdABcsBqIV_M1bN8-FxEpk9e44RGWM8QLIyBZRpZO0uaeLlFTR6xe0V1LovFIrEHS0b9fy4loeiUR0BscFyJ7_LnFgg7uwZiqcvXSzeVVEqw-dqfUFpTvUH?key=VReuh94fGGpJZLGsXsGdUQ)

# Concepto de Mensaje

Los mensajes son el mecanismo por el cual se comunican los objetos para poder interactuar y colaborar unos con otros. 

> **El mensaje es un método.** (Remarcado por el profesor)

## Tipos de Mensajes

### Sincrónicos
- El emisor se queda esperando la respuesta del receptor hasta que se produzca la respuesta.
- Son los mensajes más comunes.

### Asincrónicos
- Cuando enviamos el mensaje, el hilo no se queda esperando la respuesta, sino que esa respuesta llegará en algún momento y se realizará algo con ella.

### De Tiempo Límite
- Mezcla de los anteriores.
- Inicialmente, se comportan de manera sincrónica, pero si pasa un tiempo límite (`time-up`) sin respuesta, el objeto emisor puede continuar su procesamiento (parte asincrónica).
- Si no se recibe una respuesta dentro de ese tiempo, se genera un error.

## Ejemplos de Mensajes

- **Getters:** Obtener el valor de un atributo de un objeto.
- **Setters:** Asignar un valor a un atributo de un objeto.
- **Custom:** Para realizar operaciones más complejas entre objetos.
