# Ejemplos
## Mostrando las edades (código completo)
```js
let edades = [120, 40, 90, 330, 0, 20, 50, 150, 50, 90];
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);

  for (let i = 0; i < edades.length; i += 1) {
    text(edades[i], 25 * i, 20);
  }
}
```

## Gráfico de barras
Podemos usar los datos de un arreglo para que indiquen la altura de un rectángulo, generando una especie de gráfico de barras.
```js
let datos = [120, 40, 90, 330, 0, 20, 50, 150, 50, 90];
function setup() {
  createCanvas(400, 400);
}

function draw() {
  background(220);

  for (let i = 0; i < datos.length; i += 1) {
    rect(20*i,0,20, datos[i]);
  }
}
```
Este algoritmo dibuja nuestro gráfico de cabeza, no tiene colores, ni referencias de los datos, pero sirve para una base que podría transformarse en un generador de gráficos de barras.

## Lluvia con arreglos
Podemos hacer una lluvia, similar a la de la unidad de condicionales, pero en lugar de usar 3 gotitas, podemos usar un número mucho más grande, por ejemplo 400.
Podemos usar un arreglo de 400 lugares, en donde cada dato del arreglo va a guardar la posición de una gota en pantalla. Si hacemos que la posición sea un número al azar negativo (que esté por "arriba" del lienzo), tenemos gotas que caen en distintos tiempos.
En este caso es necesario definir el arreglo, e inicializarlo en el bloque ```setup()```
```js
var gotas = []

function setup() {
  createCanvas(600, 600);

  var i = 0
  for (i = 0; i < width; i++) {
    gotas[i] = random(-50, -1500)
  }
}
```
Luego, vamos a recorrer todo el arreglo, dibujar un rectángulo en la posición del arreglo gotas en i, y aumentar ese dato en una velocidad (en este caso elegí 4). Si ese número llega a pasarse del alto de nuestro canvas, lo vuelvo hacia arriba.
```js
function draw() {
  noStroke()
  fill(100,200,240,170)
  background(41)
  for (i = 0; i < width; i++) {
    rect(i, gotas[i], 2, 8)
    gotas[i] = gotas[i] + 4
    if (gotas[i] > height) {
      gotas[i] = random(-50, -500)
    }
  }
}
```
