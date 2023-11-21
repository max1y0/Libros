# Sintaxis
Según lo que estuvimos viendo anteriormente, tenemos las siguientes instrucciones:
```js
createCanvas(400,400)
```
```js
rect(70,40,90,110)
```
Ahora necesitamos organizarlo en un código funcional. Para esto tenemos que entender el concepto de bloques. Los bloques de programación son las instrucciones que están entre los símbolos ```{ }```

Los programas p5 generalmente cuentan con dos bloques.
```Setup``` sirve como nuestro bloque de inicialización de variables, tamaño de lienzo, y a veces configuración del color de fondo. Las instrucciones de un bloque ```setup``` se realizan sólo una vez.
El bloque ```draw``` es donde vamos a escribir todas nuestras instrucciones de dibujo. ```Draw``` es un ciclo infinito. Al terminar todas las instrucciones del bloque se vuelven a ejecutar desde el principio.
```js
function setup(){
    createCanvas(400, 400)
}
function draw(){
    rect(70, 40, 90, 110)
}
```
_Código en p5 con el canvas de 400 píxeles de ancho por 400 de alto. Y un rectángulo en la posición (70,40) de 90 píxeles de ancho y 110 de alto._
