# Ciclo for in
El ciclo ```for``` tiene una variante particular: el ```for in```. A diferencia del anterior, en este no indicamos cuantas veces vamos a repetir, en este indicamos que vamos a repetir **sobre todos los elementos de una lista**. Veamos:
```python
lista = [3,5,1,99]
for numero in lista:
    print(numero)
```
Este código se puede leer de forma coloquial como sigue: "Para cada numero en la lista, hacerle prints". Es decir, el ciclo repite el código ```print(numero)``` en cada elemento de la lista.

Tambien sirve para ciclar sobre cadenas de texto (```strings```):

```python
texto = "hola como estas"
contador = 0
for letra in texto:
    if letra == 'a':
        contador +=1
```

En este caso estamos ciclando por cada letra en la variable ```texto```, si la letra es la 'a', le sumamos a un ```contador``` en 1. Nuestro programa entonces cuenta la cantidad de letras 'a' en la frase.

Las variables que esten entre ```for``` e ```in``` pueden llamarse de cualquier forma. En este caso usamos ```numero``` y ```letra``` solo para que sea entendible.