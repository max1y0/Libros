# Estructura Secuencial

La estructura secuencial es una de las estructuras de control básicas en programación y se caracteriza por la ejecución secuencial de instrucciones. Aquí están las características clave de la estructura secuencial:

1. Secuencia de instrucciones: Las instrucciones se ejecutan en un orden específico, de arriba a abajo, una tras otra, sin bifurcaciones ni saltos. La ejecución sigue un flujo lineal.
2. Un solo punto de entrada y salida: La ejecución comienza en un solo punto de entrada y continúa de manera secuencial hasta alcanzar un punto de salida. No hay bifurcaciones ni bucles en la estructura secuencial básica.
4. Fácil lectura y mantenimiento: La estructura secuencial es fácil de leer y comprender, ya que refleja el flujo natural del pensamiento humano. Esto facilita el mantenimiento y la depuración del código.
5. Instrucciones ejecutadas una única vez: Cada instrucción dentro de la estructura secuencial se ejecuta exactamente una vez. No hay ciclos o repeticiones automáticas en esta estructura básica.
6. Aplicación de operaciones básicas: Las instrucciones dentro de la estructura secuencial suelen consistir en operaciones primitivas.
7. Simplicidad estructural: La estructura secuencial es la más simple de todas las estructuras de control. Aunque es limitada en términos de control de flujo, es esencial para construir bloques fundamentales de lógica en programas.

## Variables

Las variables son espacios de memoria en el sistema de almacenamiento principal (RAM) que contienen un nombre simbólico. Se utilizan para guardar los datos de los programas.

### Tipos de datos
Es un conjunto de valores posibles y las operaciones que se usan para manipularlos.
Tipos de datos en python:
* Simples
  * Enteros
  * Reales
  * Booleanos
* Compuestos
  * Dinámicos:
    * Listas
    * Diccionarios
    * Conjuntos
  * Estáticos:
    * Strings
    * Tuplas

## Primitivas a usar
### Asignación:
El objetivo de la asignación es cambiar el valor almacenado en una variable

```py
x = e
```
guarda en x, el valor de e.

_sintaxis:_
```
<variable> = <expresión>
```

> Una expresión es una combinación de constantes, variables o funciones, que es interpretada de acuerdo a las normas particulares de precedencia y asociación para un lenguaje de programación en particular. Una expresión evaluada da como resultado un valor.

### Entrada de datos:
```py
x = input()
```
Guarda en x un valor ingresado por teclado en la terminal

_sintaxis:_
```
<variable> = input(<texto informativo al usuario>)
```
### Salida de datos:
```py
print(e)
```
Informa por terminal el valor de ```e```. ```e``` puede ser un conjunto de variables, o una expresión.

_sintaxis:_
```
print(<expresion>,<variable/s>)
```
