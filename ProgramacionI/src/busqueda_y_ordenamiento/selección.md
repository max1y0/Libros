# Ordenamiento selección

El ordenamiento burbuja se guía bajo este algoritmo general:
1. Empezar a recorrer la secuencia guardando el que es más chico
1. Una vez recorrido, reemplaza el número más chico encontrado con el que está en primera posición
1. El primer número queda fijo y se vuelve a empezar por el punto 1.

### Veamos la traza para la siguiente lista de números:

```py
[11,3,21,3,15,0]
```
Al recorrer todo el arreglo, encuentra que el número más chico es el ```0```

```py
[0,3,21,3,15,11]
```
Intercambia el número más chico encontrado por el que está en primer lugar.
```py

[[0],3,21,3,15,11]
```
El primer número queda fijo y se vuelve a empezar, buscando el segundo más chico

Veamos los pasos más rápido:
```py
[[0,3],21,3,15,11]
[[0,3],21,3,15,11]
[[0,3,3],21,15,11]
[[0,3,3,11],15,21]
[[0,3,3,11,15],21]
[[0,3,3,11,15,21]]
```