# MotoMundo.pe - Tienda de Motos

Proyecto web completo de una tienda de motos desarrollado con **HTML5 semántico**, **CSS3 responsivo**, **Bootstrap 5**, **Font Awesome** y **JavaScript vanilla**.

## Estructura del Proyecto

```
proyect-web-motos/
├── index.html            # Landing page principal
├── nosotros.html         # Quiénes somos
├── catalogo.html         # Catálogo con 7 filtros dinámicos
├── servicio.html         # Servicio Técnico con planes, FAQ y CTAs
├── tiendas.html          # Nuestras Tiendas con 6 sucursales
├── contacto.html         # Formulario de contacto con validación
├── presentacion.html     # Presentación del proyecto
├── css/
│   └── styles.css        # Estilos personalizados (213 líneas)
└── README.md
```

## Páginas y Funcionalidades

### index.html — Inicio
- Navbar sticky con logo, menú de 6 enlaces, buscador e icono de usuario
- Hero con gradiente oscuro, título y CTA "Ver Catálogo"
- Sección "¿Por qué elegirnos?" con 3 tarjetas (Garantía, Envío Gratis, Soporte 24/7)
- Motos destacadas con efecto hover (translateY + shadow)
- Video embebido de YouTube (multimedia)
- Footer con redes sociales
- Menú responsive con panel lateral y overlay

### nosotros.html — Nosotros
- Imagen representativa del taller
- Historia de la empresa
- Visión, Misión y Valores en cards

### catalogo.html — Catálogo
- Título en hero superior con fondo claro
- **Sidebar de filtros** (7 categorías):
  - Marca (Yamaha, Honda, Kawasaki, Suzuki, Ducati, Harley-Davidson)
  - Precio (rangos desde <$5,000 hasta >$20,000)
  - Tipo de Moto (Deportiva, Cruiser, Urbana, Adventure)
  - Motor (Monocilíndrico, Bicilíndrico, Tricilíndrico, Tetracilíndrico)
  - Cilindrada (rangos de cc)
  - Potencia (rangos de HP)
  - Nro. de cilindros (1, 2, 3, 4)
- Grid de productos en 3 columnas con imágenes reales
- Badges "Nuevo" y "Oferta"
- Botón "Agregar" con alerta interactiva
- Filtros combinados con lógica AND en JS
- Responsive: menú de filtros colapsable en móvil

### servicio.html — Servicio Técnico
- Hero con gradiente oscuro y CTAs (Agendar Cita, Ver Servicios)
- **3 planes de servicio** con precios y checklist:
  - Mantenimiento Preventivo — S/149
  - Reparación General — S/399 (destacado "Más popular")
  - Personalización — S/249
- **Proceso en 4 pasos** (Agendar → Diagnosticar → Presupuestar → Recoger)
- **Testimonios** de clientes con fotos y valoración de 5 estrellas
- **FAQs** (5 preguntas en acordeón)
- **CTA final** con teléfono y reserva online

### tiendas.html — Nuestras Tiendas
- Grid de 6 sucursales con mapas embebidos:
  - Lima Centro, Miraflores, San Isidro
  - Arequipa, Cajamarca, Piura
- Cada una con dirección, teléfono y horario

### contacto.html — Contacto
- Formulario con validación HTML5 + JS
  - Nombre (mín. 3 caracteres)
  - Correo electrónico (formato válido)
  - Teléfono
  - Mensaje (mín. 10 caracteres)
- Alertas dinámicas de confirmación
- Mapa de Google Maps embebido
- Información de contacto (dirección, teléfono, email, horario)

### presentacion.html — Presentación
- Navegación por secciones (scrollspy)
- Explicación del flujo del proyecto
- Estructura de archivos
- Tecnologías utilizadas
- Fragmentos de código con sintaxis coloreada
- Tabla de interacciones JavaScript

## Tecnologías

| Tecnología | Uso |
|------------|-----|
| **HTML5** | Etiquetas semánticas (`<header>`, `<main>`, `<section>`, `<article>`, `<footer>`, `<nav>`, `<details>`, `<summary>`) |
| **CSS3** | Flexbox, Grid, transitions, media queries, `clamp()`, `aspect-ratio`, `accent-color` |
| **Bootstrap 5** | Grid responsivo, cards, accordion, badges, utilities, navbar |
| **Font Awesome 6** | Iconos en navbar, servicios, testimonios y footer |
| **Bootstrap Icons** | Iconos complementarios en cards y redes sociales |
| **JavaScript** | Manipulación del DOM, eventos, arrays, filter, template strings, validación de formularios |
| **Multimedia** | Imágenes Unsplash (lazy loading), video YouTube, Google Maps embebido |

## Diseño Responsivo

- **Desktop (>1024px):** Grid de 3-4 columnas, sidebar visible, navbar horizontal
- **Tablet (768-1024px):** Grid de 2-3 columnas
- **Móvil (<768px):** Grid de 1-2 columnas, menú panel lateral, filtros ocultos con botón toggle
- **Navbar:** Sticky, menú hamburguesa en móvil con overlay oscuro

## JavaScript — Interacciones DOM

| Página | Función | Descripción |
|--------|---------|-------------|
| `catalogo.html` | `mostrarMotos()` | Renderiza cards de productos en el grid |
| `catalogo.html` | `aplicarFiltros()` | Filtra motos por marca, precio, tipo, motor, cilindrada, potencia y cilindros |
| `catalogo.html` | Botón "Agregar" | Muestra alerta con el nombre del producto |
| `catalogo.html` | `btn-clear` | Limpia todos los filtros activos |
| `contacto.html` | `submit` evento | Valida formulario y muestra mensaje de éxito |
| Todas | Menú móvil | Toggle del panel de navegación lateral |


