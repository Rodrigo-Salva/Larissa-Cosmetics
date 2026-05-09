# Rodrigo Dev — Catálogo de Proyectos

Catálogo web construido con **Astro** para mostrar y vender proyectos de software.

## 🚀 Cómo correrlo

```bash
npm install
npm run dev       # desarrollo en http://localhost:4321
npm run build     # build de producción
npm run preview   # previsualizar el build
```

## ✏️ Agregar o editar proyectos

Edita el archivo `src/data/proyectos.json`. Cada proyecto tiene esta estructura:

```json
{
  "id": 9,
  "nombre": "Mi Nuevo Proyecto",
  "precio": 1500,
  "descripcion": "Descripción detallada del proyecto...",
  "categoria": "Web App",
  "badge": "",
  "emoji": "🚀",
  "tecnologias": "Node.js, React, MySQL",
  "tiempo": "3–4 semanas",
  "incluye": "Deploy, documentación, soporte",
  "tags": ["Node.js", "React", "MySQL"]
}
```

### Campos del JSON

| Campo | Descripción |
|-------|-------------|
| `id` | Número único del proyecto |
| `nombre` | Nombre del proyecto |
| `precio` | Precio en Soles (S/) |
| `descripcion` | Descripción completa |
| `categoria` | SaaS, CRM, E-Commerce, Web App, API, Dashboard, Mobile |
| `badge` | `"popular"`, `"new"` o `""` (vacío para ninguno) |
| `emoji` | Emoji representativo |
| `tecnologias` | Stack tecnológico |
| `tiempo` | Tiempo estimado de entrega |
| `incluye` | Qué está incluido en el precio |
| `tags` | Array de tecnologías para los chips |

## 📁 Estructura del proyecto

```
src/
├── components/
│   ├── Navbar.astro       — Barra de navegación
│   ├── Hero.astro         — Sección hero + marquee
│   ├── ProductCard.astro  — Tarjeta de cada proyecto
│   ├── Modal.astro        — Modal de detalle
│   └── Footer.astro       — CTA de contacto + footer
├── data/
│   └── proyectos.json     — ← TU FUENTE DE DATOS
├── layouts/
│   └── BaseLayout.astro   — HTML base
├── pages/
│   └── index.astro        — Página principal
└── styles/
    └── global.css         — Design tokens y estilos base
```

## 🎨 Personalizar

- **Colores**: edita las variables en `src/styles/global.css`
- **WhatsApp**: busca `51999999999` y reemplaza con tu número
- **Correo**: busca `rodrigo@email.com` y reemplaza
- **Información personal**: edita `src/components/Footer.astro`

## 🌐 Deploy

Compatible con **Vercel**, **Netlify** y **Render** (output: static).
