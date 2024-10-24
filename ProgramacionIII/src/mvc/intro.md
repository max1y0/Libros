# Model View Controller

El Modelo Vista Controlador (MVC)es un patrón de arquitectura de software, que separa los datos, la lógica y la presentación. MVC divide en tres componentes: el modelo, la vista y el controlador.

### Modelo
Es la representación de la información del sistema. Normalmente está relacionado con la base de datos de nuestra aplicación. Desde el **controlador** se envía la petición de acceso o modificación de información. El modelo envía a la **vista** aquella información que sea solicitada para ser mostrada.

### Vista
Es la interfaz de usuario. Además muestra la información del **modelo** y envía la interacción del usuario al **controlador**. En nuestro trabajo, estos fueron los archivos HTML y CSS

### Controlador
El controlador es un intermediario entre la vista y el controlador. Maneja la interacción del usuario, actualiza el modelo de forma acorde, y actualiza la vista con los cambios que se hicieran al modelo. Normalmente esta relacionado a nuestros archivos python.

<!--TODO IMAGEN -->

## Flujo de comunicación entre componentes
1. El usuario interactúa con la vista (clickeando un botón, entrando un texto)
1. La vista recibe la entrada, y la envía al controlador
1. El controlador recibe la entrada de la vista, la interpreta, ejecuta las operaciones y decide como seguir.
1. El controlador actualiza el modelo basado en la interacción del usuario o la lógica del sistema.
1. El modelo notifica a la vista si hacemos cambios.
1. La vista solicita al modelo los posibles cambios para modificar la interfaz.
1. El controlador actualiza a vista

<!-- imagen secuenciacion (hacer una propia?) -->


### Ejemplo simplificado de una interacción para un carrito de compras
1. El usuario interactua con la interfaz y clickea comprar (agregar a carrito)
2. El controlador recibe la actualización de la vista
3. El controlador notifica el modelo para agregar el item
4. El modelo retorna los nuevos datos al controlador, y actualiza la vista
