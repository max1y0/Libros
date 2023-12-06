# Usando la clase
Si tenemos una clase persona, con los atributos nombre, apellido y año de nacimiento, creamos un archivo ```persona.py``` y ponemos lo siguiente: 
```python
class Persona:
	def __init__ (self,nombre,apellido,edad):
          self.nombre = nombre
          self.apellido = apellido
          self.edad = edad
```
Notar que en python es necesario agregar ```self``` (lo que en pseudocodigo era ```propio```, en los paréntesis). Si además tiene los métodos ```decirNombre``` y ```decirEdad```, tenemos que escribir “funciones” que resuelvan lo que hace el método y programarlo dentro del archivo. Resultando en esto:
```python 
class Persona:
	def __init__ (self,nombre,apellido,edad):
          self.nombre = nombre
          self.apellido = apellido
          self.edad = edad
      
      def decirNombre(self):
    	    return "me llamo" + self.nombre+self.apellido

      def decirEdad(self):
    	    return 2021- self.anio_nac
```

Con eso, la clase está programada y lista para usarse en distintos programas. 

## Usando la clase
Supongamos que tenemos el siguiente algoritmo (en otro archivo, normalmente llamado, ```principal.py```) que la usa:
```python
from persona import Persona

persona1 = Persona("Juan","Perez",2001)
```
Hay que notar, que al principio, la línea ```from persona import Persona```

indica que vamos a usar la clase que escribimos en el archivo ```persona.py```

Después, la línea ```persona1 = Persona("Juan","Perez",2001)```

Crea un objeto  de clase persona, asignando valores Juan, Perez y 2001 a los atributos ```nombre```, ```apellido```, ```anio_nac``` respectivamente. 

Si actualizamos el código a esto: 
```python
from persona import Persona

persona1 = Persona("Juan","Perez",2001)


print(persona1.nombre)
print(persona1.decirNombre())
print(persona1.decirEdad())
```

Dado que los métodos retornan tanto textos como números, al hacer ```print``` de estos, imprime justamente lo que la función está retornando. En este caso, los tres ```print``` del final escriben lo siguiente:
```
Juan
me llamo Juan Perez
22
```

Notar que cuando hacemos ```persona1.nombre``` estamos accediendo a un **atributo**. En cambio cuando ponemos ```persona1.decirNombre()``` estamos accediendo a un **método**. La diferencia está en los paréntesis al final.
