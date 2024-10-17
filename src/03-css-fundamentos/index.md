---
title: "Fundamentos de CSS"
description: "Cap.3 - Fundamentos de CSS"
date: 2024-10-15
series: ["Guía HTML y CSS"]
series_order: 3
build:
  list: never
---


## 3. Fundamentos de CSS
**CSS** (*Cascading Style Sheets*) es un lenguaje de hojas de estilo utilizado para describir cómo se presenta el contenido de un documento **HTML**.

Los fundamentos de **CSS** incluyen la comprensión de su sintaxis, selectores, propiedades y cómo aplicar estilos a los elementos **HTML** para mejorar la apariencia visual de las páginas web.


---

## 3.1 Introducción a CSS

**CSS** permite que los desarrolladores definan la apariencia visual de un sitio web separando la estructura del contenido (**HTML**) del diseño.

Esto facilita la modificación del diseño sin tener que cambiar el contenido de la página.


```html
<!DOCTYPE html>
<html lang = "es">
    <head>
        <meta charset = "UTF-8">
        <meta name = "viewport" content = "width=device-width, initial-scale=1.0">
        <title>Mi Página con CSS</title>
        <style>
            body {
                background-color: #f0f0f0;
                font-family: Arial, sans-serif;
                }
            h1 {color: #333333;}
            p {font-size: 16px; color: #666666;}
        </style>        
    </head>
    <body>
        <h1>Bienvenido a Mi Página</h1>
        <p>Este es un ejemplo de cómo se aplican estilos CSS.</p>
    </body>
</html>
```


### 3.1.1 Sintaxis CSS Básica

La sintaxis de **CSS** consiste en selectores que apuntan a los elementos **HTML** y en reglas que definen los estilos que se aplicarán a esos elementos.

Cada regla **CSS** tiene dos partes:

- **Selector** : Identifica el elemento **HTML** al que se le aplicará el estilo.
- **Bloque de declaración** : Contiene las propiedades **CSS** y sus valores.

```css
h1 {
    color: blue;
    font-size: 24px;
}
```

En este ejemplo, el selector ```h1``` se refiere a los elementos ```h1``` en el **HTML**, y las declaraciones dentro del bloque ```{ }``` definen que el texto de los encabezados será de color azul y tamaño 24 píxeles.

---

## 3.2 Propiedades CSS Comunes

**CSS** tiene una gran cantidad de propiedades que permiten controlar la presentación de los elementos HTML.

A continuación, se mencionan algunas de las propiedades más comunes.

### 3.2.1 Color y Fondos

- **color** : Define el color del texto.
- **background-color** : Establece el color de fondo de un elemento.

```css
p {
    color: red;
}

body {
    background-color: #f0f0f0;
}
```

### 3.2.2 Tipografía

**CSS** ofrece varias propiedades para controlar la apariencia del texto.

- ```font-family``` : Define la fuente utilizada para el texto.
- ```font-size``` : Controla el tamaño del texto.
- ```font-weight``` : Establece el grosor del texto (normal o negrita).

```css
p {
    font-family: Arial, sans-serif;
    font-size: 18px;
    font-weight: normal;
}
```

### 3.2.3 Espaciado

**CSS** proporciona herramientas para controlar el espaciado entre elementos mediante las propiedades ```margin``` y ```padding```.

- ```margin``` : Define el espacio exterior de un elemento (*fuera de su borde*).
- ```padding``` : Define el espacio interior de un elemento (*dentro de su borde*).

```css
h1 {
    margin-bottom: 20px;
}

p {
    padding: 10px;
}
```

---

## 3.3 Modelo de Caja (Box Model)

El modelo de caja es un concepto fundamental en **CSS**, ya que cada elemento en una página web se representa como una caja rectangular.

El **box model** describe el espacio que un elemento ocupa en la página.

**Componentes del Modelo de Caja:**

- **Contenido** : El contenido real del elemento, como texto o imágenes.
- **Relleno (padding)** : El espacio entre el contenido y el borde del elemento.
- **Borde (border)** : El espacio entre el contenido y el borde del elemento.
- **Margen (margin)** : El espacio fuera del borde del elemento, que separa el elemento de los demás.

```css
/* Este código define un div con un ancho de 300 pixeles,
20 pixeles de relleno, un borde de 5 pixeles,
y un margen de 10 pixeles. */
div {
    width: 300px;
    padding: 20px;
    border: 5px solid black;
    margin: 10px;
}
```

---

## 3.4 Diseño (Box Model)

Un aspecto clave del diseño web moderno es que las páginas se adapten a diferentes tamaños de pantalla.

**CSS** incluye herramientas como **media queries** y **flexbox** para hacer que el contenido sea adaptable.

### 3.4.1 Uso de Media Queries

Las **media queries** permiten aplicar diferentes estilos dependiendo del tamaño de la pantalla o del dispositivo.

```css
/*En este ejemplo, el color de fondo cambia a azul
claro cuando el ancho de la pantalla
es de 600 píxeles o menos.*/
@media ❨max-width:600px❩
body: {
    background-color: lightblue;
}
```

---

<div class="footer-nav">
    <a href="../html-fundamentos/">2. Fundamentos de HTML</a>
    <!-- <a href="#" class="prev-link" class="tachado">Anterior</a> -->
    <a href="../estructuracion/" class="next-link">4. Estructuración de Proyectos Web</a>    
</div>