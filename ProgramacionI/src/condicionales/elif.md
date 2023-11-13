# Condicionales Elif
Como dijimos, en python hay un atajo a la segunda variante, el condicional elif
```py
if (nota < 7):
	print ("estas desaprobado")
elif (nota >= 7):	
	print ("estas aprobado")
elif (nota == 10):	
	print ("¡¡Un diez!!")
```


Para python, este código funciona exáctamente como la variante 2 (con su seguridad y robustez) pero tiene la legibilidad de la variante 1.

Entonces ¿Siempre que tengamos una condición con más de dos posibilidades vamos a usar elif? **La gran mayoría de los casos, si.**
