# Estructura Condicional

La estructura secuencial es usada cuando es necesario tomar decisiones en función de los datos que se están manejando en nuestro programa. Una estructura condicional esta compuesta por una (o más) condición lógica, e instrucciones que se ejecutarían dependiendo de la evaluación de la condición. Existen muchas formas de componer una estructura condicional, muchas dependiendo del lenguaje. Pero se podrían resumir a tres:

### Una alternativa
Esta composición, evalúa una condición, en el caso de ser verdadera, se ejecuta un conjunto de instrucciones. Caso contrario, se continúa el flujo del algoritmo.
```py
    [...]
    if (<condicion>):
        <instrucciones>
    [...]
```

### Dos alternativas
Esta composición, evalúa una condición, en el caso de ser verdadera, se ejecuta un set de instrucciones. Caso contrario, se ejecutan otro set de instrucciones. Luego de ejecutado una u otra rama, se vuelve al flujo del programa.
```py
    [...]
    if (<condicion>):
        <instrucciones>
    else:
        <instrucciones>
    [...]
```

### Múltiples alternativas
Esta composición, a diferencia de las anteriores, evalúa más de una condición. Cada condición esta vinculada a un set de instrucciones. Cuando una de esas condiciones resulta verdadera, se ejecuta dicha instrucción y se continúa con el flujo del programa.
```py
    [...]
    if (<condicion>):
        <instrucciones>
    elif (<condicion2>):
        <instrucciones>
    elif (<condicion3>):
        <instrucciones>
    [...]
    elif (<condicionN>):
        <instrucciones>
    [...]

```

Ademas, es posible usar la clausula ```else``` como última condicion en un ```elif```. En este caso las instrucciones debajo del else se ejecutarían cuando **ninguna de las condiciones anteriores sea verdadera**


Esta condición es propensa a errores, por lo que es necesario tener en cuenta las siguientes buenas prácticas:
* Las condiciones deben cubrir todo el dominio de los datos a consultar
* Las condiciones deben ser mutuamente excluyentes

## Equivalencias
La composición de muchas alternativas (a la que le vamos a llamar informalmente como ```elif```) es en realidad un atajo a escribir composiciones de dos alternativas anidadas

```py
if (<condicion1>):
    <instrucciones1>
else:
    if (<condicion2>):
        <instrucciones2>
    else:
        if (<condicion3>):
            <instrucciones3>
        else:
            <instrucciones4>
```
```py
[...]
if (<condicion1>):
    <instrucciones1>
elif (<condicion2>):
    <instrucciones2>
elif (<condicion3>):
    <instrucciones3>
else:
    <instrucciones4>
[...]
```

Por otro lado, los siguientes códigos **no son equivalentes** por más que parezcan a simple vista que sí lo son.
```py
if (<condicion1>):
    <instrucciones1>
if (not<condicion1>):
    <instrucciones2>
```
```py
if (<condicion1>):
    <instrucciones1>
else:
    <instrucciones2>
```
