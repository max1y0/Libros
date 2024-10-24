# Ejercicio Programación Orientada a Objetos
Vamos a usar POO para hacer un sistema de gestión de tareas. Vamos a poder generar una tarea, modificar una tarea o eliminarla. Una tarea va a consistir en una descripción, una prioridad, y una fecha límite. No se va a entrar en detalle de la implementación ya que es algo que se fue trabajando durante todo el año anterior.

## Clase tarea
Para resolver el problema podemos modelar una clase tarea según lo especificado. Los **atributos** de la tarea entonces podrían ser:
* ```Descripción``` Atributo para indicar el texto de la tarea en sí, la actividad a realizar
* ```Prioridad``` La prioridad es un atributo que puede ser: Alta, Media, Baja.
* ```Fecha límite``` Define la fecha en la que la actividad debería ser completada como límite
* ```Completada``` Este último campo de tipo booleano, que sirva para indicar si la tarea ya se realizó o está pendiente.

Además necesitamos definir los **métodos**. Podríamos en un principio considerar los siguientes:
* ```Completar``` Cambia el atributo completada a verdadero
* ```Agregar descripción``` Modifica la descripción según un parámetro
* ```Cambiar prioridad``` Modifica la prioridad por otra
* ```Asignar fecha límite``` Modifica la fecha límite
* ```En deuda?``` Retorna verdadero o falso si la tarea debería haberse completado para la fecha actual

> NOTA: Se podría discutir que los primeros métodos no son necesarios, y podría modificar los atributos directamente, pero se considera una buena práctica usar métodos que modifiquen los atributos y que el usuario no tenga porqué conocer la estructura de nuestro objeto. De todas maneras, en el alcance de nuestra materia, no considero obligatorio usar métodos para modificar los atributos.

## Algoritmo principal
Podemos pensar al algoritmo principal alrededor del menú de opciones posibles:
```
1. Cargar tarea
2. Modificar tarea
3. Eliminar tarea
4. Completar tarea
5. Ver tareas
6. Ver tareas completadas
7. Ver tareas pendientes
```
Para administrar las tareas necesitamos usar una lista. La lista va a contener objetos de la clase Tarea.

## Programando

Empecemos por la clase y sus atributos (con el método constructor)
```py
class Tarea:
    def __init__(self, descripcion,prioridad,fecha):
        self.descripcion = descripcion
        self.prioridad = prioridad
        self.fecha = fecha
        self.completada = False
```
```completada``` se inicializa en falsa, ya que al crear una tarea se asume no completada.

Creemos los métodos:
```py
def completar(self):
  self.completada = True

def set_descripcion (self, descripcion):
    self.descripcion = descripcion

def set_prioridad (self, prioridad):
    self.prioridad = prioridad.lower()

def set_fecha (self, fecha):
    self.fecha = fecha

def en_deuda (self):
    if self.fecha > datetime.now():
        return True
    else:
        return False

# El método __str__ es un método que nos permite agregar la funcionalidad del print a nuestro objeto.
def __str__(self):
    return f""" Tarea
        ----------
        {self.descripcion}
        fecha: {self.fecha}
        prioridad: {self.prioridad}
        """
```

Vamos al código principal, inicialicemos la lista y generemos el menú de opciones
```py
tareas = []
opcion = 1
while opcion != 0:
    print ("""   ---- Menu de Opciones ----
            1. Cargar tarea
            2. Modificar tarea
            3. Eliminar tarea
            4. Completar tarea
            5. Ver tareas
            6. Ver tareas completadas
            7. Ver tareas pendientes
            0. Salir
            """)
    opcion = int( input() )
```

Encaremos primero las opciones de Alta, Baja y Modificacion:
```py
if opcion == 1:
    descripcion = input( "Ingrese la descripción de su tarea\n" )
    prioridad = input ( "Ingrese la prioridad de su tarea: alta/media/baja\n" )
    str_fecha = input ("Ingrese la fecha en el siguiente formato dd-mm-aaaa")
    fecha = datetime.datetime.strptime(str_fecha, "%d-%m-%Y")

    tarea = Tarea(descripcion,prioridad,fecha)
    tareas.append(tarea)

elif opcion == 2:
        if not tareas:
            print("No hay tareas disponibles para modificar.")
            continue

        for i, tarea in enumerate(tareas):
            print(f"{i}: {tarea}")

        index = int(input("Ingrese el índice de la tarea que desea modificar: "))
        if 0 <= index < len(tareas):
            sub_opcion = 1
            while sub_opcion != 0:
                print("""Ingrese qué desea modificar:
                        1. Descripción
                        2. Fecha
                        3. Prioridad
                        0. Salir
                        """)
                sub_opcion = int(input("Seleccione una opción: "))
                if sub_opcion == 1:
                    nueva_descripcion = input("Ingrese la nueva descripción: ")
                    tareas[index].set_descripcion(nueva_descripcion)
                elif sub_opcion == 2:
                    str_fecha = input("Ingrese la nueva fecha en el siguiente formato dd-mm-aaaa: ")
                    fecha = datetime.datetime.strptime(str_fecha, "%d-%m-%Y")
                    tareas[index].set_fecha(fecha)
                elif sub_opcion == 3:
                    nueva_prioridad = input("Ingrese la nueva prioridad (alta/media/baja): ")
                    tareas[index].set_prioridad(nueva_prioridad)
        else:
            print("Índice inválido.")

elif opcion == 3:
    if not tareas:
        print("No hay tareas disponibles para eliminar.")
        continue

    for i, tarea in enumerate(tareas):
        print(f"{i}: {tarea}")

    index = int(input("Ingrese el índice de la tarea a eliminar: "))
    if 0 <= index < len(tareas):
        tareas.pop(index)
        print("Tarea eliminada.")
    else:
        print("Índice inválido.")

```

Nos quedan las opciones de listado
```py
    elif opcion == 4:
        if not tareas:
            print("No hay tareas disponibles para completar.")
            continue

        for i, tarea in enumerate(tareas):
            print(f"{i}: {tarea}")

        index = int(input("Ingrese el índice de la tarea a completar: "))
        if 0 <= index < len(tareas):
            tareas[index].completar()
            print("Tarea completada.")
        else:
            print("Índice inválido.")

    elif opcion == 5:
        for i, tarea in enumerate(tareas):
            print(f"{i}: {tarea}")

    elif opcion == 6:
        for i, tarea in enumerate(tareas):
            if tarea.completada:
                print(f"{i}: {tarea}")

    elif opcion == 7:
        for i, tarea in enumerate(tareas):
            if not tarea.completada:
                print(f"{i}: {tarea}")

    elif opcion == 0:
        print("Saliendo del programa.")
    else:
        print("Opción no válida.")
```
