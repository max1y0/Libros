# Atributos
Los objetos, similares a los arreglos, son estructuras que permiten guardar más de un valor. Pero en lugar de pensarlo como una secuencia o lista de cosas, se lo piensa como una sola cosa con distintas características. 

Supongamos que tenemos que hacer un programa que maneja los datos de una persona, y se necesita el dni, la edad y el nombre. Lo normal hasta ahora sería hacer tres variables para cada cosa. Pero en realidad podemos crear un objeto con tres atributos.

```python
persona = { 
  nombre: "martin",
  apellido: “funes”,
  edad: 46
  dni: 26700808
}
```

El nombre del objeto, puede ser cualquiera, la idea es que tenga que ver con lo que estamos intentando modelar, en este caso una persona. La cantidad y nombres de atributos puede ser la que consideremos, no hay límite. Es más, un atributo puede incluso ser un arreglo, u otro objeto “más chico”.

Lo importante cuando diseñemos objetos es que evitemos rellenar un objeto con atributo que no tienen sentido dentro de ese objeto. Es decir, no tendría sentido que dentro de mi objeto persona haya atributos como ```cantidadDeRuedas``` o ```tamañoDeVentana```.

La idea es que nos sirva para modelar cosas que existen en la vida real o que tiene sentido que estén agrupadas.
