---
name: ecoweb-carousel-generator
description: Genera carruseles de Instagram/Facebook con el branding exacto de EcoWeb (colores, tipografías, logo) y elementos visuales ilustrados consistentes (silla dental, celular con WhatsApp, calendario, reloj, etc.) a partir de un guion o ángulo ya definido. Úsala SIEMPRE que el usuario pida "hacer un carrusel", "diseñar slides para Instagram" o "convierte este ángulo en carrusel". No la uses para generar el guion o el copy del carrusel: esta skill SOLO diseña y renderiza las slides finales listas para subir.
---

# EcoWeb Carousel Generator

Convierte un guion de carrusel (texto por slide, ya escrito) en imágenes
finales con el branding real de EcoWeb: colores exactos, tipografías Syne +
DM Sans, logo, y una librería reutilizable de ilustraciones on-brand.

Esta skill NO escribe el copy. Si el usuario no trae un guion ya armado,
ayúdale a armarlo en conversación antes de entrar al diseño, partiendo de
una base temática de `context/content/briefs/` y de la etapa que le toque
según `context/estrategia/distribucion-semanal.md`.

## Flujo de trabajo

1. **Recibe el guion**: texto por slide (título/hook, cuerpo, o dato), y el
   ángulo general (de qué pilar sale, qué emoción busca).
2. **Elige la plantilla de cada slide** según su función (ver sección
   "Plantillas de slide" abajo).
3. **Elige o genera la ilustración** que acompaña cada slide que lo
   requiera (ver "Librería de ilustraciones").
4. **Arma el HTML de cada slide** usando `references/template.html` como
   base, con las variables de texto e ilustración sustituidas.
5. **Renderiza cada HTML a PNG** a 1080×1350 px (formato 4:5, el que mejor
   rinde en el feed de Instagram) usando el script de render.
6. **Entrega las imágenes numeradas** (`01.png`, `02.png`, ...) en
   `output/<nombre-carrusel>/` junto con el copy de la descripción/caption
   si el usuario lo pidió.
7. **Presenta los archivos** al usuario con `present_files` — nunca dejes
   el resultado solo en el filesystem sin mostrarlo.

## Design tokens (usar SIEMPRE estos valores exactos, nunca aproximar)

```css
--eco-green:   #1DB86B;  /* acento principal, CTAs, iconos, datos */
--forest-deep: #0F6E56;  /* hover / variante oscura del verde */
--deep-violet: #262033;  /* fondo oscuro, texto sobre claro */
--mist-white:  #F5F7F5;  /* fondo claro */
--red-alert:   #E53E3E;  /* solo para cifras de pérdida/dolor, nunca decorativo */
--gray-text:   #666666;  /* texto secundario sobre fondo claro */

--font-display: 'Syne', sans-serif;   /* títulos, cifras grandes, siempre bold 700-800 */
--font-body:    'DM Sans', sans-serif; /* cuerpo de texto, peso 400-500 */

--slide-size: 1080px × 1350px;  /* formato 4:5, feed de Instagram */
--safe-margin: 80px;            /* nada de texto ni iconos fuera de este margen */
```

No uses ningún otro color, ni gradientes que no estén en esta paleta, ni
tipografías distintas. Si una slide se ve "vacía", resuélvelo con espacio
en blanco o con una ilustración de la librería, nunca agregando un color
o fuente nueva.

## Plantillas de slide

Cada slide del carrusel cumple UNA función. No mezcles dos funciones en
la misma slide.

### 1. Portada / Hook (siempre la slide 1)
- Fondo `--deep-violet`
- Ilustración grande centrada arriba (línea, color `--eco-green` sobre
  fondo oscuro)
- Título en `--font-display`, bold 800, blanco, 64-80px, máximo 2 líneas
- Sin cuerpo de texto adicional — la portada solo detiene el scroll

### 2. Dato / Cifra
- Fondo `--mist-white`
- Cifra enorme en `--font-display`, 120-160px, color `--eco-green`
  (o `--red-alert` si la cifra es una pérdida/dolor)
- Texto de contexto debajo, `--font-body`, 28-32px, color `--gray-text`
- Ilustración pequeña opcional en una esquina, nunca compitiendo con la
  cifra

### 3. Narrativa / Problema
- Fondo alterna entre `--mist-white` y `--deep-violet` slide por slide
  para dar ritmo visual al deslizar
- Texto en `--font-body`, 36-42px, máximo 4 líneas por slide
- Sin ilustración, o una muy sutil de fondo con baja opacidad

### 4. Comparación (tabla simple, 2 columnas)
- Fondo `--mist-white`
- Encabezados en `--font-display`
- Columna EcoWeb resaltada con borde izquierdo `--eco-green`
- Nunca más de 3-4 filas por slide — si hay más datos, se reparten en
  dos slides de comparación consecutivas

