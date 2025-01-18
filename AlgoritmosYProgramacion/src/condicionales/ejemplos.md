# Ejemplos

## Lluvia
Usando como base lo que aprendimos para mover una figura, y el condicional if mostrado antes:
```js
if (posicion > 400){
    posicion = 0
}
```
Podemos hacer una simple animación de lluvia.

Primero, necesitamos dibujar una gota, y generar que se mueva hacia abajo.
```js
ellipse(100,posicion,20,50)
posicion+=1
  ```
Si analizamos el condicional escrito más arriba, estamos diciendo que si la variable ```posición``` llega a pasarse de 400, su valor se reinicia en 0, es decir, si nuestro canvas es de (400,400), estamos diciendo que una vez que la gota se salga de la pantalla, vuelva a la posición inicial.
Con esto, tenemos programado una gotita que se mueve hacia abajo, y al salirse de pantalla, vuelve hacia arriba y continua cayendo.
Con esto, podemos hacer más de una variable, por ejemplo 3, y generar una lluvia de 3 gotitas.

```js
let gota1
let gota2
let gota3
function setup() {
  createCanvas(400, 400);
  gota1 = 0
  gota2 = 0
  gota3 = 0
}

function draw() {
  background(41);
  fill(220,220,250)
  ellipse(100,gota1,20,50)
  ellipse(200,gota2,20,50)
  ellipse(300,gota3,20,50)

  //cada una cae a una velocidad diferente
  gota1 = gota1 + 4
  gota2 = gota2 + 5
  gota3 = gota3 + 3

  //tres condicionales, uno para cada gota
  if (gota1 > 400){
    gota1 = 0
  }
  if (gota2 > 400){
    gota2 = 0
  }
    if (gota3 > 400){
    gota3 = 0
  }
}
```
