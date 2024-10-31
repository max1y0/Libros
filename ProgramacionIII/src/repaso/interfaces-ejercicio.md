# Ejercicio Interfaces
Vamos a usar HTML y CSS para hacer una página simple, a modo de tarjeta de presentación (similar a las plantillas de carrd.co). A modo de contenido vamos a necesitar:
1. __Un título:__ Que va a usarse para el nombre de la persona.
2. __Un subtítulo:__ Una muy breve descripción de la persona
3. __Un párrafo:__ Una descripción más detallada, de igual manera que no supere los 500 caracteres aproximadamente.
4. __Una imagen:__ Puede ser una foto de perfil o una imagen de fondo.
5. __Algunos links o botones:__ Que lleven a redes sociales o páginas personales.

Para la presentación de la página vamos a necesitar:
1. __Un par de fuentes:__ Vamos a usar una tipografía para el título y otra para los textos.
2. __Una paleta de colores:__ Una paleta de colores que sea armoniosa y que vaya con el estilo de la página.
3. __Un layout elegante:__ El layout define como se va a organizar la página en el espacio. Es importante que no se sienta sobrecargada, anticuada, o poco profesional.

<!-- TODO: agregar paso a paso de la actividad?. -->
## HTML
Un posible código para la estructura de nuestra página podría ser el siguiente
```html
<!doctype html>
<html>
    <head>
        <link rel="stylesheet" type="text/css" href="style.css" />
    </head>

    <body>
        <div class="tarjeta">
            <h1 class="titulo">Chaves Maximiliano</h1>
            <h3 class="subtitulo">Profesor en Ciencias de la Computación</h3>
            <img class="perfil" src="profile.png" />

            <p class="descripcion">
                Referente (ojalá) de la programación creativa. Docente
                programación de nivel medio. Hace videos en youtube cada eclipse
                solar. Neurodivergente. Si tiene tiempo juega jueguitos. No
                suele pasar seguido.
            </p>

            <div class="links">
                <a href="www.instagram.com/maxi_chvs">Instagram</a>
                <a href="www.github.com/max1y0">Github</a>
                <a href="mailto:maximiliano.e.chaves@gmail.com">Mail</a>
            </div>
        </div>
    </body>
</html>
```

## CSS
Para el estilo defino mi paleta de colores como:
<!-- Buscar como poner hex colors -->
El estilo lo voy a acomodar en una tarjeta de color blanco que esté al centro de la pantalla. La imagen que esté en formato circular encima de la tarjeta, y la información dentro de la misma. De color de fondo voy a usar un gradiente suave de los colores elegidos de mi paleta.
<!-- Agregar el css -->
