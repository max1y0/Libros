# Hola a vos
Hola a vos
Ahora vamos a partir del ```holaMundo``` para hacer un nuevo programa. La idea es hacer un programa que nos pregunte cuál es nuestro nombre y luego nos salude por la terminal.

Para eso vamos a ir paso a paso:

## Paso 1.
Por lo que sabemos print nos escribe por terminal un mensaje (antes "hola mundo")
Usando esto vamos a cambiar el mensaje para que nos diga algo como "¿cuál es tu nombre?" (para evitar errores, es mejor no poner las tildes en los mensajes)
```python
print ("¿como te llamas?")
```

## Paso 2.
Para seguir, vamos a escribir lo siguiente:
```python
print ("¿como te llamas?")
nombre = input()
```

Lo que estamos haciendo es, crear una variable que se llama nombre, y con la instrucción ```input()``` hacemos que dentro de la variable se guarde lo que escribamos con el teclado

## Paso 3. 
Si ya sabemos que en nombre va a haber información guardada, y con ```print``` podemos escribir en terminal, podríamos probar lo siguiente:
```python
print ("¿como te llamas?")
nombre = input()
print ("hola",nombre)
```

Si probamos este programa tal cual está, vamos a ver que en la terminal aparece el mensaje "como te llamás" y no pasa mas nada.
```
>¿cómo te llamas?
_
```

Es porque el programa está esperando a que ingresemos por teclado información. Si escribimos ahí mismo cualquier cosa (preferentemente nuestro nombre :) ) y apretamos enter, vamos a ver que el programa ahora muestra en terminal el mensaje:
```
>¿como te llamas?
Maxi
>Hola Maxi
```
_(En el caso de que hayamos escrito maxi)_
