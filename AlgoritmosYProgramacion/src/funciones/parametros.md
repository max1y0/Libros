# Funciones y Parámetros
Si comparamos nuestra función ```nube()``` contra la función ```rect()``` por ejemplo, podemos notar una diferencia importante. ```rect``` para funcionar necesita datos, números, que indican su posición y tamaño. Nuestra función ```nube``` siempre se dibuja en el mismo lugar, y si queremos dibujar más de una, se dibujan una encima de la otra. Para solucionar esto necesitamos programar usando **parámetros**

## Parámetros
Una función puede ser definida con parámetros. Los parámetros pueden pensarse como variables que van a tener distinto valor con cada invocación.
Nuestra función nube puede dos parámetros, uno para la posición horizontal y vertical. Y dibujamos nuestros círculos según estos dos parámetros.

```js
    function nube(posX, posY){
    fill(140)
    ellipse(posX,posY,50,50)
    ellipse(posX+30,posY+20,50,50)
    ellipse(posX+25,posY-10,50,50)
    ellipse(posX+70,posY+20,50,50)
    ellipse(posX+60,posY,50,50)
}
```
Si al invocarla, lo hacemos de la siguiente manera:
```js
    nube(50,50)
```
Los parámetros ```posX``` y ```posY``` se inicializan en ```50```. Por lo que en la definición, en todos los lugares donde estaba escrito ```posX``` se cambia por ```50```, así como en donde aparecía ```posY```. Entonces, ```nube(50,50)``` dibuja la nube tal como en el ejemplo de [antes](./funciones/funciones.md)

Gracias a los parámetros podemos: invocar la función en distintas posiciones, invocarla más de una vez, o incluso usar variables en los parámetros y hacer que se mueva.

