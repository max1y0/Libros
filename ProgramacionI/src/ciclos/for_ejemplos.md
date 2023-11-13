# Ejemplos
## Ejemplo 1
```py
for i in range (5):
    print ("Hola!", i+1)
```
A diferencia del código anterior, este tiene dos variantes muy sutiles. Por un lado, modificamos el rango en 5, es decir ahora sólo repite cinco veces. Además, sumamos en uno a la variable ```i``` en el ```print```, logramos que la cuenta sea un poco más natural, empezando en 1 en lugar de 0.
```
>Hola! 1
Hola! 2
Hola! 3
Hola! 4
Hola! 5
```

Si bien son modificaciones casi inocentes, nos dan a entender la facilidad para cambiar el número de repeticiones de un ciclo ```for```, así como la ventaja de poder usar la variable ```i``` a nuestro favor. Como por ejemplo en el siguiente caso:

## Ejemplo 2
```py
num = 7
for i in range (10):
    print (num,"x",i,"=",num*i)
```
Analicemos en detalle:

Primero, tenemos una variable ```num``` con el valor ```7```. 
El ciclo se repite 10 veces.
La instrucción que se repite es un ```print```, y es bastante complejo, veamos también por parte:

Primero imprime el valor de la variable ```num```.
Luego imprime la letra 'x'.
Al lado de esto imprime el valor de la variable ```i```.
Después escribe un signo igual.
Y por último escribe el resultado de multiplicar ```num``` por ```i```

Entonces, en una primera repetición, ```num``` vale ```7```, e ```i``` vale ```0```. Por lo que si seguimos paso a paso la descripción de nuestro ```print```, vamos a ver que se escribe por terminal lo siguiente:
```
>7 x 0 = 0
```
_(Al final hay un cero porque 7 multiplicado por 0 es 0)_

En la segunda vuelta de repetición, ```num``` sigue valiendo ```7```, pero ```i``` pasa a valer ```1```. Entonces
```
>7 x 1 = 7
```

Si seguimos consecutivamente hasta llegar a diez repeticiones podemos ver que el programa lo que hace es escribir la tabla multiplicar del 7
```
>7 x 0 = 0
7 x 1 = 7
7 x 2 = 14
7 x 3 = 21
7 x 4 = 28
7 x 5 = 35
7 x 6 = 42
7 x 7 = 49
7 x 8 = 56
7 x 9 = 63
```


