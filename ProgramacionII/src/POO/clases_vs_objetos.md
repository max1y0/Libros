# Clases vs Objetos

Las clases son fábricas de objetos. Normalmente en programación necesitamos varios objetos similares, y definir muchos objetos con los mismos atributos se vuelve tedioso. Para eso se definen clases, donde se escriben los atributos de un objeto y después se crean objetos de esa misma clase

### Objetos
```javascript
persona1 = { 
  nombre: "martin",
  edad: 46
  dni: 26700808
}

persona2 = { 
  nombre: "agus",
  edad: 26
  dni: 46700808
}
...
...
...
persona500 = { 
  nombre: "lore",
  edad: 32
  dni: 34700808
}
```

### Misma idea con clases
```python
class Persona :
  nombre
  edad
  dni

persona1 = Persona ("martin",46,26700808)
persona2 = Persona ("agus",26,46700808)
persona3 = Persona ("lore",32,34700808)
```
## Clases vs Objetos
La clase espada

![Espada clase](images/swordClass.jpg)

Los objetos: espada de madera, de piedra, de hierro, de oro y de diamante.

![Espada objetos](images/sword.png)