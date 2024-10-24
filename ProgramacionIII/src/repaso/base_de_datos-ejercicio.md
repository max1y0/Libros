# Ejercicio
La base de datos que vamos a crear modela un sistema básico de pedidos de productos. El sistema permite la carga de clientes y productos a la venta. Además se permite la carga de pedidos, un cliente realiza un pedido y este tiene asociados múltiples productos. Un mismo cliente puede realizar más de un pedido, pero un pedido puede estar asociado a sólo un cliente. Por último un producto puede estar en varios pedidos. Para esto vamos a tener tres entidades: cliente, pedido y producto.

## Diagrama ER
El diagrama de ER según lo visto podría ser el que sigue.

## Álgebra Relacional
Luego, el álgebra relacional es:
```
Cliente (ID_Cliente, Dirección, Nombre, Contacto)
Pedido (ID_Pedido, Fecha, Monto, ID_Cliente)
Producto (ID_Producto, Descripción, Precio)
Tiene (ID_Pedido, ID_Producto)
```

## SQL
El código SQL que surge del álgebra relacional:
```sql
create database pedido;
use pedido;

CREATE TABLE Cliente (
ID_Cliente int(6) PRIMARY KEY NOT NULL UNIQUE AUTO_INCREMENT,
Nombre varchar(15),
Direccion varchar(30),
Contacto varchar(30)
);

CREATE TABLE Pedido (
ID_Pedido int(6) PRIMARY KEY NOT NULL UNIQUE AUTO_INCREMENT,
Fecha date,
Monto int(6),
ID_Cliente int(6),
FOREIGN KEY(ID_Cliente) REFERENCES Cliente(ID_Cliente)
);

CREATE TABLE Producto (
ID_Producto int(6) PRIMARY KEY NOT NULL UNIQUE AUTO_INCREMENT,
Descripción varchar(50),
Precio int(6)
);

CREATE TABLE Tiene (
ID_Pedido int(6),
ID_Producto int(6),
FOREIGN KEY(ID_Pedido) REFERENCES Pedido(ID_Pedido),
FOREIGN KEY(ID_Producto) REFERENCES Producto(ID_Producto)
);

```
