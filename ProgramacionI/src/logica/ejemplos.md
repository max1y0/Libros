# Ejemplos

> Un amo de casa le indica a su robot asistente lo siguiente:
>
> _Anda a comprar una tira de pan, y si hay bananas trae tres._
>
> Al volver, el robot volvió con tres tiras de pan. Por que?


Algunos ejemplos de proposiciones lógicas pueden ser las siguientes

* Soy de 3ro ```Y``` voy a ProA
* Me gustan los perros ```O``` me gustan los gatos
* Mi edad < 18 ```Y``` puedo comprar alcohol
* Vivo sólo ```O``` estoy casado
* Los gatos ladran ```Y``` los perros cantan ```Y``` los pájaros vuelan
* Estamos en agosto ```Y``` es otoño O es 2029
* Soy chico ```O``` soy chica ```Y``` soy persona
* Duermo parado ```O``` me baño acostado ```O``` camino con las manos

Analicemos algunos:

### Ejemplo 1
```js
Me gustan los perros O me gustan los gatos
------------------------------------------
//en mi caso, prefiero los gatitos sobre los perros asi que el valor de verdad de esta frase es
    F   O   V   
//Si sigo las reglas del operador O, se que:
    V
```

### Ejemplo 2
```js
Soy chico O soy chica Y soy persona 
-----------------------------------------------
//veamos primero la frase Soy chico O Soy chica. Como yo soy chico, es verdadero solo esta parte

    V   O   F   Y   soy persona
//claramente soy persona asi que la frase queda así
    V   O   F   Y   V
//Segun las reglas del O, V O F es V, entonces:
    V   Y   V
//Y segun las reglas del Y:
    V
```
