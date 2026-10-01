# Espacio de Formación Permanente en IA · UFV

Mini webs de innovación docente de la UFV para incrustar en Canvas mediante iframe.
Se publican con GitHub Pages en `https://innapufv.github.io/formacion-ia/`.

## Estructura
- `index.html`: portada del Espacio de Formación.
- `comprender-ia/` · 01 Comprender la IA y utilizarla con criterio
- `herramientas-gemini/` · 02 Adopción de herramientas de Gemini
- `experiencias-uso/` · 03 Explorar experiencias de uso UFV con Gemini
- `evaluacion-ia/` · 04 Evaluación UFV en tiempos de IA
- `acompanar-alumnos/` · 05 Acompañar a mis alumnos
- `assets/ufv.css`: estilos compartidos (kit web UFV).
- `assets/logo-ufv.png`: logo.

## Normas
- Todas las páginas llevan `<meta name="robots" content="noindex, nofollow, …">` para que no se indexen en buscadores.
- Los enlaces hacia Canvas usan `target="_top"` y se configuran en el bloque `ENLACES` de cada página.
- El estilo sigue la guía web UFV; si una maqueta se aparta de ella, prima la guía.
- Cada vez que cambie `assets/ufv.css`, se actualiza el parámetro `?v=` del enlace a la hoja de estilos en todas las páginas para que los navegadores no usen la versión en caché.
- Diseño pensado para el ancho de una página de Canvas (unos 800–1000 px) y para que de un vistazo se vean el hero y las tarjetas: hero compacto, cabecera no fija y espaciados reducidos respecto al kit web general.
- Las páginas no llevan cabecera con logo ni pie: dentro de Canvas empiezan directamente en el hero.
- Color: el azul (número con subrayado celeste, hover) da la estructura; el frambuesa se reserva para las etiquetas de categoría de los recursos y los antetítulos, como en las webs UFV.
