# Funciones Propias

Las funciones propias son las que nosotros como programadores diseñamos y agregamos a nuestros programas según lo que necesitemos.

<!-- TODO: agregar imagen del coso funcion -->
El uso de una función consta de dos partes: La **definición** y la **invocación**.

<!-- TODO: completar -->
## Definición
La definición es donde programamos el algoritmo de nuestra función, las funciones se definen abajo de todo. La estructura es la siguiente
```js
function nombre_de_funcion(){
    //codigo que resuelve el subproblema
}
```

## Invocación
La invocación es cuando la función es usada. y puede invocarse las veces que se necesite. Para invocarla se escribe sólo el nombre de la función en donde sea necesaria usarla en el bloque ```draw```.

```js
function draw(){
    ...
    nombre_de_funcion()
}
```

### Ejemplo
Vamos a realizar una función que dibuje una nube en el canvas. Para dibujarla vamos a usar varios circulos pintados de gris
```js
function setup(){
    createCanvas(600,400)
}
function draw(){
    background(220)
    //invocación
    nube()
}

//definicion
function nube(){
    fill(140)
    ellipse(50,50,50,50)
    ellipse(80,70,50,50)
    ellipse(85,40,50,50)
    ellipse(120,70,50,50)
    ellipse(110,50,50,50)
}
```

<!-- TODO: posible subseccion? -->

