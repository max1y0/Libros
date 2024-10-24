# HTTP
Como dijimos en la sección anterior, la comunicación entre clientes y servidores se hace a través de **requests** y **respondes** (solicitudes y respuestas respectivamente).

HTTP (Hypertext Transfer Protocol) es el protocolo de comunicación de cliente y servidor de la World Wide Web. Cada vez que una persona navega por internet está usando HTTP implícitamente para transferir textos, imágenes y otros archivos multimedia a través de la web.

## Interacción cliente-servidor
|Cliente | Servidor |
|----|----|
|El cliente envía una **solicitud HTTP** | |
| |El servidor recibe la solicitud|
| |El servidor ejecuta una aplicación para resolver la solicitud |
| |El servidor retorna una **respuesta HTTP** al cliente |
| El cliente recibe la respuesta | |
| El cliente procesa la respuesta y se muestra | |

## Métodos HTTP
* ```GET```
* ```POST```
* ```PUT```
* ```HEAD```
* ```DELETE```
* ```PATCH```
* ```OPTIONS```
* ```CONNECT```
* ```TRACE```

Los métodos más comunes son ```GET``` y ```POST```

### El método GET
GET es usado para solicitar datos desde un recurso específico.
La cadena de solicitud es enviada en la URL de la página:
```/test/demo_form.php?name1=value1&name2=value2```

### El método POST
Post es usado para enviar información al servidor o crear/actualizar un recurso.
La información enviada con un POST es guardada en el cuerpo de la solicitud HTTP.
```
POST /test/demo_form.php HTTP/1.1
Host: test.com

name1=value1&name2=value2
```
