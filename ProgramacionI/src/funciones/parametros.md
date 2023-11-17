# Parámetros
Una función puede ser definida con parámetros. Los parámetros son los datos que se le ingresan a la función para poder hacer cómputos. 
<!-- TODO: volver a agregar la imagen -->
Estos pueden pensarse como variables que podemos usar dentro de la definición de la función y que van a tener distinto valor con cada invocación. La estructura es como sigue:
```py
def nombre_de_funcion(parametro1, parametro2, ....):
    #codigo que resuelve el subproblema
    return resultado_que_se_retorna #esta instruccion se omite en el caso de que la función no retorne nada.
```
### Ejemplo
Vamos a realizar una función que reciba como dato la edad de una persona, y me devuelva un aproximado de cuantos días pasaron desde que nació hasta la actualidad.

```py
def cantidad_dias (edad):
    resultado = edad * 365
    return edad
```

Y en nuestro algoritmo principal, la podemos invocar de la siguiente mandera

```py
print("Ingresa tu edad")
edad = int( input( ) )
dias = cantidad_dias(edad)

print("La cantidad aproximada de días desde que naciste es, ", dias)
```