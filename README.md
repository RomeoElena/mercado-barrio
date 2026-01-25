# Mercado de Barrio "La Alhóndiga"

**Sitio web informativo del Mercado de Barrio La Alhóndiga**
https://romeoelena.github.io/mercado-barrio/index.html

---

## Resumen del Proyecto

Este proyecto consiste en el diseño e implementación de un sitio web para el Mercado de Barrio "La Alhóndiga", un mercado tradicional del barrio con más de 35 años de historia. El sitio tiene como objetivo presentar el mercado, mostrar los puestos disponibles y facilitar el contacto con los vecinos.

### Características principales:

- Diseño responsive (móvil, tablet, desktop)
- Accesibilidad WCAG 2.1 Nivel A
- HTML5 semántico
- CSS vanilla (sin frameworks)
- Validación HTML5 de formularios
- 10 puestos con categorización visual

---

## Mapa del Sitio

```
Mercado La Alhóndiga
│
├── Inicio (index.html)
│   ├── Hero de bienvenida
│   ├── Sobre nosotros
│   ├── Puestos destacados (3)
│   └── Horarios
│
├── Puestos (puestos.html)
│   ├── Filtros por categoría
│   └── Listado completo (10 puestos)
│
└── Contacto (contacto.html)
    ├── Formulario de contacto
    └── Información de contacto
```

---

## Estructura de carpetas:

```
/mercado-barrio/
├── index.html
├── puestos.html
├── contacto.html
├── css/
│   └── styles.css
├── img/
│   └── (imágenes de los puestos)
└── README.md
```

### Navegación

1. **Desde la página de inicio:**

   - Haz clic en "Descubre nuestros puestos" para ir a la página de Puestos
   - Usa el menú superior para navegar entre secciones

2. **En la página de Puestos:**

   - Usa los filtros de categoría para ver puestos específicos (visual, sin funcionalidad)
   - Explora los 10 puestos disponibles con su información

3. **En la página de Contacto:**
   - Rellena el formulario con tus datos
   - Todos los campos marcados con \* son obligatorios
   - El checkbox de privacidad debe estar marcado

---

## Decisiones de Diseño

### Paleta de Colores

| Color        | Código HEX | Uso                                    |
| ------------ | ---------- | -------------------------------------- |
| Beige claro  | `#F2ECCB`  | Fondos suaves, detalles                |
| Rosa claro   | `#F49CBB`  | Acentos secundarios, hover             |
| Rosa medio   | `#F26A8D`  | Botones secundarios, transiciones      |
| Rosa intenso | `#DD2D4A`  | CTAs principales, elementos destacados |
| Verde oscuro | `#2D650A`  | Header, footer, títulos importantes    |

**Justificación:**

- El verde oscuro transmite tradición, naturaleza y productos frescos
- Los tonos rosa aportan calidez y cercanía (trato humano del mercado)
- El beige crea un fondo acogedor que no cansa la vista

### Tipografías

**Títulos y navegación:**

```css
font-family: system-ui, -apple-system, "Segoe UI", Roboto, sans-serif;
```

- Moderna y legible
- Buena para escaneado rápido
- Excelente en pantallas

**Cuerpo de texto:**

```css
font-family: Georgia, "Times New Roman", Times, serif;
```

- Serif tradicional que aporta calidez
- Refleja la esencia de "mercado de toda la vida"
- Excelente legibilidad en párrafos largos

### Layout y Espaciado

**Sistema de espaciado:**

- Padding y márgenes consistentes (múltiplos de 8px)
- Espaciado generoso para facilitar lectura
- Jerarquía visual clara con tamaños de fuente

**Grids responsive:**

- Desktop: 3 columnas para tarjetas
- Tablet: 2 columnas
- Móvil: 1 columna

### Componentes Visuales

**Tarjetas de puestos:**

- Sombras suaves que se elevan en hover
- Bordes redondeados (12px) para suavidad
- Categorías con código de color distintivo

**Botones:**

- CTAs principales: Rosa intenso (#DD2D4A)
- Botones secundarios: Rosa claro (#F49CBB)
- Estados hover con elevación y cambio de color
- Mínimo 44x44px para táctil (móvil)

**Formularios:**

- Labels siempre visibles
- Bordes de 2px para claridad
- Focus state con outline y sombra
- Validación HTML5 nativa

---

## Accesibilidad

### Cumplimiento WCAG 2.1 Nivel A

**Contraste de color:**

- Texto normal: 4.5:1 mínimo
- Texto grande: 3:1 mínimo
- Verificado con herramientas de contraste

**Navegación por teclado:**

- Todos los elementos interactivos accesibles con Tab
- Focus visible con outline de 2px
- Orden lógico de tabulación

**Estructura semántica:**

- Header, nav, main, section, article, aside, footer
- Jerarquía de encabezados sin saltos (H1 → H2 → H3)
- Un solo H1 por página

**Imágenes:**

- Alt descriptivo en todas las imágenes
- Alt="" en imágenes decorativas (si las hubiera)

**Formularios:**

- Labels asociados con for e id
- Required para campos obligatorios
- Type="email" para validación automática

**Idioma:**

- `<html lang="es">` declarado

---

## Validaciones

### W3C HTML Validator

**Resultado:** 0 errores, 0 advertencias

**URL de validación:**

- index.html: Válido
- puestos.html: Válido
- contacto.html: Válido

### W3C CSS Validator

**Resultado:** 0 errores

**URL de validación:**

- styles.css: Válido

### Lighthouse (Chrome DevTools)

**Página de Inicio:**

- Performance: 100/100
- Accessibility: 92/100
- Best Practices: 100/100
- SEO: 100/100

**Página de Puestos:**

- Performance: 100/100
- Accessibility: 93/100
- Best Practices: 100/100
- SEO: 100/100

**Página de Contacto:**

- Performance: 100/100
- Accessibility: 94/100
- Best Practices: 100/100
- SEO: 100/100

---

## Responsive Design

### Pruebas realizadas:

**Desktop:**

- 1920x1080px (Full HD)
- 1366x768px (HD estándar)

**Tablet:**

- 768x1024px (iPad)
- 1024x768px (iPad horizontal)

**Móvil:**

- 375x667px (iPhone SE)
- 414x896px (iPhone 11)
- 360x640px (Android común)

### Características responsive:

- Grid de tarjetas adapta columnas automáticamente
- Navegación se apila verticalmente en móvil
- Textos escalados para legibilidad sin zoom
- Botones táctiles (mínimo 44x44px)
- Imágenes fluidas (max-width: 100%)

---

## Tecnologías Utilizadas

- **HTML5** (semántico)
- **CSS3** (vanilla, sin frameworks)
- **Validación HTML5** (formularios)

**NO se utiliza:**

- JavaScript
- Frameworks CSS (Bootstrap, Tailwind, etc.)
- Preprocesadores (Sass, Less)
- Librerías externas

---

## Objetivos Cumplidos

**Documento de Especificación Formal (DEF)** completo y profesional  
**Wireframes** de las 3 páginas principales  
**Mapeo semántico HTML5** detallado  
**Implementación HTML** semántica y válida  
**CSS responsive** sin frameworks  
**Accesibilidad** WCAG 2.1 Nivel A  
**Validación** W3C sin errores  
 **README** con documentación completa

---

## 👨‍💻 Autor

**Elena Bragado Romeo**  
Diseño de Interfaces Web - Curso 2025/2026  
Reto 1 - Primer Trimestre

---

## 📄 UAX

Este proyecto es un trabajo académico para el módulo de Diseño de Interfaces Web.

---


