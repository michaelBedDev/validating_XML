Un elemento es tiene un tipo simple si no contiene otros elementos o atributos dentro, sino es complejo
Un elemento está vacío si no tieme otros elementos entro. Puede tener un tipo complejo

Todos los elementos tienen un nombre y un tipo

Elemento mixto: tiene elementos y texto dentro. (o atributos? otros elementos y atributos?) 
element -> type -> mixed:"true"

Listas y enumerados van dentro de un elemento con un tipo simple.

element -> simpleType -> list     LAS LISTAS PUEDEN TENER TYPE (y union)
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


Los elementos de las secuencias tienen que aparecer en orden

Fixed value: 
atribute (dentro) fixed=""
Fechas: 2023-03-02


Revisar simplecontent text only
Revisar empty elements

XSD

Elementos y atributos
Tipos: xs:gYear, xs:date, positiveInteger, etc

Generar tipos. Simples y complejos

Mixed con atributo
element -> tipo ->simpleContent ->extension base (texto)->atributo (tipo atributo)
Mixed con elemento
element -> complexType mixed="true"-> element 
