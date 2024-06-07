

# Definicion

## Asociación

- **Asociación:** Conexión semántica entre instancias de clases.
  - **Diferencia con otras relaciones:** Da sentido a la conexión entre objetos de esas clases.
  - **Relación estructural:** Entre instancias.
  - **Proporciona conexión:** Entre objetos para el envío de mensajes.
  - **Típicamente binaria:** Es el pegamento que mantiene unido el sistema.

### Enlace

- Una instancia de una asociación es un enlace.
- Un enlace es una asociación entre dos objetos.
- Un enlace consta de una tupla (una lista ordenada) de objetos, cada uno obtenido a partir de su clase correspondiente.
- Un enlace binario comprende un par de objetos.

### Adornos

Adornos son todos los elementos adicionales que se pueden poner en el diagrama. Estos mecanismos incluyen:

- **Nombre**
- **Rol**
- **Multiplicidad**
- **Agregación/Composición**

#### Nombre

- Puede tener un nombre en cada dirección (llamado extremos de la asociación).
- No son obligatorios.
- Puede omitirse en caso de tener nombres de rol.
- Es conveniente poner nombres diferentes a cada relación.
- Se marca con un triangulito la dirección.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXf7FrkwSpYywK1UyTIUTxqi2pWe8T0ecaJu1SEv5FqTpTEsR_ZK8q6nbr0Ekf9irGAb1iF70FQwZTGLlC8n8Ft_M5g4klT-rl8F7EjrieeyYA5ECynX4EgN9hFX97DPZDvd-ii7vxPGPZV5Woa-ouN9dNI?key=VReuh94fGGpJZLGsXsGdUQ)


#### Rol

- Es el papel interpretado por una clase en una asociación.
- Nombre del extremo (rol) -> A los extremos se le agrega el rol.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeC6Bu4VUQXgQZRq5kyxTuMID_lJa-H41L_SJxrHHIVhWzLrANS8doARkcRvucx7Hv2SRSIdmInDpA1VPCBaodhQkvHFuPdWDV16v1We6C7XjAZ4ES29uyLwczTfAvwqs6TFjF2eD6Gp6aNAPyPeFhObFs?key=VReuh94fGGpJZLGsXsGdUQ)


#### Multiplicidades - Cardinalidades

- **Especificación (min ... max):**
  - `1`   → uno y solo uno.
  - `0..2` → cero o uno.
  - `M..N` → de M a N (enteros naturales).
  - `*`   → cero o muchos.
  - `0..*` → cero o muchos.
  - `1..*` → uno o muchos (al menos uno).
- **Multiplicidad mínima:** >=1 establece una restricción de existencia.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXebc59tzCdLGFtqPEaU5B6ZQI64P4hGxmkehr7aYrdgDvByWeEEx85agM_60P0RnLElT1YT_-Z15Qtjuv_mKPdb01Ygzjwjj8J2N7NVQluwLAdhbETV1qXWI6Oc78I7oEZ3ISXGCLVkFq2WAK4rz-F7iznr?key=VReuh94fGGpJZLGsXsGdUQ)


### Agregación y Composición

- Representa una relación todo-partes entre objetos.
- Variante de la asociación, con mayor fuerza semántica.

#### Agregación (o Agregación Compartida)

- Pertenencia débil de las partes con el todo.
- Una parte puede pertenecer a varios todos.
- No hay exclusividad.

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXeOVsymNYKH_Yb6ao-oYAIIn_9zcRFR9e_jXxwD8c22VOtKthRsdwb8PdIJ84LxZfzrApXoAX-Jb6O_2K816zsmEHQL0oFQyL2MbTnvxYNwnvBxTiYYVxmqGvWqkgcHO39s8gT4uHTKOqONBdEYeGFLIe2r?key=VReuh94fGGpJZLGsXsGdUQ)

#### Composición

- Forma de asociación más fuerte en el cual el compuesto es responsable de gestionar sus partes. Ej: asignación y desasignación.
- Implica:
  - **Dependencia existencial:** Si elimino el todo la parte desaparece.
  - **Pertenencia fuerte:** Todo y parte están fuertemente unidos.
  - **No compartición de objetos:** Los objetos contenidos no son compartidos (se pueden reutilizar las clases, los objetos no se comparten).


![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfgkdPqRMkdF7VFaKdic2ojwFBc-7HyfbZ6lSHhBZiS9urw8C_No6DkYIyA6SLAodt09LStqJpIhOzBEAdOBSlFLSG1_bvjoNYJhPWHEDMd_VXeUEtS8f2wAcG1xIuWu6qifpz6OKUMLNXTTB6urqcHoON_?key=VReuh94fGGpJZLGsXsGdUQ)