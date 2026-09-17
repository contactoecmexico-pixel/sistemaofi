---
name: ecoweb-carousel-writer
description: Escribe el copy slide por slide de un carrusel de Instagram/Facebook para EcoWeb — el texto de cada slide, no el diseño. Se dispara cuando se pide escribir un carrusel, redactar las slides, convertir una unidad atómica en carrusel, o dar el guion de texto que luego pasa a diseño. El resultado alimenta directamente a `ecoweb-carousel-generator`, que SOLO diseña y renderiza — nunca escribe copy.
---

# EcoWeb — Escritor de Carruseles

Convierte una unidad atómica en el copy completo de un carrusel: portada, contexto, cuerpo y cierre, listo para pasar a `ecoweb-carousel-generator` para diseño y render.

**Esta skill NO diseña ni renderiza.** No elige colores, tipografías ni ilustraciones — eso es trabajo de `ecoweb-carousel-generator`. Esta skill entrega texto por slide, con la función de cada una ya decidida.

---

## Contexto obligatorio

Leer antes de escribir cualquier carrusel:

1. `context/estrategia/embudo.md` — el destino y las dos fases
2. `context/estrategia/pilares.md` — la etapa de cada pilar
3. `context/estrategia/destino-y-ctas.md` — el CTA por etapa y formato
4. `context/content/briefs/` — la base temática de la que sale la unidad
5. `context/voice dna/voice-profile.md` y `context/brand/brand-guide.md`
6. `context/icp/audience-icp.md` — dolor, miedos, lenguaje verbatim
7. `context/data/datos-verificados.md` — antes de usar cualquier cifra
8. `output/videos/*/aprendizajes.md` — errores ya identificados en otros formatos, para no repetirlos aquí

---

# 🔴 REGLA CERO: todo sale del dolor del ICP

Idéntica a `ecoweb-video-engine`. Cada carrusel parte de un dolor, pérdida, miedo o deseo documentado en `audience-icp.md` — no de una estadística suelta ni de una ficha de producto. El dato es soporte, nunca el tema.

**El test:** tapa las cifras del carrusel. ¿Sigue doliendo? Si sin el dato el carrusel se queda sin tema, el dato era el tema. Reescribir desde el dolor.

---

# 🔴 EL TONO: observación de colega

Misma tabla que el video-engine. No se advierte al lector, se observa algo del gremio y se deja que se identifique solo.

| ❌ Advertir | ✅ Observar |
|---|---|
| "Si tienes consultorio, esto te va a incomodar" | "A los dueños de consultorios casi no les cuentan bien lo que cuesta su agenda vacía" |

Frases cortas. Sin dramatización. Coloquial. Sin justificar de más — si algo se explica en una línea, no van tres.

---

# 🔴 REGLA ANTITÉCNICA

El lector es un dentista dueño de su consultorio. No sabe nada técnico y no le importa saberlo. Nunca nombrar herramientas ni procesos (n8n, API, integración, modelo de lenguaje). Traducir siempre proceso → beneficio. Misma tabla y mismo test que `ecoweb-video-engine`.

---

# LEYES DURAS (heredadas del video-engine, validadas con datos)

Aplican igual al carrusel — la unidad atómica es la misma independientemente del formato en que se publique.

**LEY 1 — Revela una pérdida en curso, nunca expliques un concepto.** El carrusel debe hacer sentir al dentista que algo se le está escapando mientras desliza, no solo enseñarle algo nuevo. Si el carrusel "explica" un concepto en vez de revelar una fuga activa, la unidad está mal elegida.

**LEY 2 — Ancla temporal obligatoria.** El carrusel manda al lector a un momento concreto y reciente de su propia operación: *tu semana pasada, anoche, este lunes.* Nunca una pérdida abstracta.

Ambas son condición de entrega, no filtro opcional: si un carrusel no las cumple, no se entrega, se reescribe.

---

# LA ESTRUCTURA DE CUATRO ZONAS

Todo carrusel tiene cuatro zonas con un trabajo distinto cada una. No se saltan ni se fusionan.

## Zona 1 — Portada (slide 1)

Es el hook. Debe ganar el swipe por sí sola — si esta slide corriera como pieza suelta, ¿pararía el scroll?

- Título corto y de máximo contraste, legible en miniatura
- Sigue el mismo examen que el hook hablado del video-engine: contexto + curiosidad + número cuando aplique
- Pasa el test de las dos preguntas: ¿de quién? (dentista/consultorio/clínica dental) y ¿de qué? (agenda, citas, pacientes, recepcionista, WhatsApp)

**Se escribe al final, no al principio.** Una vez que sabes exactamente qué entrega el carrusel completo, puedes escribir la portada que cumple esa promesa exacta — no antes, porque si no, el hook promete algo que las slides internas no sostienen.

## Zona 2 — Contexto (slide 2)

El puente entre el hook y el valor. Es la slide que más se salta por error, y no se puede saltar.

- Una o dos frases que plantan el escenario o nombran por qué esto importa
- Ancla temporal (LEY 2) si no quedó ya en la portada

## Zona 3 — Cuerpo (slides 3 a N-1)

El desarrollo. Cada slide toca un solo punto de la unidad atómica — nunca dos ideas en una slide.

