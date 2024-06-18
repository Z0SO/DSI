
---

## Principio de Responsabilidad Única (SRP)

### Enunciado
"No debería haber nunca más de una razón para cambiar una clase."

### Interpretación
Una clase debería concentrarse sólo en hacer una cosa de tal forma que cuando cambie algún requisito en mayor o menor medida, dicho cambio sólo afecte a dicha clase por una razón.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeD4SAduEEhgbXjDAndj9DKSeLpjeIjcKJoR9J0LOvhoIA0MBzAIc0Hh_BNBlssl-4GgYVXnHB6ROurrcrJz3tPam0SSg0ZyN7y0ggGd0BvQIjOA_8oVLARWEGwZjFkSi4aIO8TpM8_Lph5B-nlpVdfUb0N?key=VReuh94fGGpJZLGsXsGdUQ)
### Explicación
Cuando el sistema evoluciona, aparecen nuevos requisitos. Si al cambiar el modelo hay que modificar más de una parte, es porque no se aplicó correctamente el SRP. El SRP asegura que una clase tenga una única responsabilidad, lo que facilita la mantenibilidad y extensibilidad del código.

### Ejemplo Práctico

#### Caso del Contenido de un Email
Si el contenido del email puede ser de más de un tipo, lo único que tendríamos que modificar es la interfaz de `IContenido`, cumpliendo así con el SRP.

```java
interface IContenido {
    String getContenido();
}

class TextoContenido implements IContenido {
    private String texto;

    public TextoContenido(String texto) {
        this.texto = texto;
    }

    @Override
    public String getContenido() {
        return texto;
    }
}

class HTMLContenido implements IContenido {
    private String html;

    public HTMLContenido(String html) {
        this.html = html;
    }

    @Override
    public String getContenido() {
        return html;
    }
}
```

#### Caso del Emisor del Email
Si el emisor puede ser de más de un tipo, habría que definir una interfaz de `IEmisor`. En caso de varios tipos de emisores, solo se tendría que modificar dicha interfaz.

```java
interface IEmisor {
    void enviarEmail(IContenido contenido);
}

class EmailEmisor implements IEmisor {
    @Override
    public void enviarEmail(IContenido contenido) {
        // Lógica para enviar email
    }
}

class SMSemisor implements IEmisor {
    @Override
    public void enviarEmail(IContenido contenido) {
        // Lógica para enviar SMS
    }
}
```

### Beneficios del SRP
- **Facilidad de Mantenimiento**: Al tener una sola razón para cambiar, las clases son más fáciles de entender y modificar.
- **Reusabilidad**: Las clases con responsabilidades únicas son más fáciles de reutilizar en diferentes contextos.
- **Pruebas Unitarias**: Las clases con una única responsabilidad son más fáciles de testear, ya que tienen un comportamiento bien definido.

Aplicando el SRP, se mejora la calidad del software, haciéndolo más robusto y flexible ante futuros cambios.

