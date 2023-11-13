# Ciclos for
Vamos a empezar con el ciclo ```for```.  En este ciclo siempre sabés cuántas veces necesitas repetir, diez veces, cinco, mil, etc. Es muy similar al repetir de scratch.
```py
for i in range (10):
    print ("Hola!")
```
Lo que hace este código es simplemente "Hola!" diez veces.

Miremos con más detalles:
```py
range (10) 
```
Es el rango de repetición, representa la cantidad de veces que se van a repetir las instrucciones del ciclo.
```py
    print ("Hola!")
```

En este caso es la instrucción que se va a repetir. Podemos poner más instrucciones siempre respetando el nivel de indentación dentro del ciclo.

Ahora... ¿Qué es esa ```i``` que está ahí metida?

La ```i``` es una variable numérica muy interesante. Siempre tiene que estar cada vez que escribimos un ```for```, y su función es llevar la cuenta de las repeticiones.
Es decir, que en la primera repetición ```i``` vale ```0```, en la segunda repetición, vale ```1```, en la tercera vale ```2``` y así hasta que lluegue a la cantidad de repeticiones indicada en el rango (i empieza a contar desde cero)

Si a mi programa lo cambio y además de escribir hola, escribo ```i```:
```py
for i in range (10):
	print ("Hola!", i)
```

Cuando ejecute el algoritmo va a pasar lo siguiente:
```
>Hola! 0
Hola! 1
Hola! 2
Hola! 3
Hola! 4
Hola! 5
Hola! 6
Hola! 7
Hola! 8
Hola! 9
```

Como ```i``` empieza desde 0, termina en 9. Pero fijense que hay diez holas, o sea diez repeticiones.
