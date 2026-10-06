# DIVINE | Calzado Femenino de Autor

Sitio web oficial de **DIVINE**, marca de calzado femenino de autor con confección artesanal y materiales nobles.

## 🌐 Sitio Web Online
*Ver sitio desplegado: https://FabiolaEstudio23.github.io/proyecto-divine-coderhause-94785/

## 🛠️ Tecnologías Utilizadas
- **HTML5**: Maquetación semántica y estructura accesible.
- **CSS3**: Mobile-First, CSS Grid (`grid-template-areas`), Flexbox y pseudoclases interactivas (`:hover`, `:focus`, `:active`).
- **Bootstrap 5**: Navbar responsive con menú hamburguesa y Carousel de modelos.

## 📱 Páginas Responsivas
- `index.html`: Portada, galería principal y presentación de marca.
- `pages/productos.html`: Catálogo con Carousel y sección de reseñas de clientas.
- `pages/contacto.html`: Canales de atención y boutiques con CSS Grid.
- `pages/sobre-nosotros.html` y `pages/guia-talles.html`: Páginas informativas con Navbar y Footer unificados.

- **SCSS (Sass)**: Estilos organizados en partials con variables, mixins, nesting y `@use`.

## 🗂️ Estructura SCSS

scss/
├── main.scss        # Único punto de entrada (@use)
├── utilities/       # _variables.scss y _mixins.scss
├── base/            # _base.scss y _tipografia.scss
├── layout/          # _header.scss, _nav.scss, _grid.scss y _footer.scss
└── components/      # _buttons.scss, _cards.scss, _hero.scss, _carousel.scss y _resenas.scss

## ⚙️ Cómo compilar

El archivo `styles/styles.css` es el resultado de la compilación y no se edita a mano.

sass scss/main.scss styles/styles.css --no-source-map