---
title: "Estructuración de Proyectos Web"
description: "Cap.4 - Estructuración de Proyectos Web"
date: 2024-10-15
series: ["Guía HTML y CSS"]
series_order: 4
build:
  list: never
---


## 4. Estructuración de Proyectos Web
Uno de los aspectos clave en el desarrollo de aplicaciones web es mantener una estructura clara y organizada, tanto en los archivos como en las carpetas del proyecto.

Una buena estructuración facilita el mantenimiento, la escalabilidad y la colaboración entre desarrolladores.

En este tema se verán las buenas prácticas para organizar un proyecto web.

---

## 4.1 Organización de Archivos y Carpetas

En un proyecto web, es importante seguir una convención clara para organizar los archivos y las carpetas, con el objetivo de facilitar la navegación por el código y reducir errores.

Una estructura típica de proyecto podría verse de la siguiente manera:



```
my_project/
    ├── css/
    │   └── styles.css
    ├── js/
    │   └── script.js
    ├── images/
    │   └── logo.png
    ├── index.html
    ├── about.html
```


### 4.1.1 Convenciones de Nombres de Archivos


Es importante seguir ciertas convenciones al nombrar archivos:

- **Utiliza** nombres descriptivos y concisos.

- **Evita** el uso de espacios; **usa** guiones bajos (`_`) o guiones medios (`-`) para separar palabras.

- **Utiliza** extensiones correctas: `.html`, `.css`, `.js`, `.jpg`, etc.



### 4.1.2 Uso de Archivos CSS Externos

Mantener los estilos en archivos **CSS** externos es una buena práctica, ya que facilita la reutilización y la administración de los estilos en múltiples páginas.

A continuación, se mencionan algunas de las propiedades más comunes.


```css
<link rel = "stylesheet" href = "css/styles.css">
```

---

## 4.2 Herramientas de Desarrollo

Las herramientas de desarrollo web son esenciales para escribir, depurar y probar el código en diferentes navegadores y dispositivos.

### 4.2.1 Editores de Código Recomendados

Existen muchos editores de código recomendados para el desarrollo web, como:

- **Visual Studio Code** : Un editor de código ligero y muy popular que ofrece una amplia gama de extensiones para mejorar la productividad.
- **Sublime Text** : Un editor rápido y personalizable.
- **Atom** : Un editor open source que también cuenta con una gran cantidad de plugins.

### 4.2.2 Uso de DevTools en el Navegador

Los navegadores modernos (como *Google Chrome*, *Firefox* y *Safari*) ofrecen herramientas de desarrollo integradas que permiten inspeccionar y modificar el código **HTML** y **CSS** directamente en la página, depurar errores de **JavaScript**, y monitorear el rendimiento de la página.

- *Acceso a las herramientas de desarrollo (DevTools):*

En *Google Chrome* y *Firefox*:

`F12` o `clic derecho` ➟ **Inspeccionar**

---

## 4.3 Buenas Prácticas de Código

Mantener un código limpio y bien estructurado es crucial para el mantenimiento y la escalabilidad de un proyecto web. A continuación se presentan algunas buenas prácticas recomendadas.

### 4.3.1 Escribir HTML Semántico

El **HTML** semántico es el uso de etiquetas que transmiten el significado del contenido.

En lugar de usar `div` para todo, es mejor utilizar etiquetas como `<header>`, `<nav>`, `<article>`, `<section>` y `<footer>`, ya que mejoran la accesibilidad y optimizan el **SEO**.

```html
<header>
    <h1>Bienvenido a mi sitio web</h1>
</header>
<nav>
    <ul>
        <li>
            <a href = "index.html">Inicio</a>
        </li>
        <li>
            <a href = "about.html">Sobre Nosotros</a>
        </li>
    </ul>
</nav>
```

### 4.3.2 Comentarios y Documentación en CSS

Es importante documentar el código para que otros desarrolladores (*o tú mismo en el futuro*) puedan entenderlo fácilmente.

Los comentarios se utilizan para explicar partes del código o separar secciones.

- Comentarios en **HTML**:

    `<!-- Este es un comentario en HTML -->`

- Comentarios en **CSS**:

    `/* Este es un comentario en CSS */`



---

<div class="footer-nav">
    <a href="../css-fundamentos/">3. Fundamentos de CSS</a>
    <!-- <a href="#" class="prev-link" class="tachado">Anterior</a> -->
    <a href="../estilo-avanzado/" class="next-link">5. Diseño y Estilo Avanzado</a>    
</div>