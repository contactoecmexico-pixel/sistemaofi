---
name: ecoweb-video-engine
description: Planea y escribe guiones de video para EcoWeb razonando desde el sistema de contenido (el árbol de temas, las 4 perillas, los movimientos, los hooks, la energía y los CTAs), no recitando reglas. Trabaja en dos modos, plan en lote y guion uno por uno, con el guion de oro como patrón de calidad. Se dispara cuando se pide planear videos, generar un banco de guiones, escribir un guion de TikTok, Reel o Short, o llenar el calendario de video.
---

# EcoWeb Video Engine

Convierte una intención en un guion **razonando el sistema**, no aplicando una plantilla. Cada guion se escribe una vez y se publica igual en TikTok, Instagram Reels y YouTube Shorts.

**Principio de esta skill:** el criterio vive en los documentos de `context/estrategia/`. Esta skill no los repite, los **orquesta**: dice en qué orden decidir, de dónde jalar cada cosa, y qué verificar antes de entregar. Si un guion sale estéril, casi siempre es porque se recitaron reglas en vez de razonar el orden de abajo.

| Modo | Qué hace |
|---|---|
| **PLAN** | Convierte un conjunto de intenciones en un lote de piezas, girando las 4 perillas. No escribe guiones |
| **GUION** | Escribe un guion completo, uno por vez |
| **CALIBRACIÓN** | Ajusta con base en resultados reales |

---

# 🔴 Cómo se piensa una pieza (el corazón)

Una pieza única sale de girar cuatro perillas, en este orden. **La intención primero, el tema al final.** Nunca al revés: empezar por el tema y pegarle intención encima es lo que volvía todo igual.

> **PILAR × FORMATO × MOVIMIENTO × INTENCIÓN = pieza única**

El proceso completo, paso a paso:

1. **Intención** — ¿qué quiero que el dentista *sienta* y *haga*? (`mapa-de-temas.md`, sección 2)
2. **Profundidad / etapa** — ¿ancho para alcance (TOFU) o hondo para el de máximo valor (BOFU)?
3. **Raíz y rama** — el tema, de una raíz que sirva a esa intención (`mapa-de-temas.md`, el árbol). Raíces de problema (1-5) o de conexión (6-8)
4. **Formato** — cuál de los 6 (`estrategia-de-contenido.md`)
5. **Movimiento** — el motor de razonamiento, de la familia que corresponde a la capa (`argumentos.md`): Revelación para problema, Postura para conexión, Prueba para conversión
6. **Energía** — el modo que coincide con la intención: íntimo, autoridad o convicción (`estrategia-de-contenido.md`)
7. **Hook** — los dos canales y el test de 4 filtros (`hooks.md`)
8. **CTA** — por etapa, con los tres destinos (`destino-y-ctas.md`)

**La regla de rotación, la que más importa:** no repitas la misma combinación de **pilar + formato**, ni el mismo **movimiento**, en piezas consecutivas. Aunque el tema cambie. Es lo que evita que todo suene igual, que era el problema de fondo del banco viejo.

**La regla de coherencia:** si la intención es de conexión o emocional, el guion no lleva cifras. Si es de autoridad, sí. Mezclar las dos las anula.

---

# 🔴 Las fuentes (única verdad — se leen, no se copian)

Antes de planear o escribir, se cargan. **El detalle vive aquí, no en esta skill.**

| Documento | Qué gobierna |
|---|---|
| `context/estrategia/estrategia-de-contenido.md` | Documento maestro: las 4 perillas, los 6 formatos con su reverse engineering, la energía (3 modos), la mezcla semanal |
| `context/estrategia/mapa-de-temas.md` | El árbol: raíces, ramas, intenciones, profundidad. De aquí sale el tema |
| `context/estrategia/argumentos.md` | Los 16 movimientos en 3 familias. El motor de razonamiento de la pieza |
| `context/estrategia/hooks.md` | El sistema de hooks: dos canales, test de 4 filtros, lo que la data probó |
| `context/estrategia/destino-y-ctas.md` | Los 3 destinos (engagement, carta, conversación) y el CTA por etapa y formato |
| `context/estrategia/guion-de-oro-anti-pitch.md` | El patrón de calidad. Se calibra contra este |
| `context/voice dna/voice-profile.md` · `context/brand/brand-guide.md` | Voz, tono, prohibiciones de formato |
| `context/data/datos-verificados.md` | Antes de usar cualquier cifra |
| `context/icp/audience-icp.md` | El dolor, los miedos, el lenguaje verbatim, las objeciones |
| `context/brand/product-context.md` · `positioning.md` · `pricing.md` | Qué hace y qué no el sistema, los ángulos, el ancla de precio |
| `output/videos/` + `aprendizajes.md` | Lo ya escrito (no repetir) y los errores medidos (no repetir) |

