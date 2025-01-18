# Ejemplos
<!-- TODO: agregar ejercicios hechos en clase -->
## Cronómetro
Un ejemplo más simple es el de realizar un "cronómetro". Usando la instrucción ```text()``` podemos escribir en el lienzo cualquier mensaje o los contenidos de una variable. En este código vemos en tiempo real como la variable va aumentando de uno en uno a una velocidad de 60 sumas por segundo.

```js
let numero; //creacion
function setup() {
  createCanvas(400, 400);
  numero = 0; //inicializacion
}
function draw() {
  background(255, 200, 200);
  textSize(32);//instrucción para modificar el tamaño del texto
  rect(130, 130, 140, 120);
  fill(21);
  text(numero, 180, 200);//instrucción para escribir el contenido de la variable número
  numero = numero + 1; //uso
}
```

### Deformando figuras
No sólo vamos a poder hacer que un rectángulo o ellipse se muevan. Si usamos la variable en otros parámetros podemos modificar su ancho o alto
```js
rect(130, 130, numero, 120); //modificamos su ancho
```

```js
rect(130, 130, 120, numero); //modificamos su alto
```

Es más, usando variables en otras instrucciones también podemos generar efectos interesantes. ¿Qué pasará en este caso?

```js
fill(variable1, 130, vaiable2); //asumiendo que ambas variables van cambiando de valor constantemente
```
