# Ciclos while
El ciclo while (se pronuncia wail) se usa cuando sabemos que tenemos que repetir, pero __no sabemos bien cuántas veces__. 

En español se traduce como:  "ciclo mientras"

Usamos este ciclo cuando sabemos que tenemos que repetir mientras se dé alguna condición. Cuando esa condición ya no se cumple, se deja de ciclar. 

Pensemos en el siguiente ejemplo: 
> Mientras me digan que no, voy a seguir repitiendo la pregunta 'soy el mejor?' "
```py
respuesta='no'
while (respuesta=='no'):
	print ("Soy el mejor?")
	respuesta = input()
```
_(en este caso necesito inicializar la variable en 'no' para que mínimo repita una vez)_
