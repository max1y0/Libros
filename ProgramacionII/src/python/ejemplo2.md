# Ejemplo 2
Queremos hacer una función que diga “son familiares?” si ambos tienen el mismo apellido.
```python
def familia (persona1, persona2):
    if (persona1.apellido == persona2.apellido):
        print( "son familia?")
    else:
        print("apellidos diferentes")

```