# Conjunto de Generalización en UML

## Definición

Es una **agrupación de subclases** que **representan diferentes aspectos** de la estructura y semántica de un concepto. Cada subclase se especializa en una **dimensión específica** del concepto padre, lo que permite una visión multidimensional de la jerarquía de clasificación. Todas las subclases en un conjunto de generalizaciones comparten el mismo padre.

Un Conjunto de Generalización es un grupo de subcategorías (subclases) que representan diferentes aspectos de una categoría principal (clase padre). Cada subcategoría se enfoca en una característica específica de la categoría principal, permitiendo ver la estructura desde varios ángulos. Todas estas subcategorías tienen el mismo origen (la misma clase padre).

![[Pasted image 20240607195345.png]]
## Características

- **Unicidad:** Cada conjunto de generalizaciones representa una dimensión única del concepto original.
- **Abstracto:** Los clasificadores dentro del conjunto son abstractos, ya que describen parcialmente al padre, resaltando una cualidad específica mientras ignoran otras.
- **Completitud:** Para crear una instancia concreta, es necesario especializar todas las dimensiones simultáneamente.

## Notación
Se representa como una etiqueta de texto a continuación de dos puntos colocada en una flecha de generalización. Ejemplo: “:situación” y “:localidad”.

### Restricciones

**Disjoint (Disjunto):** Un elemento no puede pertenecer a dos subcategorías al mismo tiempo dentro del conjunto. Ninguna instancia puede ser parte de dos subcategorías a la vez. 

**Overlapping (Solapado):** Un elemento puede pertenecer a dos o más subcategorías al mismo tiempo. Una instancia puede ser parte de varias subcategorías a la vez. 

**Complete (Completo):** Todas las subcategorías posibles están enumeradas en el conjunto y no se pueden agregar más. 

**Incomplete (Incompleto):** No se han enumerado todas las subcategorías posibles. Se espera que haya más o ya se conocen pero no se han declarado. **Por defecto:** Si no se dice nada más, se asume que el conjunto es {incomplete, disjoint} (incompleto y disjunto).

**

![](https://lh7-us.googleusercontent.com/docsz/AD_4nXfI-jXN1AZ6EydviMFDmeX118umTyT3MPSmDhIkdqfGX99s_IQxDKMoM9vmj_ivdBLqSyx9W6FULEIO2bRha1DiXjKcyQIYeo8XUoCzjE59ly-3OOaIaFwTZX6lS2OMcSvwIdI_Sn9-kkdLEgGr_PVOvNfI?key=eC-A4tU6YurBdRY8QSa-gA)
