# Ordenamiento inserción
El ordenamiento inserción se guía bajo este algoritmo general:
1. Empezar a comparar el primer par de números
1. Si el número 1 es mas grande que el número 2, intercambiarlos. Estos quedan ordenados entre si.
1. Avanza al siguiente número, y lo inserta en la subsecuencia ordenada en la posición que corresponde.
1. Repetir el punto 3. hasta insertar todos los números.

### Veamos la traza para la siguiente lista de números:

```py
[11,3,21,3,15,0]
```
Primero compara el ```11``` y el ```3```. Como el ```11``` es mayor, los intercambia.

```py
[[3,11],21,3,15,0]
```
Luego avanza al ```21```. Se lo inserta en la subsecuencia ordenada en la posición correcta

```py
[[3,11,21],3,15,0]
```
En el siguiente número, el ```3```, se lo ingresa en la subsecuencia en la primera posición

```py
[[3,3,11,21],15,0]
```
Luego el ```15``` 

```py
[[3,3,11,15,21],0]
```
Por ultimo se inserta el ```0```

```py
[[0,3,3,11,15,21]]
```
