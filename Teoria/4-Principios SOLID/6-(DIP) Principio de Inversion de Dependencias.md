
----
## Principio de Inversión de Dependencias (DIP)

### Enunciado
"Los módulos de alto nivel no deberían depender de módulos de bajo nivel. Ambos deberían depender de abstracciones."

### Interpretación
Para lograr robustez, flexibilidad y reutilización, es crucial que el código dependa de abstracciones en lugar de implementaciones concretas. Esto se logra utilizando interfaces y clases abstractas, y exponiendo las dependencias a través de constructores o parámetros.

### Explicación
El principio de inversión de dependencias (DIP) es uno de los principios SOLID que promueve la inversión de la dirección de las dependencias en un sistema. En lugar de que los módulos de alto nivel dependan directamente de módulos de bajo nivel, ambos deben depender de abstracciones. Esto permite que los detalles específicos de implementación se mantengan separados de los componentes de alto nivel, facilitando la modificación, la extensión y la prueba del sistema.

### Ejemplo Práctico

#### Definición de la Abstracción
Primero, definimos una interfaz `IDataRepository` que especifica un método `getData()` para obtener datos.

```typescript
// Definimos una interfaz para la obtención de datos
interface IDataRepository {
  getData(): any;
}
```

#### Implementaciones Concretas
Luego, creamos implementaciones concretas de `IDataRepository` utilizando diferentes tecnologías de almacenamiento de datos, como MongoDB y SQLite.

```typescript
// Implementación concreta del repositorio usando MongoDB
class MongoRepository implements IDataRepository {
  getData() {
    let data = MongoDB.find({});
    return data;
  }
}

// Implementación concreta del repositorio usando SQLite
class SQLiteRepository implements IDataRepository {
  getData() {
    let data = SQLite.query('SELECT * FROM data');
    return data;
  }
}
```

#### Módulo de Alto Nivel (Controlador)
El `Controller` representa un módulo de alto nivel que necesita interactuar con el repositorio de datos. En lugar de depender directamente de las implementaciones concretas (`MongoRepository` o `SQLiteRepository`), depende de la abstracción `IDataRepository`.

```typescript
// Controller depende de la abstracción IDataRepository
class Controller {
  private repository: IDataRepository;

  constructor(repository: IDataRepository) {
    this.repository = repository;
  }

  handleRequest() {
    let data = this.repository.getData();
    doSomething(data);
  }
}
```

#### Uso en el Código
Finalmente, en el código de aplicación, creamos una instancia de `MongoRepository` o `SQLiteRepository` y la pasamos al `Controller` mediante su constructor.

```typescript
// Uso en el código
let repository = new MongoRepository(); // O SQLiteRepository()
let controller = new Controller(repository);
controller.handleRequest();
```


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXe0SKgry3nDcsAYroUZ1JRQa6mq5i-ZRYna9ZpJR_EcGJ6sBOkdKM_5m0SHumvZ59J7DWn0oDGzJiVKxKUiEBVRlzKmUCL4ck6uDoF9CwsAVAxzoa0MdKyg32MTut2ATH65Jyb0H2_I6b2KFwBBWA59rBvM?key=VReuh94fGGpJZLGsXsGdUQ)


### Beneficios del DIP
- **Desacoplamiento**: Permite que los módulos de alto nivel no dependan directamente de las implementaciones concretas de bajo nivel, lo que facilita el intercambio y la prueba de componentes.
- **Flexibilidad**: Se pueden introducir nuevas implementaciones de `IDataRepository` sin modificar el `Controller` ni otros módulos de alto nivel.
- **Reutilización**: Las abstracciones facilitan la reutilización de código, ya que diferentes implementaciones pueden ser intercambiables.

Aplicando el DIP, se mejora la modularidad y la mantenibilidad del sistema, haciendo que el código sea más resistente a cambios y más fácil de mantener a largo plazo.