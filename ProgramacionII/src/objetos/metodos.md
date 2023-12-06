# Métodos
Los objetos además de ser una estructura que permite tener varios campos de datos en forma de atributos, podemos diseñar **funcionalidades específicas para cada uno**. Los métodos son como funciones que sólo pueden ser usadas por el objeto. 

Supongamos un objeto espada, un método podría ser:
```
metodo Atacar (propio):
    // acá va el código que la programa
```

Y en nuestro objeto persona, podríamos tener los siguientes métodos
```
metodo decirDatos (propio):
    escribir (“nombre: ”+ propio.nombre + propio.apellido)
    escribir (“dni: ” + propio.dni)
    
metodo añoNacimiento (propio, añoActual):
    escribir(añoActual - propio.edad)
```

### ¿Qué es ese ```propio``` que aparece ahí?

```propio```, sirve para indicar que estamos accediendo a los atributos de __ese mismo objeto que la está usando__. 