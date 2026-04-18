# Fundar Labs — Landing

Sitio estático construido con **Astro 5** y **Tailwind CSS v4**.

## Desarrollo

```bash
npm install
npm run dev       # http://localhost:4321
npm run build     # genera /dist
```

## Deploy

Configurado para **Cloudflare Pages**:

- Build command: `npm run build`
- Build output directory: `dist`
- Node version: 20+

Dominio productivo: `fundarlabs.com.mx` (DNS en Vultr, proxy/servicio en Cloudflare Pages).

## Estructura

```
src/
  layouts/Base.astro     # HTML shell + fuentes
  pages/index.astro      # Landing completa
  styles/global.css      # Tailwind v4 + tokens
public/                  # favicon, robots.txt, assets estáticos
```

## Notas

- Mientras el sitio esté en construcción, `<meta name="robots" content="noindex,nofollow">` está activo y `robots.txt` bloquea crawlers.
- Contacto: `hola@fundarlabs.com.mx` (pendiente de configurar).
