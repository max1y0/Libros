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

## Uso en programación
El arreglo en programación es útil cuando, como dijimos anteriormente, necesitamos guardar una secuencia de datos. Los datos guardados en el arreglo pueden accederse como cualquier variable accediendo a estos usando su índice.
```js
rect(20,20,datos[3],datos[3])
```
Pero generalmente, queremos a acceder a todos los elementos de un arreglo y hacer un tratamiento sobre ellos. Para esto entonces, es necesario ciclar sobre el arreglo. Es decir, usar una estructura repetitiva para tratar cada elemento en particular del arreglo.

### Recorriendo el arreglo usando el ciclo for
Supongamos el arreglo ```edades``` definido antes, y que queremos mostrar los datos en el canvas.

Si repasamos el ciclo for, necesitamos tres cosas: desde donde empiezo a ciclar, hasta cuando necesito ciclar, y de cuanto en cuanto avanzo.
**Desde donde se comienza:** Los arreglos comienzan a contabilizar desde la posición 0, así que lo correcto es empezar a ciclar desde 0.
**Hasta cuando ciclo:** Generalmente, vamos a recorrer todo el arreglo, entonces, necesitamos ciclar hasta que las repeticiones sean iguales al tamaño del arreglo (si el arreglo tiene tamaño 10, repito diez veces). la instruccoin ```nombre_de_arreglo.length``` nos indica el tamaño de un arreglo dado.
**De cuanto en cuanto avanzamos:** Si vamos a recorrer todos los elementos del arreglo, vamos a avanzar nuestro índice de uno en uno.

Teniendo esto nuestro for se definiría como sigue
```js
for (let i = 0; i < edades.length; i+=1){
  // instrucciones
}
```
Entonces, si en nuestro for, la variable ```i``` va aumentando uno a uno, podemos acceder a todos los elementos de arreglo usando esta variable como índice. Es decir:

```js
for (let i = 0; i < edades.length; i+=1){
  text (edades[i],20,20)
}
```
Este código automáticamente va a mostrar todas los números que están guardados en el arreglo edades. Aunque este algoritmo no funciona, porque cada número se está dibujando en la misma posición, la (20,20). Podemos aprovechar la variable i para ir moviendo la posición de los números

```js
for (let i = 0; i < edades.length; i+=1){
    text (edades[i],20*i,20)
  }
```
