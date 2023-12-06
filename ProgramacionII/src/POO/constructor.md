# El método constructor

Supongamos una clase alumno, podríamos tener el siguiente constructor
```python
metodo constructor (nombre, apellido, dni, anio_ingreso):
    propio.nombre = nombre
    propio.apellido = apellido
    propio.dni = dni
    propio.anio_ingreso = anio_ingreso
```

Si bien la estructura puede no tener mucho sentido, escribir un método constructor permite lo siguiente:

### Sin constructor
```python
alumno1 = Alumno()

alumno1.nombre = "Lucas"
alumno1.apellido = "Russo"
alumno1.dni = 46464646
alumno1.anio_ingreso = 2019
```
### Con constructor
```python
alumno1 = Alumno ("Lucas","Russo",46464646,2019)
```

## Código final
La clase ```Persona``` quedaría de esta forma con todo lo visto:
```python
clase Persona:
  nombre
  edad
  dni

  metodo constructor (nombre, apellido, dni, anio_ingreso):
    propio.nombre = nombre
    propio.apellido = apellido
    propio.dni = dni
    propio.anio_ingreso = anio_ingreso

  metodo decirDatos (propio):
    escribir (“nombre: ”+ propio.nombre + propio.apellido)
    escribir (“dni: ” + propio.dni)
    
  metodo añoNacimiento (propio, añoActual):
    escribir(añoActual - propio.edad)
```