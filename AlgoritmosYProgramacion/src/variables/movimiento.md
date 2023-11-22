# Movimiento
Si agregamos la siguiente línea al código anterior:
```js
posicionX = posicionX + 1
```
Logra que el rectángulo se mueva de izquierda a derecha. Analicemos porqué.

El rectángulo tiene en su parámetro de posición en el eje X una variable llamada ```posicionX``` que originalmente está inicializada en ```20```. La instrucción, le asigna a la variable ```posicionX```, lo que tenía previamente sumada en uno, es decir, queda en ```21```. Como el bloque ``draw`` es un ciclo infinito, lo que pasa a continuación es que se vuelve a dibujar el rectángulo, pero esta vez la variable ```posicionX``` tiene un nuevo número, ```21```, entonces no se dibuja en la misma posición que antes, está corrido en un lugar a la derecha. Si esto se repite constantemente, sumando constantemente 1 a la variable ```posicionX```, la animación que se genera es la de que el cuadrado se va moviendo de forma horizontal hacia la derecha.

**¿Qué hace falta para poder realizar movimientos en otros sentidos?**