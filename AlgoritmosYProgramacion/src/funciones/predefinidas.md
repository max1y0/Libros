# Funciones Predefinidas

Las funciones predefinidas son funciones que ya existen en el lenguaje de programación y pueden ser usadas sin necesidad de saber como están programadas. Justamente ya las estuvimos usando sin saber que eran funciones: ```rect```, ```ellipse```, ```background```, ```fill```, etc.

De estas funciones predefinidas, una interesante es ```random```

## La función random
La función ```random``` es una abstracción, que recibe dos números como entrada, y retorna un sólo valor resultado
<!-- TODO: agregar dibujo funcion random  -->

```random``` retorna un número al azar. Los datos de entrada son los límites en donde se puede mover el número generado. 

### Ejemplos

```random(1,7)``` retorna un número al azar entre 1 y 6 
```random(0,400)``` retorna un número aleatorio entre 0 y 399
```fill(random(0,255),random(0,255),random(0,255))``` configura el color de relleno en un color totalmente aleatorio

