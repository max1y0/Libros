# Usando los ejemplos
Si ampliamos nuestro código principal para que tenga más de un objeto. Podemos usar estas funciones
```python
from persona import Persona
#Suponer que acá están escritas todas las funciones anteriores
persona1 = Persona()

persona1.nombre = "Juan"
persona1.apellido = "Perez"
persona1.anio_nac = 2001

persona2 = Persona ()
persona2.nombre = "Lucia"
persona2.apellido = "Rodriguez"
persona2.anio_nac = 2010

esMayor(persona1, persona2)
familia(persona1,persona2)
```

En este caso las funciones escribirían
```
Juan es la persona más grande
apellidos diferentes
```
