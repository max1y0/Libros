# Analizando la clase Alumno
```python
Clase Alumno:
    metodo constructor (propio, nombre, apellido, dni, anio_ingreso):
        propio.nombre = nombre
        propio.apellido = apellido
        propio.dni = dni
        propio.anio_ingreso = anio_ingreso

    metodo decirDatos (propio):
        escribir (“nombre: ”+ propio.nombre + propio.apellido)
        escribir (“dni: ” + propio.dni)

    metodo añoQueCursa ( propio, año ):
        escribir(“cursa el año:”, año  - alumno1.año_ingreso)

alumno1 = Alumno ("Lucas","Russo",46464646,2019)

alumno1.decirDatos()

año = 2021
alumno1.añoQueCursa(año)
```

Lo primero que hacemos es crear un objeto de la clase Alumno. Nuestro objeto se llama ```alumno1```. Después rellenamos los atributos de nuestro alumno con información: Lucas Russo, dni 46464646, año de ingreso 2019. 

Al hacer ```alumno1.decirDatos()```, estamos invocando al método ```decirDatos()```, y lo estamos invocando con la información que tiene ```alumno1```. Entonces, en el método, automáticamente se reemplaza donde decía propio, por alumno1. Es decir, ```alumno1.decirDatos()``` imprime lo siguiente:
```
nombre: Lucas Russo
dni: 46464646 
```
En el siguiente segmento de código
```python
año = 2021
alumno1.añoQueCursa(año)
```
El método ```añoQueCursa``` cambia todo los propio por ```alumno1```, y donde decia ```añoActual```, se ingresa la variable ```año```. 
Es decir que se imprime lo siguiente:
```python
cursa el año 4
```
(hace la resta 2023-2019)
