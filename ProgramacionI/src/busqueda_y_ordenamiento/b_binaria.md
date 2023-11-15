# Busqueda dicotómica

Buscar de forma secuencial puede ser intuitivo pero en una secuencia larga, la cantidad de pasos que hace el programa crece proporcionalmente.

Una secuencia de 1000 elementos, en el peor de los casos, la cantidad de pasos que hace es justamente 1000. Y podemos suponer que el caso promedio es que encuentre el elemento en aproximadamente 500 pasos.

Hay un método de búsqueda que, para una secuencia de 1000 elementos, reducimos la cantidad de pasos a 10... **en el peor caso**.

El requisito para poder aplicar este método tan potente, es tener la secuencia ordenada previamente (usando los algoritmos previos por ejemplo).

La idea es la siguiente:

1. Buscar el elemento que está a la mitad del arreglo.
2. Si mi elemento a encontrar es más grande que el de la mitad, busco en la mitad superior, sino en la mitad inferior.
1. La búsqueda en esos subsecuencias se realiza de la misma manera. Buscando el elemento de la mitad, comparando y seleccionando submitades nuevamente.
1. La búsqueda termina cuando ese elemento a la mitad en algún momento es el que busco o, cuando la subsecuencia que se busca ya no tiene elementos.

### Ejemplo 1
Si queremos buscar el elemento ```4```, que si está en la secuencia
```py
[0,1,3,4,6,8,9,11,12]
```
El número de la mitad es 6, entonces se pregunta si ```4 > 6```. Como es más chico, se busca en la submitad de la izquierda
```py
[0,1,3,4,6]
```
El número de la mitad es 3, entonces pregunta ```4>3```, Como es más grande, busca en la submitad de la derecha
```py
[3,4,6]
```
El número de es 4, justamente el mismo que estamos buscando. Se termina la búsqueda

### Ejemplo 2
Si queremos buscar el elemento ```10```, que no está en la secuencia
```py
[0,1,3,4,6,8,9,11,12]
```
El número de la mitad es 6, entonces se pregunta si ```10 > 6```. Como es más grande, se busca en la submitad de la derecha
```py
[6,8,9,11,12]
```
El número de la mitad es 9, entonces se pregunta si ```10 > 9```. Como es más grande, se busca en la submitad de la derecha
```py
[9,11,12]
```
El número de la mitad es 11, entonces se pregunta si ```10 > 11```. Como es más chico, se busca en la submitad de la izquierda
```py
[9]
```
El número de la mitad es 9, entonces se pregunta si ```10 > 9```. Como es más grande, se busca en la submitad de la derecha
```py
[]
```
La submitad es vacía, entonces no encontré el número en la secuencia.