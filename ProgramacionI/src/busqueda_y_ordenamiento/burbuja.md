# Ordenamiento burbuja
El ordenamiento burbuja se guía bajo este algoritmo general:
1. Empezar a comparar el primer par de números
1. Si el número 1 es mas grande que el número 2, intercambiarlos
1. Avanzar al siguiente par y comparar como en 2.
1. Al llegar al final de la secuencia se deja fijo el último
1. Se empieza de nuevo por el punto 1.

### Veamos la traza para la siguiente lista de números:

```py
[11,3,21,3,15,0]
```
Primero compara el ```11``` y el ```3```. Como el ```11``` es mayor, los intercambia.

```py
[3,11,21,3,15,0]
```
Luego avanza al siguiente par, el ```11``` y el ```21```. En este caso no se intercambia por ser el ```11``` más chico

```py
[3,11,21,3,15,0]
```
En el siguiente par, el del ```21``` y el ```3```, se hace un intercambio.

```py
[3,11,3,21,15,0]
```
Compara el par de ```21``` y ```15``` y se intercambian.

```py
[3,11,3,15,21,0]
```
Por ultimo (para la primer pasada de la secuencia), compara el ```21``` con el ```0``` y los intercambia, dejando el ```21``` en el último lugar y **fijandolo**

```py
[3,11,3,15,0,[21]]
```

Ahora vuelve a empezar, pero el ```21``` ya no se modifica. Veamos los pasos más rápido:
```py
[3,11,3,15,0,[21]]
[3,3,11,15,0,[21]]
[3,3,11,15,0,[21]]
[3,3,11,0,15,[21]]
[3,3,11,0,[15,21]]
```
Al finalizar esta segunda pasada, el que queda fijo es el ```15```, y se vuelve a empezar, hasta que el que queda fijo es el primer número del arreglo.
```py
[3,3,11,0,[15,21]]
[3,3,11,0,[15,21]]
[3,3,11,0,[15,21]]
[3,3,0,[11,15,21]]
[3,3,0,[11,15,21]]
[3,0,[3,11,15,21]]
[0,[3,3,11,15,21]]
[[0,3,3,11,15,21]]
```