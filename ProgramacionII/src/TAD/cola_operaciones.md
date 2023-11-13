# Operaciones

```Encolar(x)```
Inserta al final de la secuencia el elemento ```x```
```Desencolar()```
Elimina de la secuencia el elemento en primer lugar
```Consultar() ```
Retorna el elemento que está en primer lugar para ser utilizado
```Vacía()```
Retorna verdadero si la cola está vacía, falso en caso contrario 
```Llena()```
Retorna verdadero si la cola está llena, falso en caso contrario.

|Operacion | Descripción|
|-------|------|
| Q = cola(4) | Primero creamos una variable Q de tipo cola, de tamaño 4. |
|print(Q.vacia())| Hacemos un print de la operación vacía, que retorna verdadero porque la cola está recién creada y vacía.|
|Q.encolar(2)| Luego encolamos el número 2 |
|Q.encolar(3)| y después el número 3. |
|x = Q.consultar()|Guardamos en una variable x lo que retorna consultar. Es decir, x termina teniendo el numero 2.|
|print(x)| Se imprime x|
|Q.desencolar() | Por último, se desencola el 2|
|print(Q.llena())| Se imprime el resultado de la operación llena, que es falso|

En el gráfico muestro paso a paso cómo fue cambiando la cola.
<!-- TODO:  insertar imagen -->

[0,0,0,0] -> [0,0,0,2] -> [0,0,3,2] -> [0,0,0,3]