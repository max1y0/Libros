# Bases de Datos

Una base de datos es una colección organizada de datos que se accede a través de un sistema de gestión de bases de datos.

Un sistema de gestión de bases de datos es un software que permite definir, crear, mantener y controlar bases de datos.

El tipo de bases de datos visto el año pasado es el relacional.

## Bases de datos relacionales
Una base de datos relacional organiza los datos en tablas con columnas y filas, con una clave que identifica cada fila. Cada fila se llama tupla o registro, y cada columna se denomina atributo.

Normalmente una tabla representa a una **entidad**. Una entidad puede pensarse como una representación lógica de un objeto, concepto, sujeto, etc. Las columnas de la tabla representan los **atributos** de la entidad, estos son sus características o propiedades. Mientras que las filas de una tabla representan **instancias** de dicha entidad.

Por ejemplo: Si tenemos una tabla persona, podemos pensar sus atributos como el nombre, su DNI, su apellido, y cualquier otro dato relevante para el problema.

| Nombre   | DNI      | Edad |
|----------|----------|------|
| Eloisa   | 6543543  | 67   |
| Filanor  | 4988766  | 76   |
| Valdomiro| 4657981  | 76   |

Mientras que las filas que rellenan la tabla representan instancias de personas (la instancia Eloisa, Filanor, Valdomiro)

Además, las tablas pueden representar relaciones. Las relaciones son tablas que enlazan información entre dos entidades diferentes.

## Diagramas de entidad relación
Para diseñar las bases de datos relacionales se puede hacer uso de los Diagramas de Entidad Relación. Estos diagramas representan las entidades, atributos y relaciones de forma gráfica para luego ser descritas en el Software de Gestión de Bases de Datos.

Las entidades se representan con un rectángulo. Los atributos como elipses, estos elipses se desprenden de la entidad a la que representan. Las relaciones se representan con un rombo, y unen con flechas dos entidades.
### Cardinalidad
Las entidades pueden estar relacionadas entre si con distinta **cardinalidad**, esta representa el número de instancias de una entidad que pueden estar relacionadas con el número de instancias de otra entidad.
Las relaciones pueden tener tres tipos de cardinalidades:
1. ```Relación de 1 a n de la entidad A a B ```: Una instancia de la entidad A se relaciona con muchas de la entidad B
2. ```Relación de n a m de la entidad A a B ```: ```n``` instancias de la entidad A se relaciona con ```m``` de la entidad B
3. ```Relación de 1 a a de la entidad A a B ```: Una instancia de la entidad A se relaciona con sólo una de la entidad B

Por ejemplo:
<!-- Agregar imagen de diagrama ER-->

## Tabulación
Tabular es la técnica de pasar de un Diagrama ER a un conjunto de tablas relacionales.

### Tabular Entidades
Se crea una tabla por cada entidad en el diagrama, ésta tiene una columna por cada atributo simple de la entidad, y debe tener una clave primaria que se corresponde con la clave de la entidad.

| Clave | Atributo2 | ... | Atributo1 |
|---------|-----------|-----|-----------|
|     |    |   | |
|    |    |   | |

### Tabular relaciones n a m
Se crea una tabla (relación) por cada relación, esta tabla va a contener
como columnas a los atributos claves de las entidades que esta relacionando

Su clave primaria va a ser la
combinación de las claves de las tablas que relaciona.

* Entidad 1:

| ClaveE1 | Atributo2 | ... | AtributoN |
|---------|-----------|-----|-----------|
|     |    |   | |
|    |    |   | |

* Relación:

| ClaveE1 | ClaveE2 |
|-----------|-----------|
|     |    |
|    |    |

* Entidad 2:

| ClaveE2 | Atributo2 | ... | AtributoN |
|---------|-----------|-----|-----------|
|     |    |   | |
|    |    |   | |

### Relaciones de 1 a n
No agregan una nueva tabla, lo que se hace es agregar en la relación del lado del ```n```, el o los atributos claves de la relación del lado del ```1```,

Estos atributos pasan a ser claves foráneas de la relación del lado del ```n```.

* Entidad 1:

| ClaveE1 | Atributo2 | ... | AtributoN |
|---------|-----------|-----|-----------|
|     |    |   | |
|    |    |   | |

* Entidad 2:

| ClaveE2 | Atributo2 | ... | ClaveE1 |
|---------|-----------|-----|-----------|
|     |    |   | |
|    |    |   | |

