# Funciones
Las funciones son estructuras de código que permiten **modularizar** nuestro código. Es decir, se subdivide un problema en varios subproblemas, y cada subproblema se encararía mediante una función.
<!-- TODO: agregar las imagenes de ayp(la presentacion de apuntes) y funciones -->
Las funciones pueden pensarse de forma coloquial como un "coso" que recibe información, la computa, y retorna un sólo resultado.
<!-- TODO: agregar imagen del coso funcion -->
El uso de una función consta de dos partes: La **definición** y la **invocación**.

<!-- TODO: completar -->
## Definición
La definición es donde programamos el algoritmo de nuestra función. 

## Invocación
La invocación es cuando la función es usada. y puede invocarse las veces que se necesite.
Además, hay distintas funciones predefinidas, estas funciones ya están definidas en p5, y para usarlas sólo es necesario invocarlas (ej: mousePressed, fill, random)

## Utilidad
<!-- TODO: copiar los 3 utilidades de la presnetacion ayp -->

<!-- TODO: posible subseccion? -->
## Parametros 
Una función puede ser definida con parámetros. Los parámetros pueden pensarse como variables que van a tener distinto valor con cada invocación.
Nuestra función nube tiene dos parámetros para posición horizontal y vertical. Y dibujamos nuestros círculos según estos dos parámetros.
Al invocar, primero invocamos con 120 y 90. Así que posH pasa a tener 120 y posV 90. Entonces la nube se dibuja en esa ubicación.
En la segunda invocación los parámetros son otros (50 y 200), entonces se dibuja una segunda nube en esta nueva posición.

