# Funciones predefinidas y Bibliotecas

En muchas situaciones nos encontramos con que tenemos que realizar las mismas funcionalidades en muchos programas: longitud de un arreglo, buscar en un arreglo, pasar cadena a minúsculas, etc. Si bien la idea de las funciones es la reutalización del código, muchas de estas funciones útiles vienen predefinidas en los lenguajes, listas para ser utilizadas. Para conocerlas, nos basta con visitar la documentación de cada lenguaje e investigar lo que nos haga falta.

### Veamos el siguiente ejemplo

Supongamos que nos piden que realicemos una funcionalidad para un sistema, esta funcionalidad se basa en detectar la seguridad en una contraseña. Nos piden que la contraseña ingresada tiene que tener las siguientes características:

1. La contraseña tiene que ser de 8 caracteres mínimo.
1. La contraseña tiene que tener mínimo 1 número
1. La contraseña tiene que tener mínimo 1 símbolo
1. La contraseña tiene que tener mínimo 2 letras en minúscula
1. La contraseña tiene que tener mínimo 2 letras en mayúsculas.

Para cada una de estas características podemos usar una función predefinida del lenguaje (en este caso python).

* ```islower()``` Nos dice si un caracter es minúscula
* ```isupper())``` Nos dice si un caracter es mayúscula
* ```isdigit())``` Nos dice si un caracter es un número
* ```isalnum())``` Nos dice si un caracter es un número o una letra.

# Bibliotecas

Entonces, por un lado están las funciones predefinidas por el lenguajes, y las funciones definidas por nosotros como programadores. Hay un tercer caso en donde podemos usar funciones definidas por otros programadores.

Estas funciones vienen empaquetadas en lo que se llama biblioteca.

### Ejemplos

1. ```NumPy```: Para cálculos numéricos y manipulación de matrices y arreglos.
1. ```Pandas```: Para manipulación y análisis de datos estructurados en forma de tablas.
1. ```Matplotlib y Seaborn```: Para visualización de datos y creación de gráficos.
1. ```Requests```: Para realizar solicitudes HTTP y trabajar con APIs web.
1. ```Flask y Django```: Para crear aplicaciones web y sitios web.
1. ```TensorFlow y PyTorch```: Para la implementación de aprendizaje profundo y machine learning.
1. ```SQLite3 y SQLAlchemy```: Para trabajar con bases de datos.
