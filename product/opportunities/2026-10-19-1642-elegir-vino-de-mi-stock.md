---
status: framed
segment: Aficionados al vino con 10 o más botellas que, al menos de vez en cuando, deben decidir cuál abrir para una ocasión — desde quien recibe gente seguido hasta quien acumula botellas regaladas y sabe poco de vino
personas: carolina-mendez, tomas-rivas, lucas-fernandez, elena-valdivia
---

# Oportunidad: Elegir qué vino de mi stock abrir para cada ocasión

Los aficionados con 10+ botellas en casa eligen mal qué botella propia abrir para
una comida u ocasión —abren "la más a mano", una de guarda en una ocasión cualquiera,
o compran otra— porque no saben bien qué tienen ni qué combina con el plato; las
herramientas actuales (Vivino, buscadores, ChatGPT) registran vinos o dan maridajes
genéricos, pero no responden "cuál de *mis* botellas abro hoy".

## Segmento y personas

- Carolina Méndez (primary) — sufre el problema: frecuente, con costo concreto (botellas de guarda desperdiciadas, compras repetidas).
- Tomás Rivas (secondary) — sufre el problema, de forma esporádica: teme abrir "la cara" en la ocasión equivocada. Incluido en el segmento por decisión del fundador.
- Lucas Fernández (tertiary) — no lo sufre; lo causa (retira botellas sin registrar) y opina sobre el gasto del hogar → informa la viabilidad.
- Elena Valdivia (negative) — no lo sufre en esta forma; elige con rigor experto. Fuera de alcance.
- Faltante: ninguna.

Nota: el segmento combina dos subgrupos (recibe gente con frecuencia / botellas
regaladas y poco conocimiento); la investigación debe distinguirlos.

## Señales

| Señal | Provenance | Fuente |
|---|---|---|
| El fundador abandonó Vivino porque no recomienda según su propio stock, y AppSheet porque la carga era manual y no recomendaba | real (n=1, fundador) | conversación `/start-product` |
| El fundador pierde tiempo buscando físicamente si tiene más de una unidad de una botella | real (n=1, fundador) | conversación `/frame-opportunity` |
| Es difícil encontrar maridaje para el plato específico de la ocasión | unverified | investigación previa del fundador, sin fuente nombrada |
| Carolina abre "la más a mano" y desperdicia botellas de guarda | synthetic | product/personas/carolina-mendez.md |
| Tomás no sabe cuáles de sus botellas regaladas son buenas | synthetic | product/personas/tomas-rivas.md |
| Los maridajes de ChatGPT/Google son genéricos y no dicen cuál botella *propia* abrir | synthetic | Carolina, Tomás |

## Resultado de negocio

Comercial. Principal: **retención** — que el usuario siga pidiendo recomendaciones
y actualizando su stock después de 2–3 meses (el patrón observado es el abandono de
herramientas). Secundario: **conversión a pago** de una parte de los retenidos.

## Restricciones

- Horizonte: ~6 meses (hasta abril de 2027), sin fecha límite externa.
- Presupuesto: ≈ CLP 10.000.000 en 6 meses (estimación del fundador, sin desglose).
- Construcción: low code deseable, no obligatorio; el fundador construye sin equipo de desarrollo dedicado.
- Costo variable: el consumo de recursos por recomendación (p. ej., tokens de IA) debe caber dentro del ingreso esperado por usuario (≈ USD 2–4 al mes, creencia 5 del overview).

## Creencias

Referencias a product/overview.md — el registro único de creencias.

- [product] [value] (creencia 2 del overview, reutilizada) Los aficionados con 10+ botellas tienen, al menos un par de veces al mes, la duda de cuál de sus propias botellas abrir para una comida, y hoy la resuelven mal.
- [opportunity: elegir-vino-de-mi-stock] [viability] (creencia 3 del overview) Al menos el 40% de quienes reciban recomendaciones basadas en su propio stock sigue pidiéndolas al menos 2 veces al mes después de 3 meses — claramente más de lo que retuvieron Vivino u otros registros abandonados. *(Umbral inicial; revisar con benchmark.)*
- Relacionadas: creencia 1 del overview (la carga del stock como causa del abandono) y creencia 5 (precio).

## Agenda de investigación

| Creencia | Instrumento | Decisión que desbloquea | Para cuándo |
|---|---|---|---|
| Creencia 2 (el problema existe y es frecuente) | 1) `/research-market`: foros, grupos y reseñas de apps de vino que pidan "qué abro de lo que tengo" | Si hay señales externas, seguir; si no hay ninguna, reconsiderar el foco | mediados de nov. 2026 |
| Creencia 2 | 2) `/design-survey`: frecuencia de la duda, cómo eligen hoy, cuántas botellas, subgrupo (recibe gente / regaladas); opt-in a entrevista | Confirmar o descartar la oportunidad; decidir si Tomás queda dentro o en el borde | mediados de dic. 2026 |
| Creencia 2 (el porqué) | 3) `/design-interview` con quienes aceptaron en la encuesta, priorizando a quienes contradigan la creencia | Entender la última vez que eligieron mal y qué hicieron; entrada para `/explore-solutions` | mediados de ene. 2027 |
| Creencia 3 (retención 40% a 3 meses) | 1) `/research-market`: benchmark de retención de apps de bodega o maridaje | Ajustar el umbral del 40% antes de medir | mediados de nov. 2026 |
| Creencia 3 (retención 40% a 3 meses) | 2) Prueba de solución (concierge / Wizard of Oz) vía `/design-solution-tests` | Decidir si se construye; la retención solo se mide con uso real | entre feb. y abr. 2027 |

## Ideas candidatas (sin evaluar)

- Registro detallado del stock con la información relevante de cada vino.
- Autocompletar los datos del vino desde internet a partir de su nombre.
- Preguntar por el plato u ocasión y recibir una recomendación limitada al propio stock.
- Consultar rápidamente cuántas unidades se tienen de una botella.
