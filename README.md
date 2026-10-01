# Espacio de Formación Permanente en IA · UFV

Mini webs de innovación docente de la UFV para incrustar en Canvas mediante iframe.
Se publican con GitHub Pages en `https://innapufv.github.io/formacion-ia/`.

## Estructura
- `index.html`: portada del Espacio de Formación.
- `<pieza>/index.html`: cada subpágina en su propia carpeta.
- `assets/ufv.css`: estilos compartidos (kit web UFV).
- `assets/logo-ufv.png`: logo.

## Normas
- Todas las páginas llevan `<meta name="robots" content="noindex, nofollow, …">` para que no se indexen en buscadores.
- Los enlaces hacia Canvas usan `target="_top"` y se configuran en el bloque `ENLACES` de cada página.
- El estilo sigue la guía web UFV; si una maqueta se aparta de ella, prima la guía.
- Cada vez que cambie `assets/ufv.css`, se actualiza el parámetro `?v=` del enlace a la hoja de estilos en todas las páginas para que los navegadores no usen la versión en caché.
