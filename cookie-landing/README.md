# Cookie Landing (Astro)

Landing page estatica para una casa de galletitas artesanales en Buenos Aires.

## Stack

- Astro
- CSS puro
- Imagenes WebP optimizadas

## Estructura

```text
cookie-landing/
  public/
    images/
      hero-cookies.webp
      product-chocolate.webp
      product-oat-honey.webp
      product-lemon.webp
      product-almond.webp
      og-cover.webp
    noise.png
  src/
    components/
      CTA.astro
      Hero.astro
      HowToOrder.astro
      ProductCard.astro
      SectionIntro.astro
      Testimonials.astro
    layouts/
      BaseLayout.astro
    pages/
      index.astro
    styles/
      global.css
  astro.config.mjs
  package.json
  README.md
```

## Ejecutar en local

```bash
pnpm install
pnpm dev
```

Sitio en `http://localhost:4321`.

## Build de produccion

```bash
pnpm build
pnpm preview
```

## Reemplazar placeholders por imagenes finales

1. Exportar fotos en `.webp` con tamanos recomendados:
   - `hero-cookies.webp`: 1600x1200 (peso ideal < 180 KB)
   - `product-*.webp`: 900x700 (peso ideal < 80 KB)
   - `og-cover.webp`: 1200x630
2. Mantener los mismos nombres de archivo dentro de `public/images/`.
3. Si queres cambiar precios o sabores, editar `src/pages/index.astro`.

## WhatsApp

- Enlace base: `https://wa.me/54911XXXXXXXX`
- Mensaje por defecto: `Hola, quiero pedir galletitas.`

Si queres usar un numero real, reemplazar `54911XXXXXXXX` en:

- `src/components/Hero.astro`
- `src/components/ProductCard.astro`
- `src/components/CTA.astro`
- `src/pages/index.astro`
