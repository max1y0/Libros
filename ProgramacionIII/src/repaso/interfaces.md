# Interfaces con HTML y CSS

## HTML
El Lenguaje de Marcado de Hiper Texto (HyperText Markup Language) es el componente más básico de la web. Es un lenguaje de describe el contenido  y la estructura de una página.

Para estructurar una página se hacen uso de las etiquetas html, que indican qué tipo de contenido se está mostrando. Algunas etiquetas son ```<head>```, ```<title>```, ```<body>```, ```<header>```, ```<footer>```, ```<p>```, ```<div>```, ```<span>```, ```<img>```, entre muchas otras.

Algunas etiquetas pueden tener formatos particulares para describir el contenido de esta, pero generalmente se escribe de la siguiente manera:
```html
<etiqueta>
    contenido
</etiqueta>
```

## CSS
Las Hojas de Estilo de Cascada (Cascading Style Sheet), es otro lenguaje descriptivo usado para indicar la presentación de los documentos HTML.
Es decir, así como HTML se encarga de **qué** vamos a mostrar en una página, CSS se encarga del **cómo**.

Para poder describir la presentación de un archivo html se necesita indicar qué elemento vamos a "decorar". Si es una etiqueta de html, se escribe como sigue:
```css
etiqueta {
  propiedad: valor;
}
```
En el caso de aplicar estilo a una clase descrita en el HTML, se especifica de la siguiente manera:

```css
.clase {
  propiedad: valor;
}
```

## Interfaces
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
