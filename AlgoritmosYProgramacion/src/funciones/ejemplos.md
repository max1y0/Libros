# Ejemplos

### Función lluvia con función predefinida **random**

Con la función random podemos programar una simulación de gotas de lluvia sobre el piso. Dibujando pequeños circulitos en posiciones al azar de la pantalla, y dibujando el fondo sólo una vez.

```js
var posX,posY;
function setup() {
  createCanvas(400, 400);
  background(220);
}

function draw() {
  posX = random(0,width);
  posY = random(0,height);

  fill(10,100,200,100);
  noStroke()
  ellipse(posX,posY,10,10)
}
```

### Función dado

La función dado, va a ser una función que dibuja un dado en una posición y tamaño dada por parámetros. El número que salga en la cara va a ser calculado mediante la función random. Esta función combina el uso de funciones predefinidas, funciones con parámetros, y el uso de funciones dentro de funciones (ya que cada cara del dado puede ser sus función propia.)

```js
function dibujoDadoD6(posX, posY, tamX, tamY) {
  fill(255);
  //rect(posX, posY, tamX, tamY);
  fill(0);
  let cara = floor(random(1,7)) //floor redondea el número al azar obtenido.
  if (cara == 1) {
    uno(posX, posY, tamX, tamY)
  } else if (cara == 2) {
    dos(posX, posY, tamX, tamY)
  } else if (cara == 3) {
    tres(posX, posY, tamX, tamY)
  } else if (cara == 4) {
    cuatro(posX, posY, tamX, tamY)
  } else if (cara == 5) {
    cinco(posX, posY, tamX, tamY)
  } else if (cara == 6) {
    seis(posX, posY, tamX, tamY)
  }
}
```
