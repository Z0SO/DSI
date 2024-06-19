## 👷🏻‍♀️Fabricación Pura - Pure Fabrication

This principle allows introducing new classes to fulfill specific responsibilities without violating cohesion or coupling principles. It helps maintain clear class boundaries.

### Descripción
La fabricación pura se da en las clases que no representan un ente u objeto real del dominio del problema sino que se han creado intencionalmente para disminuir el acoplamiento, aumentar la cohesión y/o potenciar la reutilización del código. La fabricación pura es la solución que surge cuando el diseñador se encuentra con una clase poco cohesiva y que no tiene otra clase en la que implementar algunos métodos.

### Características
- Se crea una clase "inventada" o que no existe en el problema como tal, pero que, añadiéndola, logra mejorar estructuralmente el sistema.
- Como contraindicación, al abusar de este patrón suelen aparecer clases función o algoritmo, esto es, clases que tienen un solo método.

### Arquitecturas de “n capas”
Las arquitecturas de “n capas” se basan en el patrón de “fabricación pura” ya que cada capa le aporta abstracción al proyecto. Su objetivo es la alta cohesión.