---

# 🔴 Los no-negociables

Los pocos invariantes de nivel skill. El resto del criterio está en los documentos.

1. **Regla Cero:** cada pieza parte de un dolor, miedo, pérdida, deseo o postura, no de un dato ni de una ficha de producto. El dato es soporte, nunca el tema. *Test: tapa las cifras. ¿Sigue doliendo? Si no, el dato era el tema.*
2. **Honestidad:** cifras solo de `datos-verificados.md`, cero casos o clínicas inventadas, cero promesas de resultado sin caso documentado. Es el diferenciador de la marca, no un detalle.
3. **Regla antitécnica:** el dentista no sabe ni le importa lo técnico. Cero jerga (n8n, API, modelo, integración). Todo en beneficios.
4. **El precio puede vivir en un video BOFU, en la carta y en la conversación, nunca en TOFU ni MOFU.** Un BOFU sí puede hablar de precio (por ejemplo, el costo anual del sistema contra el de una recepcionista), siempre anclado contra el costo de la alternativa, anual contra anual con cargas, y nunca minimizado (`voice-profile.md`, `pricing.md`).
5. Nunca la palabra "demo". Nunca el guion largo (—). Español de México, tuteando.
6. Una sola idea por pieza. El mismo guion va igual a las tres plataformas.

---

# 🔴 Lo que la data ya probó (tratar como ley)

Detalle completo en `aprendizajes.md`. En corto, para no re-descubrirlo:

- **Historia gana a Autoridad ~4x en alcance.** Revela una pérdida en curso, no expliques un concepto.
- **Ancla temporal obligatoria** (anoche, tu semana pasada, este lunes). Sin ella, solo te escuchan.
- **El título visual abre intriga y no la resuelve.** Los videos 13 y 16 se cayeron por resolverla en el segundo 0.
- **Guion escrito = guion grabado.** La palanca más grande y la más barata. 4 de 4 fracasos fueron desviaciones al grabar, no del guion.
- **Skip base del banco: 31-32%.** La marca a batir.
- **Compartir por DM es la señal más fuerte y la menos usada.**

---

# MODO PLAN

Convierte un conjunto de intenciones en un lote de piezas girando las 4 perillas. No escribe guiones.

1. **Define el objetivo del lote** con el usuario: ¿qué mezcla de intenciones y etapas? La proporción sale de `estrategia-de-contenido.md` (la mezcla) y de qué pilares están sub o sobreproducidos (`mapa-de-temas.md`, `output/videos/`).
2. **Elige ramas del árbol** que sirvan a esas intenciones, no marcadas como usadas.
3. **Asigna las 4 perillas a cada pieza**, aplicando la rotación (no repetir pilar+formato ni movimiento consecutivos).
4. **Propón un hook** por pieza (calibre, no definitivo).
5. **Entrega el mapa:** una tabla con ID · raíz/rama · intención · etapa · formato · movimiento · energía · hook propuesto · CTA.

Guardar en `output/videos/[slug]/00-plan.md`. Presentar y esperar visto bueno antes de escribir guiones.

**Producción:** el usuario decidió **no grabar por lotes** (la energía baja y los videos se parecen). El plan agrupa por tema y perillas para pensar, no para grabar en cadena.

---

# MODO GUION

Uno por vez. Guardar en `output/videos/[slug]/[ID]-[tema].md`.

### Paso 0 — Bloque de reverse engineering
Antes de escribir, declarar las decisiones (como el encabezado del guion de oro): pilar/raíz, formato, movimiento, intención, etapa, energía, CTA. Si no se puede llenar, no está pensada la pieza.

### Paso 1 — Tres hooks candidatos
Proponer 3 hooks para la rama y etapa ya elegidas, cada uno con su "por qué funciona". Los tres pasan el test de 4 filtros de `hooks.md` (Novedad, Relevancia, Vacío, Reconocimiento, mínimo 14/20) y los dos canales (verbal + título visual que no resuelve). El usuario elige uno.

### Paso 2 — Escribir el guion
Formato de dos columnas, como el guion de oro: **Voz** (lo único que se lee, palabra por palabra) y **Dirección** (encuadre, energía, ritmo; nunca se lee). Estructura:

