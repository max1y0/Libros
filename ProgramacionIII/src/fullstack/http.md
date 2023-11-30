# HTTP
World Wide Web Communication
The World Wide Web is about communication between web clients and web servers.
Clients are often browsers (Chrome, Edge, Safari), but they can be any type of program or device.
Servers are most often computers in the cloud.
<!-- TODO: imagen de secuenciacion -->

HTTP Request / Response
Communication between clients and servers is done by requests and responses:
A client (a browser) sends an HTTP request to the web
A web server receives the request
The server runs an application to process the request
The server returns an HTTP response (output) to the browser
The client (the browser) receives the response

The HTTP Request Circle
A typical HTTP request / response circle:
The browser requests an HTML page. The server returns an HTML file.
The browser requests a style sheet. The server returns a CSS file.
The browser requests an JPG image. The server returns a JPG file.
The browser requests JavaScript code. The server returns a JS file
The browser requests data. The server returns data (in XML or JSON).
XHR - XML Http Request
All browsers have a built-in XMLHttpRequest Object (XHR).
XHR is a JavaScript object that is used to transfer data between a web browser and a web server.
XHR is often used to request and receive data for the purpose of modifying a web page.
The XHR Object is a Web Developers Dream, because you can:
Update a web page without reloading the page
Request data from a server - after the page has loaded
Receive data from a server - after the page has loaded
Send data to a server - in the background

<!-- Imagen de secuenciacion -->



HTTP Methods
GET
POST
PUT
HEAD
DELETE
PATCH
OPTIONS
CONNECT
TRACE
The two most common HTTP methods are: GET and POST.
The GET Method
GET is used to request data from a specified resource.
Note that the query string (name/value pairs) is sent in the URL of a GET request:
/test/demo_form.php?name1=value1&name2=value2
Some notes on GET requests:
GET requests can be cached
GET requests remain in the browser history
GET requests can be bookmarked
GET requests should never be used when dealing with sensitive data
GET requests have length restrictions
GET requests are only used to request data (not modify)
The POST Method
POST is used to send data to a server to create/update a resource.
The data sent to the server with POST is stored in the request body of the HTTP request:
POST /test/demo_form.php HTTP/1.1
Host: w3schools.com

name1=value1&name2=value2

