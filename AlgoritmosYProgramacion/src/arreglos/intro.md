# Arreglos

## Qué era una variable
* Lugar de memoria, con nombre
* Sirve para guardar un y sólo un dato.
* Puedo variar el dato guardado cuantas veces quiera

_Aunque..._

Hay uno de estos items que no es del todo correcto.

* ~~Sirve para guardar un y sólo un dato.~~
* **Sirve para guardar un dato de un tipo.**

## Variables de tipo arreglo

Una variable de tipo arreglo, es una variable que puede guardar secuencia de datos finita de un mismo tipo _(por ejemplo, un arreglo numérico sólo puede guardar números)_
```js
let arreglo = [elemento1, elemento2, elemento3 ,elemento4, elemento5, elemento6]
```
De un arreglo es importante distinguir entre cuatro características: tipo, tamaño, posición y datos.
* Tipo: Es el tipo de datos del elemento de la secuencia
* Tamaño: Es la cantidad de elementos que tiene el arreglo
* Posición: Indica la ubicación de los elementos en un arreglo. La primera posición es la 0, la siguiente es la 1, y así sucesivamente.
* Datos: Los datos son justamente los elementos individuales que están dentro de un arreglo.

Para acceder a una celda del arreglo se usa la notación: ```nombre_arreglo[indice]``` 

### Ejemplo

```js
let edades = [12, 4, 9,33, 0, 2, 5,15, 5,90]
```
* Tipo: Numérico 
* Tamaño: 10
* En el arreglo ```edades``` en la posición del índice ```2```, se encuentra el dato ```9```
* En el arreglo ```edades``` el dato ```0``` se encuentra en la posición ```5```
```js
edades[2] -> 9
edades[0] -> 12
edades[2+2] -> 33
edades [3]+2 -> 11
edades [ edades[7] ] -> 0
```