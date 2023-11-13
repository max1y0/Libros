# Hola Mundo
En el mundo de la programación es una costumbre muy conocida para empezar un lenguaje nuevo, hacer un programa que diga "hola mundo"(hello world) por la pantalla.
Por ejemplo:

```assembler
    global _main
    extern _printf

    section .text
_main:
    push message
    call _printf
    add esp, 4
    ret
message:
    db 'Hola Mundo'
```
```c
#include <stdio.h>
int main(void){
    printf("Hola Mundo");
}
```
```java
public class HolaMundo {
    public static void main(){
        System.out.println("Hola mundo");
    }
}
```
```pascal
PROGRAM HolaMundo(output);
BEGIN
    WRITE('hola mundo')
END.
```

En cambio, gracias a que programar en python es más sencillo. El “hola mundo” en este lenguaje es programado así:
```python
print ("hola mundo")

```