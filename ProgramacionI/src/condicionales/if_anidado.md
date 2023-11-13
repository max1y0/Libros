# Condicionales If Anidados
Cuando se resuelve un problema, se dice que no hay dos algoritmos iguales. Pero para el problema anterior, es probable que su solución pueda parecerse a alguna de estas dos variantes.

Variante 1:
```py
if (nota<7):
	print ("estas desaprobado")
if (nota>=7):	
      print ("estas aprobado")
if (nota==10):	
      print ("¡¡Un diez!!")
```

Variante 2:
```py
if (nota<7):
	print ("estas desaprobado")
else:
	if (nota>=7):
	      print ("estas aprobado")	
      else:
	      if (nota==10):
                    print ("¡¡Un diez!!")
```


La variante 1 parece ser más fácil de entender y programar, pero no es recomendable cuando las instrucciones dentro de cada condición se vuelven complejas. 

La variante 2 (llamada normalmente **if anidado**) es mucho más segura y robusta, pero se puede volver totalmente ilegible cuando tenemos más de tres condiciones.

Por suerte, python tiene una solución a esto para que podamos escribir la variante 2, pero de forma mucho más simple: la estructura [elif](./elif.md).

