# Estructura Repetitiva

La estructura repetitiva nos es útil cuando necesitamos realizar las mismas instrucciones de forma consecutiva, ya sea una cantidad predeterminada de veces o no.

Es decir, cuando queremos repetir un bloque de acciones nos encontramos con dos posibilidades:
* Sé cuantas veces necesito repetir las instrucciones.
* De antemano no conozco cuantas veces necesito repetir, pero conozco una _condición_ que debe cumplirse para repetir

## Ciclo ```for```
El ciclo o estructura repetitiva ```for``` se usa cuando el conozco el número de repeticiones que tengo que hacer para cierto set de instrucciones. Cualquier ciclo ```for``` necesita una __variable de control__ (normalmente se usan las variables i, j, k), esta es una variable nos sirve para controlar la cantidad de repeticiones que vamos a realizar.

En general esta instruccion requiere los siguientes datos:
* Valor de inicialización de nuestra variable de control
* Valor final de nuestra variable de control
* El paso de nuestra variable de control (de cuanto en cuanto avanza).

### Sintaxis
La sintaxis en python para este ciclo es la siguiente
```py
for <variable de control> in range (<valor de inicio>,<valor final>,<paso>):
    <Instrucciones a repetir>
```

**Ejemplo**:
```py
for i in range (0,5,1):
    print (i)
```
* 0 es nuestro valor de inicialización
* 5 es nuestro valor de finalización. La variable i, __al salir del ciclo__ vale 5
* 1 es el paso, es decir que nuestra variable avanza de uno en uno

> NOTA: En python, la sintaxis de los ciclos for es bastante diferente a los ciclos for en la mayoría de los lenguajes. En estos la sintaxis es más explícita con el uso de la variable de control. Por ejemplo, el código anterior en C se escribe como ```for (int i = 0 ; i <5 ; i = i+1){```

## Ciclo ```while```
El ciclo mientras, lo usamos cuando no sabemos la cantidad de veces que vamos a repetir. Para esto, este ciclo usa una __condición lógica__ para controlar la cantidad de veces que vamos a repetir. La condición expresa lo que se debe cumplir para que el ciclo se ejecute, por lo que se denomina _condición de continuación_.
El funcionamiento es el siguiente:
* Se evalúa la condición.
    * Si la condicición es verdadera: se ejecutan las acciones del bloque del ciclo una vez, y se vuelve a evaluar la condición.
    * Si la condición es falsa: no se ejecutan las acciones y se sigue con la ejecución normal del código.

### Sintaxis
```py
while (<condicion de continuación>):
  <Instrucciones a repetir>
```

**Ejemplos:**
```py
i = 0
while (i < 5):
    print (i)
    i+=1
```

```py
opcion = 0
while (opcion != 4):
    print ("menu:")
    print("1 - cargar datos")
    print("2 - mostrar datos")
    print("3 - eliminar datos")
    opcion = int(input())
    [...]
```

### Precauciones
Al no conocer cuantas veces uno tiene que repetir, es posible que la construcción de un ciclo ```while``` sea propensa a errores, principalmente la de __ciclos infinitos__. Para esto es importante tener en cuenta las siguientes cuestiones:
* La condición de continuación tiene que ser falsa en algún momento
* Cada vez que ciclemos, nos vayamos "acercando" a que la condición de continuación sea falsa
* Que las variables que se usan en la condición de continuación, sean modificadas dentro del ciclo.
