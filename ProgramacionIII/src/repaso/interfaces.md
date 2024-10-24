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