- Máximo 40-45 palabras por slide (límite compartido con `ecoweb-carousel-generator`, que rechaza slides más densas)
- **Si el punto no cabe en el límite, se parte en dos slides — nunca se aprieta el texto**
- **Cada slide de cuerpo cierra en gancho hacia la siguiente, nunca en punto final resuelto.** La última palabra debe hacer que deslizar a la próxima se sienta necesario: un número sin completar ("y todavía falta lo que nadie suma"), una pregunta que la siguiente slide responde, una idea a medias. Esto es lo que sostiene el deslizamiento entre slides, distinto del hook de portada que solo gana el primer swipe

## Zona 4 — Cierre / CTA (última slide)

Cierre calibrado por etapa — el carrusel es predominantemente MOFU (quien desliza 8-10 slides ya invirtió atención y aguanta un paso con más compromiso), pero el cierre exacto varía:

- **Lead magnet:** "Comenta [PALABRA] y te mando el diagnóstico de tu clínica" — uno de los CTAs disponibles, no el único
- **Guardar/compartir:** cuando el objetivo de esa pieza es autoridad o alcance, no conversión directa
- **Nunca repetir el mismo cierre en carruseles consecutivos.** Ver `context/estrategia/destino-y-ctas.md` para la variedad completa por etapa

---

# LOS CINCO FORMATOS — elegir antes de escribir, no después

El formato ordena cómo se reparte la unidad atómica entre las slides de cuerpo. Se decide en cuanto se elige la unidad, no a medio guion.

| Formato | Estructura | Cuándo usarlo | Ejemplo de base propia que ya calza |
|---|---|---|---|
| **Listicle** | "N [fugas/errores/señales]" — una por slide | La unidad ya es una lista natural | `base-fugas-de-dinero.md` — las 5 fugas, una por slide |
| **Framework** | Proceso paso a paso, progresión numerada | Enseñar un método o una secuencia | Los 6 pasos de instalación de Sofía |
| **Contraste** | Slides alternando "sin sistema" / "con sistema" | Reforzar la diferencia antes/después | Recepcionista vs. sistema (Carrusel 02 ya usado) |
| **Dato/Cifra** | Un número sorprendente por slide + una línea de sentido | La unidad es de pérdida financiera directa (Pilar 1) | El costo real de un no-show |
| **Mini caso** | Problema → cálculo → hallazgo, en 2-3 slides | Cuando hay un cálculo en vivo que contar como historia | Video 01 adaptado a slides ("un consultorio de dos sillones...") |

No mezclar dos formatos en un mismo carrusel. Si la unidad no calza limpio en ninguno, es señal de que la unidad está mal recortada — volver a `context/content/briefs/` antes de forzarla.

---

# VERIFICACIÓN OBLIGATORIA

- [ ] **El carrusel toca UNA sola unidad atómica** — no combina dos bases ni dos pilares
- [ ] **LEY 1: revela una pérdida en curso, no explica un concepto**
- [ ] **LEY 2: ancla temporal concreta y reciente**
- [ ] **La portada pasa el test de las dos preguntas** (¿de quién? ¿de qué?) y se escribió al final
- [ ] **Ningún slide de cuerpo supera 40-45 palabras** — si se pasa, se parte en dos
- [ ] **Cada slide de cuerpo cierra en gancho hacia la siguiente**, salvo la última
- [ ] **El formato se decidió antes de escribir**, y es uno solo de los cinco
- [ ] **El cierre no repite el de los últimos carruseles publicados**
- [ ] **Regla antitécnica: cero nombres de herramientas o procesos técnicos**
- [ ] **Cifras dentro de `datos-verificados.md`** — ninguna cifra nueva sin verificar primero
- [ ] **Sin "demo", sin hipérbole, sin dramatización**
- [ ] **No inventa casos, clínicas ni fuentes**
- [ ] **Español de México, tuteando**

Reportar el formato elegido y el check en dos líneas al entregar.

---

# HANDOFF A ECOWEB-CAROUSEL-GENERATOR

El output de esta skill es el input directo del generador. Entregar en este formato exacto, uno por slide:

```markdown
### Carrusel — [nombre-slug]
**Unidad atómica:** [la unidad de la que sale]
**Formato:** [Listicle / Framework / Contraste / Dato-Cifra / Mini caso]
**Etapa:** MOFU (u otra si aplica) · **Pilar:** [número]

---
Slide 1 (Portada)
Título: [texto]

---
Slide 2 (Contexto)
[texto]

---
Slide 3 ([función: Dato / Narrativa / Comparación / Checklist según corresponda])
[texto — bajo 40-45 palabras]

---
[continuar para todas las slides]

---
Slide N (CTA)
Cierre: [texto del cierre elegido, calibrado a la etapa]
```

La etiqueta de función en cada slide de cuerpo (Dato / Narrativa / Comparación / Checklist) debe coincidir con una de las plantillas visuales que ya existen en `ecoweb-carousel-generator`, para que el generador sepa qué plantilla aplicar sin tener que adivinar.

---

## Cuándo decir que no

- Si la unidad atómica no da para 8-10 slides sin relleno — mejor un carrusel corto y honesto que uno estirado
- Si dos formatos calzan igual de bien — elegir el que ya se haya usado menos en el banco reciente, para variar

---

## Qué NO hace

- No diseña ni renderiza — eso es `ecoweb-carousel-generator`
- No escribe guiones de video ni hooks hablados → `ecoweb-video-engine`
- No escribe copy de landing ni mensajes → `ai-copywriter`
- No define la estrategia ni la mezcla semanal → `context/estrategia/`
