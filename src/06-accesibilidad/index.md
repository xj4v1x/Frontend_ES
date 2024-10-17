---
title: "Accesibilidad Web"
description: "Cap.6. Accesibilidad Web"
date: 2024-10-15
series: ["Guía HTML y CSS"]
series_order: 6
build:
  list: never
---


## 6. Accesibilidad Web

La **accesibilidad web** se refiere al diseño y desarrollo de sitios web de manera que puedan ser utilizados por todas las personas, incluidas aquellas con discapacidades.

Un sitio web accesible facilita la navegación y el acceso a la información, mejorando la experiencia del usuario y cumpliendo con normativas y estándares internacionales.

---

## 6.1 ¿Qué es la Accesibilidad Web?

La **accesibilidad web** garantiza que las personas con discapacidades (visuales, auditivas, motoras o cognitivas) puedan navegar, interactuar y comprender el contenido de una página web.

Para que una web sea accesible, debe estar diseñada y desarrollada teniendo en cuenta tecnologías de asistencia como lectores de pantalla, dispositivos de entrada especializados, entre otros.

#### Beneficios de la Accesibilidad Web

- **Inclusión social**: Permite que todas las personas, independientemente de sus habilidades, puedan utilizar la web.

- **Mejora la experiencia del usuario**: No solo mejora el acceso para personas con discapacidades, sino que también facilita el uso para todos, especialmente en dispositivos móviles.

- **Cumplimiento legal**: En muchos países, la accesibilidad web está regulada por leyes que exigen que los sitios web cumplan con ciertas normas de accesibilidad.

- **Mejora el SEO**: Los motores de búsqueda valoran las páginas accesibles porque facilitan el rastreo y la comprensión del contenido.

---

## 6.2 Principios de Accesibilidad

La **Iniciativa de Accesibilidad Web** (*WAI*) de la *W3C* ha establecido cuatro principios fundamentales que deben guiar el diseño accesible de sitios web:

- **Perceptible**: La información y los componentes de la interfaz deben presentarse de manera que los usuarios puedan percibirlos, ya sea visual o auditivamente.

    *Ejemplo: Proporcionar texto alternativo (`alt`) para las imágenes, de modo que los usuarios que utilicen lectores de pantalla puedan entender el contenido visual.*

- **Operable**: Los usuarios deben poder navegar y operar la interfaz utilizando una variedad de dispositivos, como teclados, ratones o comandos de voz.

    *Ejemplo: Asegurar que todos los enlaces y botones sean accesibles mediante el teclado.*

- **Comprensible**: El contenido debe ser claro, y la interfaz debe comportarse de manera predecible, de modo que los usuarios puedan entender cómo interactuar con ella.

    *Ejemplo: Proporcionar instrucciones claras y utilizar un lenguaje sencillo en los formularios.*

- **Robusto**: El contenido debe ser interpretable por diversas tecnologías, incluidas herramientas de asistencia, sin perder funcionalidad.

    *Ejemplo: Utilizar código HTML semántico y seguir las recomendaciones del W3C para garantizar compatibilidad con futuras tecnologías.*


---

## 6.3 Mejores Prácticas para la Accesibilidad en HTML

Existen diversas prácticas recomendadas que mejoran la accesibilidad de una página web:

### 6.3.1 Uso de HTML Semántico

El **HTML semántico** no solo mejora la estructura de una página, sino que también facilita la navegación para las personas que utilizan tecnologías de asistencia.

Las etiquetas semánticas como `<header>`, `<nav>`, `<article>`, y `<footer>` proporcionan más información sobre el contenido.

```html
<header>
    <h1>Bienvenido a Mi Sitio Web</h1>
</header>
<nav>
    <ul>
        <li><a href="#inicio">Inicio</a></li>
        <li><a href="#servicios">Servicios</a></li>
    </ul>
</nav>

```


### 6.3.2 Uso de Atributos ARIA

Los atributos **ARIA** (*Accessible Rich Internet Applications*) proporcionan información adicional sobre la accesibilidad para las tecnologías de asistencia, como los lectores de pantalla.

Se utilizan para mejorar la accesibilidad en elementos dinámicos que no son necesariamente reconocidos de manera nativa por las tecnologías de asistencia.

*Ejemplo de atributos ARIA:*

```html
<!--En este ejemplo, el atributo aria-label 
describe la función del botón a los usuarios de lectores de pantalla. -->
<button aria-label="Cerrar ventana">X</button>
```

### 6.3.3 Texto Alternativo para Imágenes

Proporcionar texto alternativo (atributo `alt`) es esencial para que los usuarios que no pueden ver las imágenes puedan comprender su contenido. 

El texto alternativo describe brevemente el propósito de la imagen.

```html
<img src="imagen.jpg" alt="Descripción de la imagen">
```

Si la imagen tiene un propósito meramente decorativo, el valor del atributo `alt` debe estar vacío:

```html
<img src="decorativo.jpg" alt="">
```

---

## 6.4 Formularios Accesibles

Los formularios son una parte fundamental de muchas páginas web.

A continuación se detallan algunas recomendaciones para mejorar su accesibilidad.

### 6.4.1 Uso de Etiquetas para Campos de Formulario

Cada campo de un formulario debe tener una etiqueta (`<label>`) que describa su función.

Las etiquetas ayudan a los usuarios a comprender la información que deben proporcionar en cada campo.

```html
<label for="nombre">Nombre:</label>
<input type="text" id="nombre" name="nombre">
```

### 6.4.2 Validación Accesible de Formularios

Cuando se produce un error en el formulario, se debe proporcionar una retroalimentación clara que sea accesible para los usuarios de tecnologías de asistencia.

```html
<p class="error" aria-live="assertive">Por favor, completa el campo de nombre.</p>
```

---

## 6.5 Herramientas para Evaluar la Accesibilidad

Existen diversas herramientas que los desarrolladores pueden utilizar para evaluar la accesibilidad de un sitio web y garantizar que cumpla con los estándares establecidos.

- **WAVE** : Una herramienta gratuita en línea que analiza la accesibilidad de las páginas web.
- **Lighthouse** (*de Google*) : Una herramienta integrada en *Chrome DevTools* que proporciona auditorías de rendimiento, accesibilidad, SEO, y más.
- **NVDA** (*NonVisual Desktop Access*) : Un lector de pantalla gratuito que permite a los desarrolladores probar la accesibilidad de su sitio para usuarios ciegos.

---

## 6.6 Normativas y Estándares de Accesibilidad

Los estándares de accesibilidad web están definidos por las **Pautas de Accesibilidad para el Contenido Web** (*WCAG*), que ofrecen un conjunto de recomendaciones para hacer que el contenido web sea más accesible para personas con discapacidades.

- **WCAG 2.1**: La versión más reciente de estas pautas, que se basa en los principios de ser perceptible, operable, comprensible y robusto.

Las pautas WCAG se clasifican en tres niveles de conformidad:

- **Nivel A** : Requisitos básicos que debe cumplir una página web para ser accesible.
- **Nivel AA** : Requisitos más avanzados que se consideran la norma para cumplir con las leyes de accesibilidad en muchos países.
- **Nivel AAA** : El nivel más alto de accesibilidad, recomendado para sitios que tienen como objetivo audiencias con necesidades específicas.


---

<div class="footer-nav">
    <a href="../05-estilo-avanzado/index.md">5. Diseño y Estilo Avanzado</a>
    <!-- <a href="#" class="prev-link" class="tachado">Anterior</a> -->
    <a href="../07-implementacion/index.md">7. Implementación de Proyectos</a>    
</div>
