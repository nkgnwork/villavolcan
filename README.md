# Villa Volcán Tours — Sitio web

Landing page del operador familiar Villa Volcán Tours (Putre, Chile, desde 1988).

- **Sitio principal:** [`index.html`](./index.html)
- **Explorador 3D:** [`explorador-3d/`](./explorador-3d/)

## Secciones

1. Hero — Parinacota + claim editorial.
2. Tours — 11 expediciones con foto, ruta, flora/fauna y Google Maps por destino.
3. Hotel Las Vicuñas — Base de operaciones en Putre + strip de 6 fotos.
4. Cultura del altiplano — 6 videos: Carnaval Andino, Anata Andino, FERAN.
5. Galería — 26 postales reales del altiplano chileno.
6. Cotizador WhatsApp — abre WhatsApp con mensaje listo.

## Estructura

```
.
├── index.html              # Landing principal (~107 KB)
├── img/                    # 60 fotos optimizadas (.webp, ~15 MB)
├── explorador-3d/
│   ├── index.html          # Mapa 3D con MapLibre
│   └── img/                # Thumbnails de POIs
└── .github/workflows/pages.yml
```

## Deploy en GitHub Pages

1. Settings → Pages → Source: **GitHub Actions**.
2. Cada `git push` a `main` despliega automáticamente.

URL pública: **https://nkgnwork.github.io/villavolcan-tours/**

## Local

```bash
python3 -m http.server 8000
```

## Optimización

- Fotos: ~300 MB JPG → ~15 MB WebP (-95 %).
- Videos de cultura: YouTube embed (lazy + sin cookies).

## i18n

Diccionario ES/EN con paridad total (198 claves por idioma).

---
© Villa Volcán Tours · Hotel Las Vicuñas · Putre, Arica y Parinacota.
