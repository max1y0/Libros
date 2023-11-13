# Error de indentación
Error de indentación
Este error no lo tienen muchos lenguajes, dado que python indica qué instrucción está dentro o no de un bloque según la indentación (sangría) que esa instrucción tiene.
Cuando el intérprete detecta una indentación incorrecta, nos indica algunos de los siguientes errores:
```
>  IndentationError: expected an indented block
```
```
>  IndentationError: unindent does not match any outer indentation level
```

## Entonces, ¿Qué hacer ante este error?
En el primer caso, es que el intérprete esperaba una línea indentada y no la encontró, así que es probable que nos olvidamos de darle la sangría correcta.
En el segundo es cuando las indentaciones no son consistentes, con diferente cantidad de espacios dentro del mismo bloque.
