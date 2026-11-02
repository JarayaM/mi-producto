---
status: framed
priority: 3
segment: Aficionados que buscan qué vino combina con una comida y no logran llevar la sugerencia a una botella propia, sobre todo quienes saben poco de vino
personas: carolina-mendez, tomas-rivas, lucas-fernandez, elena-valdivia
---

# Oportunidad: No pueden llevar la sugerencia de maridaje a una botella propia

Encontrar un maridaje suele ser fácil, pero la respuesta rara vez termina en una botella que tengan: adivinan, abren otra cosa o salen a comprar. Es el problema más amplio y recurrente de los tres, aunque el dolor es desigual.

**Prioridad 3 de 3**, decidida por el fundador el 2026-11-02. Las otras son [perder-botellas-sin-abrir-a-tiempo](2026-11-02-1825-perder-botellas-sin-abrir-a-tiempo.md) y [stock-incierto-en-la-cava](2026-11-02-1825-stock-incierto-en-la-cava.md).

Se superpone con [elegir-vino-de-mi-stock](2026-10-19-1642-elegir-vino-de-mi-stock.md), en pausa desde el 2026-11-02.

## Segmento y personas

- Carolina Méndez (secondary) — lo sufre: Google le recomienda vinos que no tiene y termina eligiendo el que está más a mano.
- Tomás Rivas (secondary, en el borde) — lo sufre: ChatGPT le responde "un tinto con cuerpo" y no sabe cuál de sus botellas abrir.
- Lucas Fernández (tertiary) — no lo sufre; opina sobre el gasto del hogar → informa la viabilidad.
- Elena Valdivia (negative) — no lo sufre; ella o su sommelier deciden qué abrir. Fuera de alcance.
- Faltante: ninguna.

## Señales

| Señal | Provenance | Fuente |
|---|---|---|
| Buscaron maridaje 30/44 en los últimos 3 meses, 12 de ellos varias veces | survey | product/insights/2026-11-02-1805-eleccion-y-registro-de-vino.md |
| 25/30 terminaron adivinando o con algo que no tenían, y 2/30 abrieron una botella propia sugerida | survey | product/insights/2026-11-02-1805-eleccion-y-registro-de-vino.md |
| Se repite en los 5 canales: 11/15 en comunidades externas y 14/15 en la red del fundador, entre quienes buscaron | survey | Notas/Ensayo/respuestas_encuesta_50_reclutamiento.csv |
| Abrieron una botella y notaron que otra combinaba mejor: 15/45 | survey | Notas/Ensayo/respuestas_encuesta_50_reclutamiento.csv |
| Los 10 que dudan ≥2 veces al mes buscaron con ChatGPT y ninguno terminó en una botella propia; 9 de los 10 vienen de la red del fundador | survey | Notas/Ensayo/respuestas_encuesta_50_reclutamiento.csv |
| De los 17 que adivinaron, a 8 les molesta elegir y a 8 les gusta | survey | product/insights/2026-11-02-1805-eleccion-y-registro-de-vino.md |
| De 6 que buscaron, 3 traducen la respuesta sin esfuerzo (Felipe, Marcela, Verónica) y 3 no pueden (Lucía, Andrés, Daniel). Otros 4 no buscan | real | product/insights/2026-11-02-1809-entrevistas-eleccion-y-registro.md |
| Felipe ya resuelve su stock con una foto a ChatGPT, aunque le falla una de cada tres veces | real | Notas/Ensayo/entrevistas/2026-10-28-felipe-arancibia.md |
| Ninguno de los 9 que dudan seguido y respondieron sobre pagos paga una app | survey | product/insights/2026-11-02-1805-eleccion-y-registro-de-vino.md |
| Recomendar desde el stock propio ya no diferencia: InVintory, CellarTracker y varias startups lo ofrecen, casi todas en inglés y para colecciones grandes | secondary | product/research/2026-10-19-1711-mercado-cava-recomendacion-stock.md |

## Resultado de negocio

Comercial. Principal: **retención**: es el único de los tres problemas que aparece en cada comida, así que es el que mejor podría sostener un uso recurrente. Secundario: **conversión a pago**, con el riesgo de que quienes más lo sufren hoy no pagan por una app.

## Restricciones

- Horizonte: ~6 meses (hasta abril de 2027), sin fecha límite externa.
- Presupuesto: ≈ CLP 10.000.000 en 6 meses (estimación del fundador, sin desglose).
- Construcción: low code deseable, no obligatorio; el fundador construye sin equipo de desarrollo dedicado.
- Costo variable: el consumo de recursos por recomendación debe caber dentro del ingreso esperado por usuario.

## Creencias

Referencias a product/overview.md — el registro único de creencias.

- [opportunity: sugerencia-maridaje-sin-botella-propia] [value] (creencia 10) Quienes buscan maridaje al menos una vez al mes pierden tiempo o abren una botella peor por no poder llevar la sugerencia a su stock, y les importa lo bastante como para dejar de hacerlo a mano.
- [product] [value] (creencia 4 del overview, reutilizada) La recomendación limitada al propio stock vale más que una genérica.
- [opportunity: elegir-vino-de-mi-stock] [viability] (creencia 3 del overview, reutilizada) Al menos el 25% de los usuarios activados sigue pidiendo recomendaciones al menos 2 veces al mes después de 3 meses.

## Agenda de investigación

El fundador cerró la investigación de mercado, las encuestas y las entrevistas el 2026-11-02. Lo no resuelto pasa como riesgo a `/explore-solutions` y a las pruebas de solución. Las fechas son una propuesta.

| Creencia | Instrumento | Decisión que desbloquea | Para cuándo |
|---|---|---|---|
| Creencias 4 y 10 | Prueba de solución frente a usar ChatGPT con una foto o una lista, vía `/design-solution-tests`, registrando cada búsqueda y cómo termina | Saber si superan a lo que ya existe gratis, y la frecuencia real | entre feb. y abr. 2027 |
| Creencia 3 | La misma prueba, midiendo pedidos al mes | Decidir si se construye | entre feb. y abr. 2027 |

## Ideas candidatas (sin evaluar)

- Preguntar por el plato u ocasión y recibir una recomendación limitada al propio stock.
- Traducir una sugerencia genérica a las botellas que se tienen.
- Foto de la cava o de etiquetas para recomendar sin registro previo.
