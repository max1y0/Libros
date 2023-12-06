# Métodos

Las clases pueden tener los métodos que definimos en los objetos. Esas funcionalidades las “heredan” todos los objetos de esa Clase. Es decir, si la clase Espada tiene el método atacar, todos los objetos de tipo Espada terminan teniendo ese método.

### Ejemplo de la clase persona con los atributos y métodos definidos antes:
```python
clase Persona :
  nombre
  edad
  dni

  metodo decirDatos (propio):
    escribir (“nombre: ”+ propio.nombre + propio.apellido)
    escribir (“dni: ” + propio.dni)
    
  metodo añoNacimiento (propio, añoActual):
    escribir(añoActual - propio.edad)
```

Pero ademas en una definición de clase se define un método extra:
