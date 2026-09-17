# EcoWeb — Pilares de contenido
**Versión 2.0 · Agosto 2026 · VIGENTE**

> Los pilares siguen siendo los mismos temas. Lo que cambia: se re-mapean a etapa del embudo (ya no a mes del calendario), y el Pilar 4 se reformula porque no hay casos de clientes todavía.
>
> ⚠️ **Pilar 5 eliminado (septiembre 2026).** "Pacientes que no vuelven" describía una función de recall/reactivación automática que el sistema no tiene — `product-context.md` solo confirma agendar, reagendar, cancelar y dos recordatorios sobre citas ya programadas, no campañas a pacientes inactivos. Se retira del banco de temas por completo, no solo se pausa.

---

## Mapa

| Pilar | Tema | Etapa | Estado |
|---|---|---|---|
| **1 — El dinero que se escapa** | No-shows, pacientes perdidos fuera de horario, costo de recepcionista | **TOFU** | Activo · sobreproducido |
| **3 — El dentista como dueño de negocio** | Gestión, rentabilidad, escalar sin contratar | **TOFU / MOFU** | Activo · el más diferenciador |
| **2 — Cómo funciona en la práctica** | Qué hace y qué no hace el asistente, sin jerga | **MOFU (núcleo)** | Activo · **sin producir** |
| **4 — Prueba y decisión** | Demostración, objeciones, garantía, comparativas | **BOFU** | Reformulado · **sin producir** |

---

## Pilar 1 — El dinero que se escapa <span>TOFU</span>

El dolor #1 del Dr. Roberto, y el único que es calculable hoy mismo. Nombra el problema y lo cuantifica.

**Fuentes:** `briefs/base-costo-no-show.md`, `briefs/base-fugas-de-dinero.md`, `datos-verificados.md`

⚠️ **Está sobreproducido.** Los 9 videos y 2 de los 3 carruseles existentes salen de aquí. No es que el pilar esté agotado, es que la mezcla está desbalanceada. Ver `distribucion-semanal.md`.

---

## Pilar 3 — El dentista como dueño de negocio <span>TOFU / MOFU</span>

El territorio emocional más profundo, y **el más diferenciador**: todos los competidores hablan de chatbots, ninguno le habla al dentista como empresario.

No habla de tecnología, habla de su vida: recuperar tiempo, crecer sin contratar, dejar de sentir que todo depende de él. Se comparte porque valida cómo se siente.

**El miedo raíz que toca:** *"estudié seis años para ser dentista y me la paso administrando."*

**Fuentes:** `audience-icp.md` (escalera de dolor, lenguaje verbatim, job stories), `positioning.md`

---

## Pilar 2 — Cómo funciona en la práctica <span>MOFU · núcleo</span>

**Es el núcleo del MOFU y no se ha producido ni una pieza.** Los competidores muestran features; nadie le explica al dentista qué pasa exactamente el día que se instala, qué configura él y qué hacemos nosotros.

Habla a dos miedos concretos: el de implementación y el de perder el control de la comunicación con sus pacientes.

**Material disponible sin escribir, en `product-context.md`:**
- Los 6 pasos de instalación (levantamiento → configuración → entrenamiento → pruebas → go-live acompañado → seguimiento día 1, 3, 7, 14 y 30)
- Qué hace: agenda verificando disponibilidad real, dos recordatorios (día anterior y mismo día), reagenda, procesa imágenes
- **Qué NO hace:** diagnósticos, consejo clínico, interpretar síntomas, descuentos fuera de lo cargado. La honestidad sobre los límites es lo que genera confianza
- Las reglas de escalamiento: paciente molesto, urgencia, comprobante de pago, petición explícita
- Lo que necesita la clínica, incluido el punto conflictivo del número de WhatsApp

**Fuentes:** `product-context.md`, `briefs/base-chatbot-vs-recepcionista.md`

---

## Pilar 4 — Prueba y decisión <span>BOFU</span> 🔄 REFORMULADO

**Antes era "Resultados reales": casos de éxito con métricas.** Como no hay casos de clientes documentados, ese pilar estaba bloqueado y el BOFU se quedaba vacío.

**Ahora el BOFU se produce sin prueba social**, con cuatro vetas que sí existen hoy:

### 1. Demostración del bot en vivo
Prueba de capacidad, no prueba social. EcoWeb tiene un bot público probable en 30 segundos sin registro — ningún competidor tiene eso. *"Léelo tú. Así habla con tus pacientes."*

### 2. Manejo de objeciones
Cada objeción real es una pieza. Las documentadas en `audience-icp.md`:
- "¿Y si dice algo mal?" / "no quiero que suene robótico y espante a mis pacientes"
- "¿Mis pacientes van a odiar hablar con una IA?"
- "¿Y si agenda mal y hago doble reserva?"
- "Es caro" / "¿por qué pagar $24,000 antes de ver un resultado?"
- "Mi recepcionista ya lo hace"

### 3. La garantía como remoción de riesgo
El 50/50: mitad al arrancar, mitad cuando el sistema ya esté funcionando. Sin contrato de permanencia. Responde a la objeción del setup, que es la principal.

### 4. Comparativas honestas
- Sofía vs. recepcionista → `briefs/base-costo-recepcionista.md`
- Sofía vs. chatbot de menú (el de botones que todos conocen y odian)

> **Cuando exista el primer cliente documentado, los casos reales se agregan a este pilar.** El outreach existe en parte para desbloquear eso — ver `outreach.md`.

---

## Nota de voz editorial

- **Abrir con el dolor, no con la solución.** Los primeros segundos tienen que hacerlo sentir entendido
- **Resultados en pesos, no en porcentajes genéricos.** "Reduce un 40%" no dice nada
- **Sin jerga de IA.** El sistema "entiende lo que escribe el paciente", no usa "modelos de lenguaje"
- **Tuteo consistente.** "Tu clínica", nunca "las clínicas"
- **"Sin que toques nada"** es el posicionamiento, y se refuerza en todo