```
HOOK → DESARROLLO (mini-hooks) → PAYOFF (~79%) → CIERRE
```

- Payoff después del 70%.
- Mínimo 3 mini-hooks, cada 15-20 segundos.
- Energía marcada por beat (dónde te acercas, dónde bajas el ritmo).
- Cierre por etapa (`destino-y-ctas.md`): TOFU sin venta, MOFU variado, BOFU a la carta o a la conversación. A veces el mejor cierre es el remate, sin CTA.
- Duración por conteo de palabras: 150-165 wpm. Rango 60-110 segundos. Reportar el número.
- Cerrar con la frase citable (el remate de `argumentos.md`).

### Paso 3 — Checklist de entrega (reportar en dos líneas)
- [ ] Las 4 perillas declaradas y coherentes entre sí (intención emocional → sin cifras)
- [ ] Rotación respetada respecto a la pieza anterior (pilar+formato y movimiento)
- [ ] Regla Cero: parte del dolor/postura, no del dato
- [ ] Hook pasa los 4 filtros y no resuelve la intriga (verbal y título visual)
- [ ] Un solo movimiento, de la familia correcta para la capa
- [ ] Ancla temporal concreta (cuando la etapa/intención lo pide)
- [ ] Payoff después del 70% · mínimo 3 mini-hooks · energía coherente con la intención
- [ ] CTA de la etapa, sin repetir el de los últimos guiones · precio fuera de TOFU
- [ ] Cifras solo de `datos-verificados.md` · sin casos inventados · sin "demo" · sin guion largo · tuteo MX
- [ ] Conteo de palabras dentro del rango

### Paso 4 — Calibrar contra el guion de oro
La prueba final: dado el tema y la intención, ¿este guion toma las mismas decisiones de criterio que `guion-de-oro-anti-pitch.md` (familia de movimiento correcta, energía coherente, hook que no resuelve, CTA de la etapa, honestidad real)? Si cumple el checklist pero se siente estéril, todavía no razonó, reescribir.

---

# 🔴 Guion escrito = guion grabado

Antes de diagnosticar un mal resultado, comparar el guion escrito contra la transcripción real del video. 4 de 4 fracasos del banco fueron desviaciones al grabar (beat fusionado, mini-hook perdido, hook cambiado, título visual que resolvió la intriga), no fallas del guion.

Cuando lleguen métricas peores de lo esperado, preguntar primero: *"¿me pasas el guion tal como quedó grabado?"* No asumir que coincide. El checklist de fidelidad antes de grabar está en `hooks.md` y en la disciplina de ejecución de `estrategia-de-contenido.md`.

---

# 🔴 Control de trayectoria

Cada 3 guiones nuevos, antes de seguir: *"¿Cuáles ya grabaste o publicaste? ¿Falta grabar alguno de la tanda anterior?"* Si algo quedó pendiente de grabar, no generar más hasta aclarar. Acumular guiones sin grabar no ayuda, solo llena papel.

---

# MODO CALIBRACIÓN

| Señal | Diagnóstico | A dónde ir |
|---|---|---|
| Se caen antes del segundo 3 | El hook no segmenta, resuelve la intriga, o abre estático | `hooks.md` |
| Se caen entre el 10 y el 30 | Falta un mini-hook ahí | La estructura, arriba |
| Ven completo pero no interactúan | El cierre no pide bien | `destino-y-ctas.md` |
| Ven completo pero no hay clics | El link no se mencionó claro | `destino-y-ctas.md` |
| Muchos guardados | Ese movimiento y esa raíz funcionan, profundiza | `mapa-de-temas.md` |
| Muchos comentarios de "ese soy yo" | La postura o el anti-pitch pega, haz más | `argumentos.md` |

Registrar en `output/videos/[slug]/aprendizajes.md`. Si un movimiento o formato falla dos veces grabado tal cual se escribió, proponer reemplazarlo.

---

# Qué NO hace esta skill

- **No recita el criterio: lo lee de los documentos.** Si algo de hooks, CTAs, movimientos o formatos no está claro, se va al documento, no se improvisa aquí.
- No diseña ni escribe carruseles → `ecoweb-carousel-writer` y `ecoweb-carousel-generator`.
- No define la estrategia ni la mezcla → `context/estrategia/`.
- No toca la conversación de venta ni la carta → fuera de alcance, ver `embudo.md`.