### 5. Checklist / Lista
- Fondo `--mist-white`
- Cada punto con un check circular verde (`--eco-green`) + texto corto
  `--font-body`, 32px
- Máximo 4-5 puntos por slide

### 6. CTA (siempre la última slide)
- Fondo `--deep-violet`
- Texto corto y directo en `--font-display`, blanco
- El CTA se toma de `context/estrategia/destino-y-ctas.md`. El carrusel es
  MOFU: puede cerrar con el lead magnet ("Comenta <PALABRA> y te mando el
  diagnóstico de tu clínica") O con guardar/compartir, según el objetivo de
  esa pieza. **Varía: no todos los carruseles piden la palabra**
- Logo de EcoWeb pequeño, abajo, siempre presente en esta slide

## Librería de ilustraciones

EcoWeb necesita ilustraciones **propias y consistentes entre sí**, no
iconos de stock genéricos. Estilo: línea limpia, un solo trazo grueso,
paleta de dos tonos (`--eco-green` sobre `--deep-violet` o
`--deep-violet` sobre `--mist-white`), sin relleno de color sólido salvo
detalles mínimos. El mismo estilo del logo de EcoWeb (nodos conectados en
verde sobre fondo oscuro).

### Ilustraciones que se usan con frecuencia — mantener una versión
guardada de cada una y REUTILIZARLA, no regenerarla cada vez:

- Silla dental (perfil, línea simple)
- Celular con burbuja de chat de WhatsApp
- Calendario con una fecha marcada
- Reloj marcando una hora nocturna (10-11 PM)
- Diente / muela estilizado
- Persona con signo de pesos o gráfica ascendente (para piezas de negocio)
- Recepcionista/escritorio vacío (para el ángulo de "8 horas vs 24/7")

**Cómo generarlas la primera vez:** si la ilustración que necesitas no
existe todavía en `assets/illustrations/`, generala con la herramienta de
imagen disponible en el proyecto, especificando explícitamente: "ilustración
de línea, un solo color de trazo, estilo minimalista geométrico, sin
sombreado, sin fondo (fondo transparente), que combine con un logo de
nodos conectados en verde sobre violeta oscuro". Revisa que el trazo sea
consistente en grosor con las ilustraciones ya existentes antes de
aceptarla. Guárdala en `assets/illustrations/<nombre-descriptivo>.png`
con fondo transparente para poder reutilizarla sobre fondo claro u oscuro
según la slide.

**Nunca regeneres una ilustración que ya existe en la carpeta** — reutilízala.
Esto es lo que mantiene el feed visualmente consistente entre carruseles
de semanas distintas. Antes de generar cualquier ilustración nueva, revisa
primero `assets/illustrations/` por si ya existe algo que sirva.

## Render de HTML a imagen

Usa `references/template.html` como base. Es un HTML+CSS autocontenido de
1080×1350px con las variables de marca ya cargadas como CSS custom
properties. Sustituye el contenido de texto e imagen por slide, y renderiza
cada una a PNG con un headless browser (Playwright/Puppeteer si están
disponibles en el entorno; si no, cualquier herramienta de captura de HTML
a imagen a la resolución exacta 1080×1350).

Verifica SIEMPRE después de renderizar:
- Que ningún texto se corte en el margen de seguridad de 80px
- Que el contraste de texto sobre fondo sea legible (blanco sobre violeta,
  violeta o gris oscuro sobre mist-white — nunca texto claro sobre claro)
- Que la resolución final sea exactamente 1080×1350px, no aproximada

## Qué NO hacer

- No inventar colores, gradientes o tipografías fuera de los tokens de
  marca definidos arriba
- No poner más de 40-45 palabras de texto en una sola slide (se vuelve
  ilegible en el feed)
- No usar iconos de stock (Flaticon, emojis grandes, clipart) — solo la
  librería de ilustraciones propia
- No generar una ilustración nueva si ya existe una que sirve para el
  mismo concepto en `assets/illustrations/`
- No repetir el mismo cierre en todos los carruseles. El lead magnet es uno
  de los CTAs disponibles, no el único (ver `context/estrategia/destino-y-ctas.md`)
- No mezclar dos funciones de slide (por ejemplo dato + checklist) en la
  misma imagen

## Verificación de datos antes de renderizar

Si el guion incluye una cifra o estadística, verifica contra
`context/data/datos-verificados.md` (o el archivo equivalente en el
proyecto) antes de ponerla en una slide de "Dato / Cifra". No renderices
una cifra que no esté en la lista de datos verificados sin confirmarlo
primero con el usuario.
