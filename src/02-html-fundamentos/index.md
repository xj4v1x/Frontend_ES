---
title: "Fundamentos de HTML"
description: "Cap.2 - Fundamentos de HTML"
date: 2024-10-15
series: ["Guía HTML y CSS"]
series_order: 2
build:
  list: never
---


## 2. Fundamentos de HTML
**HTML** es el lenguaje de marcado utilizado para crear la estructura básica de las páginas web.

Los fundamentos de **HTML** incluyen la comprensión de cómo está organizada la información en un documento **HTML**, las etiquetas más comunes y cómo utilizarlas para crear contenido legible y bien estructurado.

---

## 2.1 Estructura de un Documento HTML

Todo documento **HTML** sigue una estructura específica que es interpretada por los navegadores para mostrar el contenido correctamente.

A continuación, se describe la estructura básica de un documento **HTML**:

- ```<!DOCTYPE html>``` : Informa al navegador que está utilizando **HTML5**.
- ```<html>``` : Es el elemento raíz que contiene todo el contenido de la página.
- ```<head>``` : Contiene metadatos sobre el documento, como el título, enlaces a hojas de estilo y otras configuraciones que no son visibles directamente en la página.
- ```<body>``` : Contiene todo el contenido visible de la página, como texto, imágenes y enlaces.

Ejemplo de Estructura Básica de un Documento HTML:
```html
<!DOCTYPE html>
<html lang = "es">
    <head>
        <meta charset = "UTF-8">
        <meta name = "viewport" 
        content = "width=device-width, initial-scale=1.0">
        <title>Mi Sitio Web</title>
    </head>
    <body>
        <h1>Título Principal</h1>
        <p>Contenido de la página.</p>
    </body>
</html>
```
---

### 2.1.1 Elementos y Etiquetas HTML
**HTML** está compuesto por elementos que se definen mediante etiquetas.

Las etiquetas pueden definir bloques de contenido como títulos, párrafos, enlaces, imágenes, etc.

Las etiquetas más comunes incluyen:

- ```<h1>``` a ```<h6>``` : Encabezados que representan diferentes niveles de títulos. ```<h1>``` es el nivel más importante y ```<h6>``` el menos importante.
- ```<p>``` : Define un párrafo de texto.
- ```<a>``` : Define un enlace.
- ```<img>``` : Inserta una imagen en la página.

```html
<body>
    <h1>Título Principal</h1>
    <h2>Subtítulo</h2>
    <p>Este es un párrafo.</p>
    <a href = "https://www.ejemplo.com">Visita nuestro sitio</a>
    <img src = "imagen.jpg" alt="Descripción de la imagen">
</body>
```

---

### 2.1.2 Atributos HTML

Las etiquetas **HTML** pueden tener atributos que proporcionan información adicional sobre el elemento.

Los atributos se colocan dentro de la etiqueta de apertura y siempre tienen un valor asignado.

A continuación, algunos atributos comunes:

- ```href``` : Se utiliza en los enlaces ```<a>``` para especificar la URL a la que apunta el enlace.
- ```src``` : Especifica la ubicación de una imagen en la etiqueta ```<img>```.
- ```alt``` : Proporciona texto alternativo para las imágenes, útil para accesibilidad y SEO.
- ```id``` y ```class``` : Se utilizan para identificar elementos individualmente (```id```) o agruparlos en clases (```class```) para aplicarles estilos **CSS** o interactuar con **JavaScript**.

---

## 2.2 Trabajo con Texto

**HTML** proporciona varias etiquetas para trabajar con texto. Algunas de las más comunes son:

### 2.2.1 Encabezados

**HTML** tiene seis niveles de encabezados, que van desde ```<h1>``` hasta ```<h6>```.

El encabezado ```<h1>``` se utiliza para el título principal de la página, y los encabezados menores se utilizan para subtítulos y secciones.

```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
<h3>Encabezado de tercer nivel</h3>
```

### 2.2.2 Párrafos

Los párrafos se definen con la etiqueta ```<p>``` y se utilizan para agrupar bloques de texto.

```html
<p>Este es un párrafo de ejemplo</p>
```

### 2.2.3 Énfasis y Énfasis Fuerte

Para resaltar texto en **HTML**, se utilizan las etiquetas ```<em>``` y ```<strong>``` :

- ```<em>``` : Se utiliza para enfatizar texto, mostrándolo generalmente en cursiva.
- ```<strong>``` : Se utiliza para dar mayor importancia al texto, mostrándolo en negrita.

```html
<p><em>Este texto está enfatizado</em></p>
<p><strong>Este texto es importante</strong></p>
```

---

## 2.3 Enlaces y Navegación

Los enlaces son fundamentales para la navegación entre páginas web.

Se crean con la etiqueta ```<a>``` y el atributo ```<href>```, que indica la URL de destino.

### 2.3.1 Enlaces Internos y Externos

- **Enlaces internos** : Son aquellos que redirigen a secciones dentro de la misma página o a otras páginas del mismo sitio web.
- **Enlaces externos** : Redirigen a sitios web externos.

```html
<a href = "#seccion1">Ir a la Sección 1</a>
<a href = "https://www.google.com"> target = "_blank">Visitar Google</a>
```

---

## 2.4 Imágenes y Multimedia

**HTML** también permite la inserción de imágenes y contenido multimedia, lo que mejora la experiencia del usuario.

### 2.4.1 Insertar Imágenes

La etiqueta ```<img>``` se utiliza para insertar imágenes. Algunos atributos importantes incluyen:

- ```src``` : Define la ubicación de la imagen.
- ```alt``` : Proporciona una descripción alternativa de la imagen.
- ```width``` y ```height``` : Controlan el tamaño de la imagen.

```html
<img src = "imagen.jpg" alt = "Descripción de la imagen" width = "300" height = "200">
```

---

<div class="footer-nav">
    <a href="../01-html-css-guide/index.md">1. Introducción a HTML y CSS</a>
    <!-- <a href="#" class="prev-link" class="tachado">Anterior</a> -->
    <a href="../03-css-fundamentos/index.md">3. Fundamentos de CSS</a>    
</div>
