# Anexo
Código final del ejemplo persona
```python
from persona import Persona
def esMayor(persona1, persona2):
	if (persona1.decirEdad() > persona2.decirEdad()):
		print(persona1.nombre + "es la persona más grande")
	else:
		print(persona1.nombre + "es la persona más grande")

def familia (persona1, persona2):
	if (persona1.apellido == persona2.apellido):
		print( "son familia?")
      else:
		print("apellidos diferentes")

persona1 = Persona()

persona1.nombre = "Juan"
persona1.apellido = "Perez"
persona1.anio_nac = 2001

persona2 = Persona ()
persona2.nombre = "Lucia"
persona2.apellido = "Rodriguez"
persona2.anio_nac = 2010

print(persona1.nombre)
print(persona1.decirNombre())
print(persona1.decirEdad())

esMayor (persona1, persona2)
familia (persona1,persona2)
```
principal.py

```python
class Persona:
	nombre = ""
	apellido = ""
	anio_nac = 0
      
      def decirNombre(self):
    	    return "me llamo" + self.nombre+self.apellido

      def decirEdad(self):
    	    return 2021- self.anio_nac
```
persona.py
