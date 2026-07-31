# Portafolio — Ciberseguridad & Tecnología

Portafolio profesional construido con Astro. Rápido, estático y con buena base de seguridad.

## Empezar

```bash
npm install
npm run dev      # http://localhost:4321
```

## Personalizar

Todo el contenido editable está en `src/pages/index.astro` (arriba, en los arrays
`servicios`, `proyectos`, `certs`, `stack`) y en las secciones "Sobre mí" y "Contacto".

Reemplaza:
- `tu_alias` / `[Tu Nombre]` — tu nombre o marca
- `tucorreo@ejemplo.com`, LinkedIn, GitHub — tus datos reales
- Los proyectos de ejemplo por los tuyos (labs, writeups, GitHub, casos anonimizados)
- Certificaciones y stack

Los colores y tipografías están en `src/layouts/Layout.astro` (variables `:root`).

## Publicar (gratis)

1. Sube el proyecto a un repo de GitHub.
2. Entra a vercel.com o netlify.com, conecta el repo. Detecta Astro solo.
3. Deploy automático con HTTPS. Conecta tu dominio propio desde el panel.

## Detalle de seguridad (tu primer caso de estudio)

Añade headers de seguridad. En Netlify crea un archivo `public/_headers`:

```
/*
  Strict-Transport-Security: max-age=63072000; includeSubDomains; preload
  X-Frame-Options: DENY
  X-Content-Type-Options: nosniff
  Referrer-Policy: strict-origin-when-cross-origin
  Content-Security-Policy: default-src 'self'; style-src 'self' 'unsafe-inline' https://fonts.googleapis.com; font-src https://fonts.gstatic.com
```

Luego verifica tu nota en securityheaders.com y ssllabs.com.
