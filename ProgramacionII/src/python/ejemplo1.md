# Ejemplo 1
Queremos hacer una función que tomando dos objetos persona, diga el nombre del más grande de los dos.

Esto se puede programar comparando las fechas de nacimiento. El número más chico indica que es más grande. Veamos:
```python
def esMayor(persona1, persona2):
    if (persona1.año_nac < persona2.año_nac):
        print(persona1.nombre + "es la persona más grande")
    else:
        print(persona1.nombre + "es la persona más grande")
```

También podríamos haber usado el método decirEdad para lo mismo:
```python
def esMayor(persona1, persona2):
    if (persona1.decirEdad() > persona2.decirEdad()):
        print(persona1.nombre + "es la persona más grande")
    else:
        print(persona1.nombre + "es la persona más grande")
```