### Relaciones 1 a 1
No agregan una nueva tabla, lo que se hace es agregar en una de las tablas, el o los atributos claves de la otra.
Estos atributos pasan a ser claves foráneas de la relación.

* Entidad 1:

| ClaveE1 | Atributo2 | ... | AtributoN |
|---------|-----------|-----|-----------|
|     |    |   | |
|    |    |   | |

* Entidad 2:

| ClaveE2 | Atributo2 | ... | ClaveE1 |
|---------|-----------|-----|-----------|
|     |    |   | |
|    |    |   | |


# SQL
El Lenguaje de Consultas Estructuradas (Structured Query Language), es un lenguaje diseñado para crear, adminsitrar y recuperar información de bases de datos de tipo relacional.

SQL consiste en tres subtipos de lenguajes:
1. Lenguaje de definición de datos
2. Lenguaje de manipulación de datos
3. Lenguaje de control de datos

## Lenguaje de Definición de datos

### Create Table
Instrucción para crear una tabla/relación
```sql
CREATE TABLE nombre (
	columna1 tipodedato,
	columna2 tipodedato,
	columna3 tipodedato,
   ....
);
```

### Drop Table
Elimina una tabla
```sql
DROP TABLE nombre;
```

### Alter Table
Permite modificar las tablas de distintas formas:

* Agregar un atributo nuevo
```sql
ALTER TABLE nombre
ADD nombre_de_columna tipodedato;
```

* Cambiar el nombre de un atributo
```sql
ALTER TABLE nombre
RENAME COLUMN nombre_antiguo to nuevo_name;
```
* Elimina un atributo de la tabla
```sql
ALTER TABLE nombre
DROP COLUMN nombre_de_columna;
```

### Restricciones
Las restricciones son reglas que se aplican a una o más columnas, para hacer un control sobre los datos que se ingresan en esos atributos.

* ```NOT NULL```: No permite un valor nulo en la columna.
* ```UNIQUE```: Dice que todos los valores en la columna deben ser únicos.
* ```PRIMARY KEY```: Identifica a un campo como clave primaria de la tabla.
* ```FOREIGN KEY```: Especifica un campo como clave foránea de otra tabla.
* ```CHECK```: Valida los datos de la columna para que cumplan una condición
* ```DEFAULT```: Especifica un valor de fábrica si el usuario no le asigna ninguno

## Lenguaje de Manipulación de Datos

### Select
Permite consultar los datos almacenados en una Base de Datos
```sql
SELECT [{ALL|DISTINCT}]
    <nombre_campo>[, <nombre_campo>...]

FROM {<nombre_tabla>|<nombre_vista>}[,
    {<nombre_tabla>|<nombre_vista>}...]

[WHERE <condición> [{AND|OR} <condición>...]]

[GROUP BY <nombre_campo>[, <nombre_campo>...]]

[HAVING <condición> [{AND|OR} <condición>...]]

[ORDER BY {<nombre_campo>|<indice_campo>} [{ASC|DESC}][,
    {<nombre_campo>|<indice_campo>} [{ASC|DESC}]]];
```
### Insert
Agrega uno o más registros a una tabla.
```sql
INSERT INTO
    tabla(columnaA, [columnaB, ...])
VALUES
    ('valor1', ['valor2', ...]);
```
```sql
INSERT INTO tabla VALUES ('valor1', 'valor2'); --Respetando el orden de los atributos
```
### Update
Modifica los valores de un registro ya existente
```sql
UPDATE My_table SET field1 = 'updated value' WHERE field2 = 'N';
```

### Delete
Borra registros de una tabla
```sql
DELETE FROM tabla WHERE columna1 = 'valor1';
```
## Joins
La clausula JOIN es usada para combinar filas de dos o mas tablas, teniendo en cuenta una columna relacionada entre ambas

```sql
SELECT Pedido.ID, Pedido.descripcion, Cliente.Apellido
FROM Pedido INNER JOIN Cliente
ON Pedido.ID_cliente = Cliente.ID_cliente;
```
### Inner Join
Retorna los registros que tienen matches en ambas tablas.

TODO Imagen
### Left Join
Retorna todos los registros de la tabla de la izquierda y los registros que matchean de la tabla de la derecha.

### Right Join
Retorna todos los registros de la tabla de la derecha y los registros que matchean de la tabla de la izquierda.

TODO imagen
### Full Join
Retorna todos los registros cuando hay un match ya sea en la tabla izquierda o derecha
TODO imagen
