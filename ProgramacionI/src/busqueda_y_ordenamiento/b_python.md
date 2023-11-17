# Búsqueda en python
## En python
Quizá podemos pensar que esto es trabajo extra, ya que en python existe una instrucción que me devuelve verdadero si un elemento existe en una lista o no:
```py
if 10 in secuencia:
    print("si esta")
else:
    print("no está")
```
Este método de fondo utiliza búsqueda lineal. Y si bien es más simple que escribir el método lineal que vimos antes, escribir el método a mano tiene sus ventajas cuando necesitamos hacer una búsqueda más compleja, o cuando necesitamos realizar cosas con los elementos mientras estamos buscando. Además hay que tener en cuenta las desventajas en sí de realizar una búsqueda lineal sobre una lista grande. Si tenemos una lista ordenada, es ineficiente utilizar este método y conviene usar una implementación en python de la búsqueda binaria.