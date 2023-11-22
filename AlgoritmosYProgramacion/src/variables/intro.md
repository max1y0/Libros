# Variables
Una variable es un espacio de la memoria con nombre, para guardar valores. Y normalmente puede cambiar su valor con el correr del programa.

Una variable tiene tres instancias en su vida:
* Creación
* Inicialización
* Uso

### Creación
Para crear una variable se escribe la instrucción ```let``` seguida del nombre de la variable.
```js
let posicionX
```
### Inicialización
Inicializar la variable es asignarle el valor que va a tener al comienzo de su "vida"
```js
posicionX = 20
```
En este caso, asignamos a la variable ```posicionX``` el número ```20```
### Uso
El uso depende del problema que querramos resolver y se va a traducir a distintos tipos de instrucciones según corresponda.

## Ejemplo
```js
let posicionX
function setup(){
    createCanvas(400, 400)
    posicionX = 20
}
function draw(){
    background(192, 64, 0)
    rect(posicionX, 20, 50, 70)
}
```
Antes del bloque ```setup```, se crean las variables. En este caso su nombre es ```posicionX``` y va a representar una posición horizontal
```js
let posHorizontal
```

Dentro del bloque ```setup``` se inicializan las variables, asignándoles el valor inicial. En este caso es el valor numérico ```20```
```js
function setup(){
    createCanvas(400, 400)
    posHorizontal = 20
}
```

Generalmente las variables van a ser usadas en múltiples ocasiones en el bloque draw.
```js
function draw(){
    background(192, 64, 0)
    rect(posHorizontal, 20, 50, 70)
}
```

En este caso el programa funciona igual al mostrado anteriormente, en el sentido que dibuja un rectángulo en la pantalla, pero vamos a ver qué usar variables nos va a permitir realizar cosas más interesantes.