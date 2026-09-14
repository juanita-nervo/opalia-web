# Opalia Deco

Sitio web desarrollado para **Opalia Deco**, un emprendimiento dedicado a la elaboración y venta de velas artesanales y piezas decorativas de yeso.

El proyecto fue realizado aplicando HTML5, SCSS, Bootstrap, diseño responsive y animaciones.

## 📁 Estructura del proyecto

```text
opalia-web/
│
├── index.html
│
├── pages/
│   ├── sobre-mi.html
│   ├── proyectos.html
│   ├── servicios.html
│   └── contacto.html
│
├── scss/
│   ├── main.scss
│   │
│   ├── utilities/
│   │   ├── _variables.scss
│   │   ├── _mixins.scss
│   │   └── _extends.scss
│   │
│   ├── base/
│   │   ├── _base.scss
│   │   └── _tipografias.scss
│   │
│   ├── layout/
│   │   ├── _header.scss
│   │   ├── _nav.scss
│   │   └── _footer.scss
│   │
│   └── components/
│       ├── _buttons.scss
│       ├── _cards.scss
│       ├── _inicio.scss
│       ├── _proyectos.scss
│       └── _sobre-mi.scss
│
├── styles/
│   ├── styles.css
│   └── styles.css.map
│
├── img/
│   └── imágenes del proyecto
│
└── README.md
```

## 🛠️ Tecnologías utilizadas

* HTML5
* SCSS / Sass
* CSS3
* Bootstrap 5
* AOS (Animate On Scroll)
* Git
* GitHub
* GitHub Pages

## 💻 Ejecución del proyecto

### Opción 1: Live Server

1. Clonar o descargar este repositorio.
2. Abrir la carpeta del proyecto en Visual Studio Code.
3. Instalar la extensión **Live Server**.
4. Abrir `index.html` con Live Server.

### Opción 2: Sass

El proyecto utiliza SCSS como fuente de estilos y CSS como archivo compilado.

Para recompilar los estilos:

```bash
sass scss/main.scss styles/styles.css
```

Para observar los cambios automáticamente:

```bash
sass --watch scss/main.scss:styles/styles.css
```


## 📄 Páginas

El proyecto cuenta con cinco archivos HTML:

1. `index.html` — Página de inicio.
2. `pages/sobre-mi.html` — Información sobre el emprendimiento.
3. `pages/proyectos.html` — Proyectos y trabajos realizados.
4. `pages/servicios.html` — Servicios ofrecidos.
5. `pages/contacto.html` — Información de contacto.

Todas las páginas comparten la navegación y el footer, manteniendo una estructura visual coherente.


## Sitio web

Podés visitar el sitio desplegado en:

**[Ver Opalia Deco]
(https://juanita-nervo.github.io/opalia-web/)**
