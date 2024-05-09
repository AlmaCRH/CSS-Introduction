# CSS-Introduction

## Reboot Cats
Aquí una pequeña página web donde se explica el temario con gatos para que la clase sea más amena

## Classes VS IDs

Las clases se pueden repetir entre elementos
Las IDs son únicas entre elementos

## Specifity
La prioridad de estilos será:
1. Style attribute
2. Ids
3. Clases y pseudo-clases
4. Elements

Si hay dos selectores que tienen la misma prioridad, solo se aplicará el último escrito.
Siempre es mejor usar las IDs para aumentar la prioridad (specifity)
Una clase opacará a todos los selectores de elementos

## Display
### Inline
1. Permite a los elementos posicionarse uno al lado de otro
2. Solo ocupa el width que necesita
3. No mantiene el "boxness"
4. No formatea los elementos como block

### inline-block
1. Se posiciona como un elemento inline
2. Se comporta como un elemento en bloque
3. Convierte al elemento en un un elemento block box
4. Ocupa todo el ancho que pueda
5. Pero dejar situarse otros elementos a su lado

## Display none
Hace que el objeto desaparezca de la página

## Box model
### Margin
1. El margin es invisible, no tiene background-color
2. Añade espacio alrededor del borde del elemento

### Border
1. Es el borde del elemento
2. Tiene background-color

### Paddding
2. Es el espacio entre el borde y el contenido

## Position
### Static
1. No se ve afectado por las propiedades top, bottom, left y right
2. Sigue el flujo normal de la página

### Relative
1. Un elemento relativo te da control sobre todos sus elementos hijos con posición absoluta
2. Los elementos relativos se ven afectados por las propiedades top, bottom, left y right

### Absolute
1. Declarar un elemento con posición absoluta dentro de otro elemento con posición relativa, nos permite mover el elemento absoluto en base a la posición del elemento relativo como referencia.
2. Si el elemento padre no es relativo el elemento con posición absoluta tomará como referencia la posición del documento body.

### Fixed
1. Cuando scrolleas en la página se quedará en la misma posición, sin seguir el scroll.

### Sticky
1. Un elemento sticky es absoluto a la página, si scrolleas  se moverá con esta pero manteniendo su posición fijada con las propiedades top, bottom, right o left


## Float & Clears
### Float
1. Cuando estilamos con float podemos posicionar el elemtno a la derecha o izquierda y dejar que los textos lo envuelvan.
2. Estos elementos se ven eliminados del flujo normal de la página pero siguen estando en él de cierta manera

Hay 3 posibilidades:
Right o Left, para posicionar a los elementos en dichas posiciones
none, nos aseguramos que el elemento no haga float
inherit, tomará el float de su padre

### Clear
1. Clear define que elemento no estan permitidos a hacer float en dicha posición, también previene el re-flowing
2. Aplica tanto a los elementos con float como a los que no
