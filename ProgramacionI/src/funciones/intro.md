# Funciones
Las funciones son estructuras de código que permiten **modularizar** nuestro código. Es decir, se subdivide un problema en varios subproblemas, y cada subproblema se encararía mediante una función.
<!-- TODO: agregar las imagenes de ayp(la presentacion de apuntes) y funciones -->
Las funciones pueden pensarse de forma coloquial como un "coso" que recibe información, la computa, y retorna un sólo resultado. 

_En algunos casos una función puede no retornar ningún valor, en computación en realidad este tipo de estructura se llama procedimiento._
<!-- TODO: agregar imagen del coso funcion -->
El uso de una función consta de dos partes: La **definición** y la **invocación**.

<!-- TODO: completar -->
## Definición
La definición es donde programamos el algoritmo de nuestra función. La estructura es la siguiente
```py
def nombre_de_funcion():
    #codigo que resuelve el subproblema
    return resultado_que_se_retorna #esta instruccion se omite en el caso de que la función no retorne nada.
```

## Invocación
La invocación es cuando la función es usada. y puede invocarse las veces que se necesite. Para invocarla se escribe sólo el nombre de la función en donde sea necesaria usarla en el algoritmo principal.

```py
print(nombre_de_funcion()) 
#en este caso usamos el valor que devuelve la función para mostrarlo por terminal
```

### Ejemplo
Vamos a realizar una función que imprima por pantalla una cuenta regresiva del 10 al 0. (Esta función no va a retornar ningún valor)
```py
#definición
def cuenta_regresiva():
    print( "Iniciando cuenta regresiva..." )
    for i in range( 10 ):
        print( 10 - i )
    print( "DESPEGUE!" )

print ( "bienvenido al sistema" )
#invocación
cuenta_regresiva()
```

## Utilidad
La utilidad de las funciones se ve resumida en tres características:
1. **Encapsular funcionamiento:**

Todas las instrucciones de un programa que pertenezcan lógicamente a un solo trabajo o a un solo subproblema, pueden encapsularse mediante una función.

2. **Evitar la repetición de código:**

Si en más de una ocasión en nuestro programa tenemos que repetir el mismo set de instrucciones, podemos evitar la repetición haciendo una función con nuestro set de instrucciones e invocar dicha función más de una vez.

3. **Reusar y compartir código:**

Una vez que tenemos una función en un programa podemos reutilizarla en otro sin necesidad de volver a escribirla. De la misma manera podemos compartirlas con otros programadores.

<!-- TODO: posible subseccion? -->
## Parametros 
Una función puede ser definida con parámetros. Los parámetros pueden pensarse como variables que van a tener distinto valor con cada invocación.
Nuestra función nube tiene dos parámetros para posición horizontal y vertical. Y dibujamos nuestros círculos según estos dos parámetros.
Al invocar, primero invocamos con 120 y 90. Así que posH pasa a tener 120 y posV 90. Entonces la nube se dibuja en esa ubicación.
En la segunda invocación los parámetros son otros (50 y 200), entonces se dibuja una segunda nube en esta nueva posición.

