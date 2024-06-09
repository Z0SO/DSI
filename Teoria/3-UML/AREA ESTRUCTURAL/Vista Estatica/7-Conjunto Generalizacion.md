

# Conjunto de Generalización en UML

## Definición

Es una agrupación de subclases que representan diferentes aspectos de la estructura y semántica de un concepto. Cada subclase se especializa en una dimensión específica del concepto padre, lo que permite una visión multidimensional de la jerarquía de clasificación. Todas las subclases en un conjunto de generalizaciones comparten el mismo padre.


![[Pasted image 20240607195345.png]]
## Características

- **Unicidad:** Cada conjunto de generalizaciones representa una dimensión única del concepto original.
- **Abstracto:** Los clasificadores dentro del conjunto son abstractos, ya que describen parcialmente al padre, resaltando una cualidad específica mientras ignoran otras.
- **Completitud:** Para crear una instancia concreta, es necesario especializar todas las dimensiones simultáneamente.

## Notación
Se representa como una etiqueta de texto a continuación de dos puntos colocada en una flecha de generalización. Ejemplo: “:situación” y “:localidad”.

## Restricciones

- **Disjoint (Disjunto):** Ningún elemento puede tener dos hijos en el conjunto como antecesores. Ninguna instancia puede ser una instancia directa o indirecta de dos de los hijos.
- **Overlapping (Solapado):** Un elemento puede tener dos o más hijos en el conjunto de antecesores. Una instancia puede ser una instancia de dos o más hijos.
- **Complete (Completo):** Todos los hijos posibles se han enumerado en el conjunto y no puede ser agregado ninguna más.
- **Incomplete (Incompleto):** No se ha enumerado todavía todos los hijos posibles en el conjunto. Se esperan más hijos o se conocen pero no se han declarado aún.
- **Por defecto:** {incomplete, disjoint}
