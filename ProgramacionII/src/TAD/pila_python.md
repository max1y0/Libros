# Pilas en Python
En python no hay una implementación de pilas, para poder usarlas se pueden usar listas y usar las operaciones de lista de forma que respete las operaciones de pilas, o usar ```LifoQueue```. Usando la ```LifoQueue``` las operaciones se traducen como sigue (se agrega una tabla que indica como suelen ser las operaciones de pilas en otros lenguajes de programación):
<!-- TODO: armar la tabla comparativa -->
|Pseudocodigo | Python | Operaciones en general |
|---|---|---|
|Aplilar(x)|put(x)|push(x)|
|Desapilar()|get()|pop()|
|tope()|get()|top()|
|Vacía()|empty()|empty()|
|Llena()|full()|full()|

_Get funciona como un desencolar y consultar al mismo tiempo. Nos retorna el valor que sigue de la cola y automáticamente lo elimina._

```qsize()```

Con ```LifoQueue```, qsize funcione igual que con colas, nos indica el tamaño actual de la pila.

### Ejemplo
Si traducimos el código anterior a python tenemos lo siguiente:

```py
from queue import LifoQueue
S = LifoQueue (maxsize = 4)

print(S.qsize())
S.put(2)
S.put(3)

x = S.get()
print (x)

print(S.full())
```



