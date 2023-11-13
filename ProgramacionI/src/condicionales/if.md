# Condicionales If
Ejemplo:
```py
if (nota<7):
    print ("estas desaprobado")
else:
    print ("estas aprobado")
```
Analicemos parte por parte:

```py
(nota<7):
```
Esta es nuestra condición, es lo que le vamos a preguntar a las variables o datos del programa. En este caso preguntamos si la variable ```nota``` es menor a ```7```

Abajo de la línea del ```if```, con indentación (sangría) ponemos las instrucciones si la condición resulta ser verdadera
```py
    print ("estas desaprobado")
```

Para nuestro ejemplo, para que la condición sea verdadera, la variable nota tiene que tener números menores a 7. Si es así, se escribe en terminal ```“estas desaprobado”```

La instrucción ```else``` es opcional, se pone en los casos en donde necesitemos ejecutar ciertas instrucciones si la condición es verdadera, y ciertas otras si es falsa.
```py
else:
	print ("estas aprobado")
```

En el caso de que se use, se pone ```else:``` y abajo con indentación, ponemos las instrucciones que se ejecutarían si la condición resulta ser falsa. En nuestro caso, la condición es falsa cuando la variable ```nota``` tiene 7 o más.


### Problema:
¿Cómo se podría cambiar el código para que además de eso, felicite si la nota es exactamente 10?
