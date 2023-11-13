# Resumen de Instrucciones
Sin saberlo, usamos diversos tipos de instrucciones en nuestro código anterior. Repasemos cada una de ellas.
## Creación de variables. 
```python
numero = 0
nota = 10
nombre = diego
```
Se escribe el nombre de la variable, el signo igual y el valor de inicialización. 

## Asignación
```python
numero = numero + 1
resultado = (nota* 5)/2
nombre = marcos
```
Escribiendo el nombre de una variable existente, usando el signo igual se asignan diversas expresiones o valores.
Las operaciones se escriben como sigue: 

| Operador | Descripción |
|--|--|
|+ | Para sumar|
|- |Para restar|
|* |Para multiplicar|
| /|Para dividir|

## Entrada de datos
```python
print ("cual es tu signo?")
signo = input()

print ("cual es tu edad?")
edad = int(input())
```
Asignamos a una variable existente la función ```input() ```para poder ingresar información mediante el teclado en tiempo de ejecución. Cuando queramos ingresar datos numéricos, es necesario usar ```int(input())```. Si no usamos esto, es imposible hacer operaciones matemáticas con esta variable numérica

### Imprimir por pantalla
```python
print ("Hola Mundo")
print (nombre)
print ("tu edad es", edad)
```
Todo lo que esté dentro del paréntesis será mostrado a modo de salida. Ponemos en comillas lo que queremos que sea un mensaje de texto, y sin comillas cuando queremos mostrar variables.
