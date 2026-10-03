# 🌐 Proyecto Final — Sitio Web Estático

Sitio web estático de **5 páginas** desarrollado como proyecto final del curso, integrando los principales conceptos trabajados durante las clases: **HTML semántico, CSS/SCSS, Bootstrap, diseño responsive, animaciones, SEO y despliegue web**.

## 🚀 Demo

🔗 **Sitio web:** [Ver sitio desplegado](https://opaliaweb.netlify.app/)

🔗 **Repositorio:** [Ver repositorio en GitHub](https://github.com/juanita-nervo/opalia-web)

---

## 📌 Descripción

El proyecto consiste en el desarrollo de un sitio web estático de cinco páginas, diseñado para adaptarse correctamente a distintos tamaños de pantalla y mantener una identidad visual consistente en toda la navegación.

Para su desarrollo se utilizaron **HTML5, SCSS y Bootstrap**, incorporando además animaciones nativas y una librería externa de animaciones.

El sitio fue optimizado teniendo en cuenta aspectos de **SEO**, accesibilidad, organización del código y buenas prácticas de desarrollo frontend.

---

## 🛠️ Tecnologías utilizadas

* **HTML5** — estructura y contenido del sitio.
* **SCSS** — estilos, variables, mixins, nesting, extend y partials.
* **Bootstrap** — componentes y navbar responsive.
* **AOS / Animate.css** — animaciones externas.
* **JavaScript** — funcionamiento de componentes interactivos de Bootstrap.
* **Git / GitHub** — control de versiones y almacenamiento del proyecto.
* **Netlify** — despliegue del sitio.

---

## 📁 Estructura del proyecto

```text
/
├── index.html
│
├── pages/
│   ├── contacto.html
│   ├── proyectos.html
│   ├── servicios.html
│   └── sobre-mi.html
│
├── scss/
│   ├── base.scss
│   ├── components.scss
│   ├── layout.scss
│   ├── utilities.scss
│   └── main.scss
│
├── styles/
│   └── styles.css
│
├── img/
│   └── ...
│
└── README.md
```

> Los nombres de los archivos dentro de `scss/` pueden variar según la organización utilizada en el proyecto. La estructura respeta la separación entre archivos parciales y el archivo principal `main.scss`.

---

## 📄 Páginas

El sitio está compuesto por cinco páginas:

1. **Inicio (`index.html`)**
   Página principal del sitio y punto de entrada para los usuarios.

2. **Sobre mi**
   Página destinada a explicar mi historia.

3. **Proyectos**
   Últimos proyectos más importantes de Opália

4. **Servicios**
   Distintos servicios en los que se puede contratar a opália

5. **Contacto**
   Medios de comunicación para contactar a opália

Todas las páginas cuentan con una estructura semántica utilizando elementos como:

* `<header>`
* `<nav>`
* `<main>`
* `<section>`
* `<article>`
* `<footer>`

---

## 🎨 SCSS

Los estilos del proyecto fueron desarrollados utilizando **SCSS**, organizados mediante una arquitectura de **partials**.

Se implementaron:

* **Variables** para colores, tipografías, tamaños y otros valores reutilizables.
* **Nesting** para organizar los selectores.
* **Mixins con parámetros** para reutilizar estilos.
* **Extend** para compartir propiedades entre componentes.
* **Partials** para separar los estilos según su función.
* **`@use`** para importar los diferentes archivos SCSS.

El archivo `main.scss` se utiliza exclusivamente para importar los partials:

```scss
@use "variables";
@use "mixins";
@use "extend";
@use "header";
@use "navbar";
@use "components";
@use "footer";
@use "pages";
```

El CSS resultante se encuentra dentro de la carpeta `styles/`.

---

## 📱 Diseño responsive

El sitio fue desarrollado siguiendo un enfoque **responsive**, adaptándose a:

* 📱 **Mobile**
* 📲 **Tablet**
* 💻 **Desktop**

Se utilizaron **media queries** para modificar la distribución y presentación de los elementos según el tamaño de pantalla.

También se verificó que el sitio no genere **scroll horizontal** ni problemas de compresión o superposición de elementos.

---

## 🧩 Bootstrap

Se utilizó **Bootstrap** para implementar diferentes componentes y facilitar el desarrollo responsive.

Uno de los componentes principales utilizados es la **navbar responsive**, presente en las cinco páginas.

El menú hamburguesa permite navegar correctamente desde dispositivos móviles y fue personalizado mediante SCSS para mantener la identidad visual del proyecto.

---

## ✨ Animaciones

El proyecto incorpora dos tipos de animaciones:

### Animaciones nativas

Se utilizaron propiedades de SCSS/CSS como:

* `transition`
* `transform`
* `@keyframes`

Estas animaciones permiten agregar interactividad y dinamismo a diferentes elementos de la página.

### Librería externa

También se incorporó una librería externa de animaciones:

**AOS (Animate On Scroll)**

Esta herramienta permite aplicar animaciones a determinados elementos a medida que aparecen durante el desplazamiento de la página.

---

## 🔎 SEO

Cada página cuenta con elementos básicos de optimización SEO:

* `<title>` descriptivo y único.
* `<meta name="description">` propio.
* `<meta name="keywords">` propio.
* Atributos `alt` en las imágenes.
* Estructura HTML semántica.
* Contenido organizado mediante títulos y secciones.

Ejemplo:

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Título descriptivo de la página</title>

    <meta
        name="description"
        content="Descripción de la página y su contenido."
    >

    <meta
        name="keywords"
        content="palabra1, palabra2, palabra3"
    >
</head>
```

---

## 🖼️ Recursos multimedia

Todos los recursos utilizados por el sitio se encuentran organizados dentro de la carpeta `assets/`.

```text
assets/
├── img/
├── icons/
└── ...
```

Las imágenes utilizadas cuentan con su correspondiente atributo `alt` para mejorar la accesibilidad y aportar información alternativa en caso de que no puedan visualizarse.

---

## 📦 Instalación y ejecución

Para ejecutar el proyecto de manera local:

### 1. Clonar el repositorio

```bash
git clone URL_DEL_REPOSITORIO
```

### 2. Ingresar a la carpeta

```bash
cd nombre-del-proyecto
```

### 3. Abrir el proyecto

Abrir el archivo `index.html` en el navegador.

También se recomienda utilizar **Visual Studio Code** junto con **Live Server** para visualizar el proyecto durante el desarrollo.

---

## 🔄 Compilación de SCSS

Los archivos `.scss` se encuentran dentro de la carpeta `scss/` y el CSS compilado se genera dentro de `styles/`.

Si se utiliza Sass mediante npm, puede compilarse con:

```bash
sass scss/main.scss styles/main.css
```

Para mantener la compilación automática durante el desarrollo:

```bash
sass --watch scss/main.scss:styles/main.css
```

---

## 🌎 Despliegue

El sitio fue desplegado utilizando **Netlify**, permitiendo acceder públicamente al proyecto.

### 🔗 Link del sitio

**https://opaliaweb.netlify.app/**

Antes del despliegue se verificaron las rutas de:

* Imágenes.
* Archivos CSS.
* Archivos JavaScript.
* Fuentes e íconos.
* Navegación entre las diferentes páginas.

---

## 📚 Requisitos cumplidos

| Requisito                         | Estado |
| --------------------------------- | :----: |
| 5 páginas HTML                    |    ✅   |
| HTML semántico                    |    ✅   |
| `title` único en cada página      |    ✅   |
| `meta description`                |    ✅   |
| `meta keywords`                   |    ✅   |
| `alt` en imágenes                 |    ✅   |
| Navbar de Bootstrap               |    ✅   |
| Navbar responsive                 |    ✅   |
| SCSS                              |    ✅   |
| Variables                         |    ✅   |
| Nesting                           |    ✅   |
| Mixins con parámetros             |    ✅   |
| Extend                            |    ✅   |
| Partials                          |    ✅   |
| `main.scss` únicamente con `@use` |    ✅   |
| Diseño responsive                 |    ✅   |
| Media queries                     |    ✅   |
| Animación nativa                  |    ✅   |
| Animación con librería externa    |    ✅   |
| Carpeta `assets/`                 |    ✅   |
| CSS compilado en `styles/`        |    ✅   |
| Despliegue en Vercel/Netlify      |    ✅   |
| Repositorio público               |    ✅   |
| Al menos 2 commits descriptivos   |    ✅   |

---

## 👨‍💻 Autor

**Juanita Nervo**

Proyecto realizado como entrega final del curso de desarrollo web.
