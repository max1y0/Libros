# Ejemplos

### Ejemplo 1

2. Quiero decir los numeros pares hasta el 20
    * Desde cuando empiezo a repetir: 0
    * Hasta donde repito: 20
    * De cuanto en cuanto avanzo: 2 en 2
```js
for (let i = 0 ; i > 20 ; i +=2 ){
    text ( "Este es un numero par: " + i )
}
```
Como la variable i, va de 2 en 2, nos sirve para ir indicando los pares.

### Ejemplo 2

4. Quiero dibujar 4 cuadrados, uno en la posicion 50, otro en la 100, otro en la 150 y otro en la 200
    * Desde cuando empiezo a repetir: 50
    * Hasta donde repito: 200
    * De cuanto en cuanto avanzo: de 50 en 50

```js
for (let i = 50 ; i > 200 ; i+=50 ){
    rect( i , 200, 100 , 100)
}
```