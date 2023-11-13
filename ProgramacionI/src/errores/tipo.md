# Error de tipo
Este error, es quizá uno de los más comunes pero difíciles de detectar. Recordemos que cada tipo de dato tiene sus propias operaciones, un número se puede sumar, restar, dividir, multiplicar, etc. Y un tipo texto se puede unir, contar, cortar, etc.
¿Qué pasa si, por ejemplo, sin querer intento sumar un dato tipo número con un dato tipo texto?
```
>  TypeError: unsupported operand type(s) for +: 'type1' and 'type2'
```
_*type1 y type2 son dos tipos distintos_

En python nosotros indicamos el tipo de variable poniendo int (número entero) o str (texto) antes de un input.
Si tenemos error de tipo, fijarse bien cómo cargamos bien las variables, y si no es necesario usar otra operación, otro tipo en la carga, o funciones de conversión de tipo
