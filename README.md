# Jekakuaa

Landing page estática de **Jekakuaa** — Consultoría TI y soluciones digitales para empresas paraguayas.

🌐 **Sitio online**: [jekakuaa.vercel.app](https://jekakuaa.vercel.app)

## Stack

- **[Astro 7](https://astro.build)** — Framework para sitios estáticos ultra rápidos
- **[Tailwind CSS 4](https://tailwindcss.com)** — Estilos utility-first
- **[Vercel](https://vercel.com)** — Hosting con SSL automático
- **pnpm** — Package manager

## Estructura del proyecto

```
jekakuaa/
├── public/                    # Assets estáticos
│   ├── favicon.svg            # Ícono del sitio
│   ├── og-image.svg           # Imagen para compartir en redes
│   └── robots.txt
├── src/
│   ├── components/            # Componentes Astro
│   │   ├── Header.astro
│   │   ├── Hero.astro
│   │   ├── Services.astro
│   │   ├── About.astro
│   │   ├── WhyUs.astro
│   │   ├── Contact.astro
│   │   ├── Footer.astro
│   │   └── WhatsAppFab.astro
│   ├── layouts/
│   │   └── Layout.astro       # Layout base con SEO
│   ├── pages/                 # Rutas del sitio
│   │   ├── index.astro        # Home
│   │   ├── terminos.astro     # Términos y Condiciones
│   │   └── privacidad.astro   # Política de Privacidad
│   └── styles/
│       └── global.css         # Tailwind + variables de tema
├── astro.config.mjs
├── tailwind.config.js
├── tsconfig.json
└── package.json
```

## Desarrollo local

Requisitos: Node.js >= 22.12, pnpm >= 9.

```bash
# Instalar dependencias
pnpm install

# Levantar el dev server (http://localhost:4321)
pnpm dev

# Build de producción
pnpm build

# Preview del build
pnpm preview
```

## Deploy

El deploy es **automático** con cada `git push` a la rama `main`:

1. Hacé los cambios que necesites
2. `git add . && git commit -m "descripción del cambio"`
3. `git push origin main`
4. Vercel buildea y deploya en ~30-60 segundos

Para ver el estado de los deploys: [vercel.com/dashboard](https://vercel.com/dashboard)

## Paleta de colores

| Token | Color | Uso |
|---|---|---|
| `primary` | `#4FA67A` | Botones, acentos, íconos |
| `primary-light` | `#7BC4A0` | Hover, bordes sutiles |
| `primary-very-light` | `#E5F4ED` | Backgrounds alternos |
| `primary-dark` | `#1A5F4A` | Títulos, texto principal |
| `accent` | `#2E8B6B` | Links, detalles destacados |
| `whatsapp` | `#25D366` | Botón flotante WhatsApp |

Las variables están definidas en `src/styles/global.css` dentro del bloque `@theme`.

## Contacto

- **Email**: eduardo.kndia@gmail.com
- **WhatsApp**: +595 981 635 329
- **Ubicación**: Asunción, Paraguay

---

© 2026 Jekakuaa — Hecho en Paraguay 🇵🇾
