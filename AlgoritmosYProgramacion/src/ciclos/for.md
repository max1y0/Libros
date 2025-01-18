# Ciclo for

La instrucción que vamos a ver se llama ```for```, es una de las tantas instrucciones repetitivas en el mundo de la programación. Este año nos vamos a centrar solo en esta.

Veamos como traducir las configuraciones del ciclo a una instrucción ```for```.
* Desde cuando empiezo a repetir: 1
* Hasta donde repito: 10
* De cuanto en cuanto avanzo: 1 en 1

```js
for (let i = 1 ; i < 10 ; i += 1){
    //decir hola
}
```
Parece una instrucción compleja pero en realidad, se copia tal cual y se tienen que cambiar sólo algunas cosas.

Para cambiar desde donde empieza a repetir, se cambia el ```1``` por cualquier otro número
```js
    let i = 1
```

Para indicar hasta donde se repite, se cambia acá el número ```10``` (a veces vamos a querer cambiar el signo mayor ```>```, para los casos que querramos hacer una repetición de atrás para adelante)
```js
    i < 10
```

Y para indicar de cuanto en cuanto avanzo, se cambia el ```1``` en este caso. (Si quiero ir hacia atrás, en vez de un más ```+```, va un ```-```)
```js
    i +=1
```

Después, todas las instrucciones que estén dentro de las llaves del ```for```, son las instrucciones que van a ser repetidas.

## Qué es esa i?
```i``` es una variable cualquiera, es decir puede tener cualquier nombre que querramos, normalmente en los ciclos se usa la variable ```i``` porque simboliza ```indice```. En general, las variables que se usan para manejar un ciclo se le llaman variables de control. Y podemos usarlas dentro del ciclo para lo que necesitemos. Como en el siguiente ejemplo.
