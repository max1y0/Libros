# Pilas en Python
Para usar colas en python tenemos que importar el módulo Queue (cola en inglés). Y las operaciones se traducen como sigue:
<!-- TODO: armar la tabla comparativa -->
Encolar(x)
put(x)
Desencolar()
Consultar() 
get()
Get funciona como un desencolar y consultar al mismo tiempo. Nos retorna el valor que sigue de la cola y automáticamente lo elimina.
Vacía()
empty()
Llena()
full()


qsize()
Una función útil en python es indicar que tamaño tiene la cola en tal momento. Si está vacía retorna 0


Si traducimos el código anterior a python tenemos lo siguiente:
<!-- TODO: armar la tabla comparativa o directamente poner el codigo traducido (con un link al codigo anterior?) -->

Q = cola(4)

print(Q.vacia())
Q.encolar(2)
Q.encolar(3)

x = Q.consultar()
print(x)
Q.desencolar()
print(Q.llena())
from queue import Queue
Q = Queue(maxsize = 4)

print(Q.empty())
Q.put(2)
Q.put(3)

x = Q.get()
print (x)

print(Q.full())



Notar que no se hace un “desencolar” porque en python no es necesario
