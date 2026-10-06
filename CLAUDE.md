# Portal de Formación en IA · UFV — instrucciones de trabajo

Repositorio de mini webs que se incrustan en Canvas (curso 44179 de ufv-es.instructure.com) mediante iframe.
Publicación: GitHub Pages → `https://innapufv.github.io/formacion-ia/<carpeta>/`

## Normas fijas
- **Estilo UFV** (guía en el proyecto «Avance en IA para el modelo formativo» → `claude/Guía de estilo web UFV.md`). Si una maqueta o imagen se aparta del estilo, **prima el estilo**: de la imagen se toman contenido y estructura.
- Siempre en claro. Sin cabecera con logo ni pie: cada página empieza en el hero (azul noche con anillos).
- Formato compacto para el ancho de Canvas (800–1000 px).
- **Siempre no indexable**: `<meta name="robots" content="noindex, nofollow, noarchive, nosnippet, noimageindex">` (+ googlebot, bingbot).
- Hoja de estilos compartida `assets/ufv.css`. **Cada vez que cambie, actualizar `?v=AAAAMMDDHHMM`** en el enlace de todas las páginas (caché de GitHub Pages: 10 min).
- Enlaces: se configuran en el bloque `const ENLACES = {...}` de cada página. Páginas de Canvas → `target="_top"`; externas → `_blank`. Vacío = la tarjeta no navega («Próximamente»).
- Tarjetas: modelo numerado (número en Playfair 600 con subrayado celeste 3px, título Playfair 500, enlace «Ver… →»), sin filete lateral. Frambuesa (#cf2359) solo para etiquetas/antetítulos; azul para la estructura.
- Fichas emergentes (modal) con el modelo del catálogo de herramientas: cabecera azul noche, cuerpo blanco; al cerrar se detiene el vídeo.
- Vídeos: YouTube como `youtube-nocookie.com/embed/ID`; Kaltura UFV público `https://cdnapisec.kaltura.com/p/2615412/embedPlaykitJs/uiconf_id/54497012?iframeembed=true&entry_id=…&config…widgetId…`; los enlaces `external_tools/retrieve` de Canvas NO funcionan fuera de Canvas.
- PDFs de Canvas: quitar `/download?download_frd=1` y dejar `?verifier=…` para que se vean en el visor sin descarga.
- Altura del iframe: medir la página a 820 px de ancho y redondear hacia arriba (+30 px). Dar siempre el iframe con `?v=N` cuando haya que forzar la recarga.
- Antes de subir, previsualizar como artefacto (CSS en línea, vídeos sustituidos por un recuadro) cuando la usuaria lo pida.
- Commits en español; la usuaria trabaja en Windows (recargar con Ctrl+F5).

## Páginas
| Carpeta | Página | Canvas |
|---|---|---|
| `portal/` | Entrada: Portal de IA y Competencias Digitales Docentes (2 tarjetas) | — |
| `index.html` | Portada «Espacio de Formación Permanente en IA» (5 ámbitos + banner de ayuda a Teams) | pages/portal-ia |
| `comprender-ia/` | 01 Comprender la IA y utilizarla con criterio | pages/01-comprender-la-ia-y-utilizarla-con-criterio |
| `herramientas-gemini/` | 02 Adopción de herramientas de Gemini | pages/02-adopcion-de-herramientas-de-gemini |
| `experiencias-uso/` | 03 Explorar experiencias de uso UFV con Gemini (5 experiencias, datos en `const EXPERIENCIAS`; iframe 1250) | pages/06-explorar-experiencias-de-uso |
| `evaluacion-ia/` | 04 Guía «La evaluación UFV en tiempos de IA» (archivo de la usuaria, integrado tal cual; iframe 9000) | pages/04-evaluacion-ufv-en-tiempos-de-ia |
| `acompanar-alumnos/` | 05 Acompañar a mis alumnos | pages/05-acompanar-a-los-alumnos |
| `ia-is-in-the-air/` | Ciclo de webinars (3 vídeos Kaltura en pestañas) | pages/ciclo-ia-is-in-the-air |
| `ia-ola-o-tsunami/` | Conferencia Jon Hernández (YouTube) | pages/ia-ola-o-tsunami |
| `educacion-conciencia-razon/` | Conferencia Francesc Torralba (YouTube) | pages/educacion-universitaria-conciencia-y-razon-en-tiempos-de-inteligencia-artificial |
| `ciclo-instituto-newman/` | Instituto John Henry Newman (2 vídeos YouTube) | pages/ciclo-instituto-newman |
| `red-subterrania/` | La Red SubterranIA (vídeo Kaltura + texto) | pages/la-red-subterrania |
| `que-piensan-alumnos/` | ¿Qué piensan los alumnos? (telas de araña por facultad en modal + World Café → vista previa en Canvas) | pages/que-piensan-los-alumnos-sobre-la-ia |
| `pildoras-formativas/` | Píldoras formativas (10 vídeos en modal, datos en `const PILDORAS`) | pages/pildoras-formativas |

**`evaluacion-ia/` NO SE TOCA**: es la misma guía del proyecto, ya integrada y compilada con las imágenes incrustadas.
La página de Canvas «Formación para diseñar actividades y experiencias de aprendizaje» queda fuera del portal (sin tarjeta en ningún sitio). La arquitectura actual es la definitiva.

Páginas de ámbito 01–05: enlace «← Volver» (hero y pie) a `pages/portal-ia?module_item_id=1539063`.
