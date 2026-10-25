# DIVINE | Calzado Femenino de Autor

Sitio web oficial de **DIVINE**, marca de calzado femenino de autor con confección artesanal y materiales nobles.

## 🌐 Sitio Web Online

**Deploy en Netlify:** https://divine-calzado.netlify.app

## 🛠️ Tecnologías Utilizadas
- **HTML5**: Maquetación semántica y estructura accesible.
- **CSS3**: Mobile-First, CSS Grid (`grid-template-areas`), Flexbox y pseudoclases interactivas (`:hover`, `:focus`, `:active`).
- **Bootstrap 5**: Navbar responsive con menú hamburguesa y Carousel de modelos.
- **AOS**: animaciones al hacer scroll (librería externa).
- **Animaciones nativas**: `@keyframes` y `transition` escritas en SCSS.
- **SCSS (Sass)**: partials, variables, mixins con parámetros, `@extend` y operadores.

## 📱 Páginas Responsivas
- `index.html`: Portada, galería principal y presentación de marca.
- `pages/productos.html`: Catálogo con Carousel y sección de reseñas de clientas.
- `pages/contacto.html`: Canales de atención y boutiques con CSS Grid.
- `pages/sobre-nosotros.html` y `pages/guia-talles.html`: Páginas informativas con Navbar y Footer unificados.

## 📁 Estructura del proyecto

```
├── index.html          # portada
├── pages/              # productos, sobre-nosotros, guia-talles y contacto
├── assets/img/         # todas las imágenes del sitio
├── scss/               # estilos fuente (SCSS)
├── styles/styles.css   # CSS compilado
├── robots.txt
└── sitemap.xml
```

## 🗂️ Estructura SCSS

```
scss/
├── main.scss        # único punto de entrada (@use)
├── utilities/       # _variables.scss y _mixins.scss
├── base/            # _base.scss, _tipografia.scss y _animaciones.scss
├── layout/          # _header.scss, _nav.scss, _grid.scss y _footer.scss
└── components/      # _buttons, _cards, _hero, _carousel, _accordion y _resenas
```

## ⚙️ Cómo compilar

El archivo `styles/styles.css` es el resultado de la compilación y no se edita a mano.

```bash
sass scss/main.scss styles/styles.css --no-source-map
```

## 🔍 SEO y Accesibilidad

- `<title>` y `meta description` únicos en cada página, con keywords acordes a su contenido.
- Etiquetas Open Graph y `canonical` en las 5 páginas.
- Datos estructurados (JSON-LD) de la tienda en la página de contacto, para SEO local.
- Todas las imágenes con `alt` descriptivo y nombres de archivo descriptivos.
- `robots.txt` y `sitemap.xml`.
- HTML semántico: `header`, `nav`, `main`, `section`, `article` y `footer`.
- Footer sin `<div>` genéricos: redes sociales en `<nav>`, dirección y horarios en `<address>` y copyright en `<small>`.
- Reseñas con `<figure>` + `<blockquote>` + `<figcaption>`; las estrellas son decorativas (`aria-hidden`) y la calificación se anuncia con texto para lectores de pantalla.
- Contraste WCAG AA verificado en las 5 páginas (mínimo 4.5:1 en todos los textos).