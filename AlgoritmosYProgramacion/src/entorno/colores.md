# Colores
Los dibujos que hicimos hasta ahora son monocromáticos. P5 nos provee de instrucciones para poder pintar tanto el fondo del lienzo como cada forma que programemos.

P5 tiene una gama de 256 colores para tanto la escala de grises como para cada color primario. Los colores primarios que se usan son el rojo, el verde y el azul (los colores primarios de la luz).

Las funciones para pintar en processing son:
```js
background
```
Que nos permite pintar el fondo del dibujo, es decir que colorea el lienzo
```js
fill
```
Que sirve para pintar todas las figuras que dibujemos después de esta instrucción
```js
stroke
```
Pinta el contorno de las figuras.

## De qué color?

Todas estas instrucciones reciben 1 o 3 parámetros. Si la usamos con un sólo parámetro, se asume que se esta coloreando en escala de grises.

![color_gris](../images/grises.png)

```js
background(120)
```
_Pintaría el fondo de un color gris oscuro_

Cuando usamos 3 parámetros, se pinta en colores usando el primer número como el valor de rojo, el segundo como el valor de verde y el último como el valor de azul.

![color_rgb](../images/rgb.png)

```js
fill(240,240,60)
```
Pintaría las figuras de un color similar a un amarillo.

Combinando los tres valores, podemos generar 65 millones de variaciones de colores diferentes.
<!-- TODO: buscar si puedo hacer una tabla con colores hex -->
