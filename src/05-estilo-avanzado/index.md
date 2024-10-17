---
title: "Diseño y Estilo Avanzado"
description: "Cap.5 - Diseño y Estilo Avanzado"
date: 2024-10-15
series: ["Guía HTML y CSS"]
series_order: 5
build:
  list: never
---


## 5. Diseño y Estilo Avanzado
En esta sección se abordarán conceptos avanzados de **CSS** que permiten crear diseños más sofisticados y con un mayor control sobre la apariencia de una página web.

Abarcaremos temas como el uso de fuentes externas, efectos visuales, y el diseño con **CSS Grid** y **Flexbox**.

---

## 5.1 Fuentes Web y Tipografía Avanzada

El uso adecuado de fuentes y tipografía es esencial para mejorar la estética y la legibilidad de un sitio web.

**CSS** permite personalizar todos los aspectos relacionados con el texto y las fuentes.


### 5.1.1 Uso de Fuentes Externas (Google Fonts)

Las fuentes externas permiten incluir tipografías que no están instaladas en el sistema del usuario.

Una de las opciones más populares es **Google Fonts**, que ofrece una amplia variedad de tipografías gratuitas.

Ejemplo de Uso de **Google Fonts**:

1. Selecciona una fuente en Google Fonts
2. Copia el enlace proporcionado en el <head> de tu archivo HTML.
    
    `<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">`
3. Aplica la fuente a tu **CSS**.

    `body { font-family: 'Roboto', sans-serif; }`


### 5.1.2 Técnicas de Tipografía Web

**CSS** ofrece muchas propiedades para controlar la tipografía:

- `font-family` : Define la familia de fuentes para el texto.

    `body { font-family: 'Arial', sans-serif; }`

- `font-size` : Controla el tamaño de la fuente. Se pueden usar unidades como `px`, `em`, `rem`, `%`, etc.

    `h1 { font-size: 2em; /* Tamaño relativo */ }`

- `font-weight` : Define el grosor del texto (`normal`,`bold`, etc.).

    `h1 { font-weight: bold; }`


---

## 5.2 Estilos Avanzados de Fondo

**CSS** permite aplicar fondos complejos a elementos, incluyendo imágenes, gradientes, y más.

### 5.2.1 Gradientes

Los gradientes permiten aplicar transiciones suaves entre dos o más colores.

Existen dos tipos principales de gradientes: lineales y radiales.

- Gradiente Lineal

    ```css
    background: linear-gradient(to right, #1E2024 50%, #d87093);
    ```

- Gradiente Radial

    ```css
    background: radial-gradient(circle, #d87093 50%, #1E2024 80%);
    ```

### 5.2.2 Imágenes de Fondo

Las imágenes de fondo se aplican mediante la propiedad `background-image`.

Es posible controlar cómo se repite, su tamaño y su posición.

---

## 5.3 Diseño de Interfaces con CSS Grid

**CSS Grid** es una técnica avanzada que permite crear diseños complejos de cuadrícula con facilidad.

**Grid Layout** divide la página en filas y columnas, lo que da un control absoluto sobre la distribución de los elementos.

### 5.3.1 Conceptos Básicos de Grid

**Contenedor Grid** : Se define el contenedor como un grid utilizando `display: grid.`

**Filas y Columnas** : Se definen con las propiedades `grid-template-columns` y `grid-template-rows`.

```css
.container {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;/* Tres columnas de igual tamaño */
    grid-gap: 10px;/* Espacio entre elementos */
    margin: 10px;
}
```

### 5.3.2 Layouts Complejos con Grid

**CSS Grid** permite crear diseños complejos mediante el uso de áreas de grid, posiciones específicas, y tamaños flexibles.

```css
/*En este ejemplo, se define un layout básico con tres áreas:
Encabezado, Contenido principal y Pie de página,
donde el encabezado y el pie ocupan toda la fila,
y el contenido principal está dividido en tres columnas.*/
.container {
    display: grid;
    grid-template-areas:
    "header header header"
    "nav main aside"
    "footer footer footer";
    grid-gap: 10px;
}
```

---

## 5.4 Efectos Visuales

**CSS** también permite aplicar efectos visuales interactivos que mejoran la experiencia del usuario.

Dos de los efectos más utilizados son sombras y transiciones.

### 5.4.1 Sombras Avanzadas
**CSS** permite aplicar sombras a los elementos para darles una apariencia tridimensional o hacer que destaquen.

```css
box-shadow: 3px 3px 4px rgb(233, 222, 222);
```

### 5.4.2 Efectos de Hover y Focus

Los efectos de hover y focus se aplican cuando el usuario pasa el cursor sobre un elemento hover o cuando un elemento recibe foco (por ejemplo, un campo de formulario).

```css
:hover {
    background-color: #d87093; transform: scale(1.05);
}
```

---

<div class="footer-nav">
    <a href="../04-estructuracion/index.md">4. Estructuración de Proyectos Web</a>
    <!-- <a href="#" class="prev-link" class="tachado">Anterior</a> -->
    <a href="../06-accesibilidad/index.md">6. Accesibilidad Web</a>    
</div>
