# Busqueda secuencial

La búsqueda lineal implementa la noción de buscar sobre una secuencia yendo uno por uno e inspeccionando si es lo que buscamos. Si encontramos el elemento terminamos de recorrer.

La estructura general es como sigue:
```py
i = 0
cant = len(secuencia)
while (i < cant and not (verificar(secuencia[i])):
    i+=1
if i>cant:
    print("Elemento no encontrado")
else:
    print("elemento encontrado en la posición",i)
```

La funcion ```verificar(x)``` es una función que devuelve verdadero o falso según el elemento x que le pasemos, sea lo que buscamos o no. En este caso es útil para ejemplificar la plantilla, pero en muchos casos no es necesaria implementarla si la comparación es simple. 

Al finalizar el ciclo, si el ```i``` es más grande que el ```cant``` quiere decir que termine de recorrer la secuencia y nunca encontré el elemento. Caso contrario encontré lo que buscaba, y está justamente en la posición ```i```

Veamos un ejemplo donde queremos buscar el caracter '*' dentro de una secuencia de caracteres

```py
i = 0
cant = len(secuencia)
while (i < cant and not (secuencia[i] == '*'):
    i+=1
if i>cant:
    print("No hay asteriscos en la frase")
else:
    print("Encontré un asterisco en la posición: ",i)
```