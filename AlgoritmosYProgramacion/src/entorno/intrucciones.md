# Instrucciones
Las instrucciones de p5 nos van a permitir dibujar cosas en el lienzo, indicando qué dibujar y algunos parámetros. Los parámetros son información que agregamos a una instrucción para indicar por ejemplo, tamaño, posición, color, etc.
<!-- TODO imagen -->
## rect
Para dibujar un rectángulo, necesitamos especificar cuatro datos. Las coordenadas X e Y de la esquina superior izquierda de un rectángulo. Luego necesitamos indicar el ancho y por último el alto. Es decir:
```
origen: 
    x=7
    y=4 
ancho: 9
alto: 11
```
<!-- TODO: imagen  -->

En este caso rect es la instrucción para dibujar un rectángulo y los números dentro del paréntesis son sus parámetros en el orden definido anteriormente.
```js
rect (7,4,9,11)
```
La instrucción ellipse, funciona de la misma manera, indicando cuatro parámetros que simbolizan posición y tamaño, sólo que dibuja óvalos o círculos
