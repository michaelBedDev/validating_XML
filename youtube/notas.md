Un elemento es tiene un tipo simple si no contiene otros elementos o atributos dentro, sino es complejo
Un elemento está vacío si no tieme otros elementos entro. Puede tener un tipo complejo

Todos los elementos tienen un nombre y un tipo

Elemento mixto: tiene elementos y texto dentro. 
element -> type -> mixed:"true"

Listas y enumerados van dentro de un elemento con un tipo simple.

element -> simpleType -> list
element -> simpleType -> restriction -> enum

Para que un elemento sólo pueda tener dentro otros elementos selecionados, se usa un choice
element -> choice -> element


Las restricciones llevan un elemento base.


Para aplicar una restricción de patrón, lo siguiente:
element -> tipo -> restriction -> pattern


Para usar un tipo como base de una restricción, es necesario escribirlo como tipo simple y escibirlo fuera

Puedes crear un tipo para usarlo como base en una restricción (y así restringir más)

PUEDES HACER UNA RESTRICCION TANTO DE ELEMENTOS COMO DE ATRIBUTOS


EXTENSION,SEQUENCES
