# Colas en Python
Para usar colas en python tenemos que importar el módulo Queue (cola en inglés). Y las operaciones se traducen como sigue:
<!-- TODO: armar la tabla comparativa -->
|Pseudocodigo | Python |
|---|---|
|Encolar(x)|put(x)|
|Desencolar()|get() |
|Consultar()| get()|
|Vacía()|empty()|
|Llena()|full()|
_Get funciona como un desencolar y consultar al mismo tiempo. Nos retorna el valor que sigue de la cola y automáticamente lo elimina._


```qsize()```

Una función útil en python es indicar que tamaño tiene la cola en tal momento. Si está vacía retorna 0


Si traducimos el código anterior a python tenemos lo siguiente:
<!-- TODO: armar la tabla comparativa o directamente poner el codigo traducido (con un link al codigo anterior?) -->
```py
Q = Queue(maxsize = 4)

print(Q.empty())
Q.put(2)
Q.put(3)

x = Q.get()
print (x)

print(Q.full())
```
_Notar que no se hace un “desencolar” porque en python no es necesario_
