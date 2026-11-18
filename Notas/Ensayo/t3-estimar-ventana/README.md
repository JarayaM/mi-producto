# T3 estimar ventana: resultados sintéticos (ensayo)

> **Procedencia: `synthetic`.** Generado por Claude el 2026-11-18, para practicar el análisis. **No es evidencia.** No se cita en `product/insights/`, `product/overview.md` ni en la sección Resultados de `product/tests/2026-11-12-1239-perder-botellas-sin-abrir-a-tiempo.md`.

Simula T3 completa con el material de `product/tests/materials/t3-estimar-ventana/`: el armado y congelamiento del set de 30 botellas, la estimación con IA botella por botella, la clave del sommelier y la comparación. El análisis y la decisión quedan para `/analyze-solution-tests`.

## Archivos

| Archivo | Qué simula |
|---|---|
| `set-de-botellas.csv` | La hoja del material, llena: las 30 botellas, de dónde salió cada una y si cuenta para el subconjunto chileno chico |
| `respuestas-ia.md` | La respuesta textual de la IA a cada botella, con búsquedas, tokens, costo y minutos de cada corrida |
| `hoja-sommelier.csv` | La hoja del material, llena por el sommelier: año, confianza, si conoce el vino y comentario |
| `hoja-comparacion.csv` | La hoja de registro del material, llena: las dos estimaciones, la diferencia, si cae dentro de ±1 año y la fila RESUMEN |
| `bitacora.md` | Los 14 días: quién mandó fotos, qué entró al set, qué se reemplazó, cómo se corrió la IA y el ida y vuelta con el sommelier |

## Supuestos de la simulación

- **Calendario.** El día 1 es el lunes 2026-11-23 y el día 14, el domingo 2026-12-06. T3 corre en paralelo con el inicio de T1, con el mismo sommelier, y eso se nota en los plazos.
- **De dónde salen las botellas.** 14 vienen de los 6 entrevistados que compran, 13 de 7 encuestados con R2 = Sí (se contactó a 10) y 3 de la carta del restaurante. Los entrevistados y los encuestados son los del ensayo; lo que escriben en la bitácora es inventado. Ninguno coincide con los participantes de los ensayos de T1 y T2, que son ficticios.
- **Vinos.** Las etiquetas son reales. Las de productores chilenos chicos se verificaron en la web el 2026-11-18. Las fechas de la IA y del sommelier son simuladas y **no sirven como referencia de guarda real**.
- **El sommelier** es el del ensayo de T1, con criterios coherentes: unos 2 a 3 años para blancos de entrada, unos 5 para reservas, de 7 a 10 para gran reserva y de 15 a 18 para íconos, descontando por la guarda sin climatizar.
- **La IA.** La corrió tech con Claude Sonnet 5.5 por API y búsqueda web, con la misma configuración para las 30 botellas. El costo se calculó con precios de lista de noviembre de 2026. Las fuentes se anotan como dominio y descripción, no como URLs completas.
- **Cómo se llenó la hoja.** Las reglas de `prompt-estimacion.md` y del README del material se siguen al pie de la letra. Cuando un caso no calza bien con la regla, se explica en `notas`. Ninguna fila corrige la regla.
- **La fila RESUMEN** trae los porcentajes que pide el paso 5 del material. No trae una decisión.

## Cómo se calibró

Se buscaron datos públicos para que el patrón de coincidencias fuera verosímil. Las cifras salen de resúmenes y fuentes secundarias encontradas en una búsqueda web el 2026-11-18; no se leyeron todos los papers completos. Sirven para el orden de magnitud y **no son evidencia sobre el producto**.

| Hallazgo | Cómo se usó en la simulación |
|---|---|
| **Las ventanas de guarda son estimaciones gruesas.** No apareció un estudio que compare ventanas de distintos críticos para el mismo vino. La prensa especializada las describe como poco exactas, y algunos críticos evitan dar ventanas a vinos jóvenes porque quedarían demasiado anchas (Decanter, Winemag). | El acuerdo depende del largo de la ventana. En vinos para tomar en 1 a 3 años, la IA y el sommelier casi siempre coinciden; en vinos de guarda de 10 años o más, rara vez quedan a ±1 año. |
| **El juicio experto en vino es ruidoso.** En la Feria Estatal de California, cerca del 10% de los jueces repitió su medalla con la misma muestra (Hodgson, 2008). Una revisión de 2012 encontró menos consenso entre jueces de vino que en otros campos de juicio experto. | La clave del sommelier es una estimación con ruido, no la verdad. Hay casos en que la IA parece tener mejor información que él. |
| **Las fichas técnicas chilenas prometen guarda larga "bien conservado".** En los VIGNO, la guarda declarada va de 10 años (Emiliana) a 10–20 (Torres) y 20–30 (De Martino). | En vinos de guarda, la IA tiende a anclarse en la ficha o en la crítica y a ajustar poco por la guarda sin climatizar. |
| **El calor acelera el envejecimiento.** Un Sangiovese guardado en una pieza de una casa (20–26 °C) envejeció unas cuatro veces más rápido que en bodega (estudio italiano citado por The Drinks Business, 2014). Purdue indica que la tasa de absorción de oxígeno se duplica con 3,8 °C más. | El sommelier descuenta más que la IA por la guarda sin climatizar. |
| **Los modelos fallan más con lo poco conocido.** Los modelos de lenguaje fallan la mayoría de las preguntas sobre entidades poco populares, y la búsqueda ayuda justamente ahí (Mallen y otros, 2023). En SommBench (2026), los mejores modelos llegan al 97% en teoría del vino, pero no pasan del 65% al completar atributos de un vino concreto. | La IA acierta más con marcas grandes y vinos simples. Los productores chicos que exportan (los naturales de Itata y Maule) tienen bastante presencia en sitios en inglés, así que la IA los encuentra más de lo esperado. |
| **Las citas de buscadores con IA no siempre respaldan lo que dicen.** Solo el 74,5% de las citas respaldaba la frase a la que acompañaba (Liu y otros, 2023). | Algunas fuentes son de otra cosecha o de otro vino del productor, y la columna `ia_encontro_el_vino` se llena de forma inconsistente. |
| **El pipeño se hace para tomar joven.** No apareció una ventana publicada para los Cinsault de Pedro Parra o Garage Wine Co. | En naturales de Itata y Maule, la IA tiende a tratarlos como pipeño y les da fechas tempranas. El sommelier, que conoce las viñas viejas, les da más años. |
| **Las apps de cava estiman ventanas, pero no publican su precisión.** InVintory, Cellared y otras usan críticos, datos de la comunidad y curvas por cepa. | No hay una referencia de mercado para "precisión útil". Los umbrales son los que fijó el fundador. |
| **Precios de lista de la API** (noviembre de 2026): Claude Sonnet 5.5 cuesta USD 2 por millón de tokens de entrada y USD 10 por millón de salida; la búsqueda web, USD 10 por 1.000 búsquedas. | Costo por botella = tokens × precio + búsquedas × USD 0,01. |

**Lo que no se encontró:** cuánto coinciden dos expertos en el año final de una ventana de guarda, y una temperatura interior típica en verano para casas de Santiago sin aire acondicionado.

## Casos borde incluidos a propósito

Aparecen en los datos para practicar el análisis. Lo que muestran se lee en los datos mismos:

- Una botella de clasificación dudosa para el subconjunto chileno chico, marcada `no` por la regla.
- Una botella de la carta que el sommelier sí había catado y que avisó con el set ya congelado.
- Una respuesta de la IA sin año que, en el fondo, dice lo mismo que el sommelier.
- Una respuesta de la IA con un rango, que se repitió.
- Una respuesta del sommelier con un rango, que se aclaró.
- Un año del sommelier que ya pasó.
- Fuentes de otra cosecha, y la columna `ia_encontro_el_vino` llenada distinto en casos parecidos.
- Un vino donde la IA cita a la crítica y el sommelier no lo conoce.
- Una botella que estuvo en una cava que falló. Su estado real queda fuera de la prueba.
- Una botella de un encuestado que no se pudo identificar y se reemplazó antes de congelar.
- Encuestados que no respondieron o respondieron tarde.
- La planilla del sommelier devuelta un día tarde.
- Una corrida de IA mucho más larga y cara que el resto.

## Fuentes

- Ventanas de guarda como estimaciones: [Decanter, Bordeaux drinking windows](https://www.decanter.com/learn/bordeaux-drinking-windows-ask-decanter-406425/), [Winemag, editorial](https://winemag.co.za/?p=102116), [ejemplo de ventana de Tim Atkin](https://timatkin.com/tasting-notes/tesco-finest-peumo-carmenere/)
- Hodgson (2008), consistencia de jueces: [Journal of Wine Economics](https://econpapers.repec.org/RePEc:cup:jwecon:v:3:y:2008:i:02:p:105-113_00)
- Revisión de 2012 sobre confiabilidad y consenso de jueces: [Journal of Wine Economics](https://resolve.cambridge.org/core/journals/journal-of-wine-economics/article/reliability-and-consensus-of-experienced-wine-judges-expertise-within-and-between/B7BAFAB594A095C6EEE1D01C4EEA958E)
- Guarda declarada en fichas VIGNO: [Torres](https://www.torres.es/en/wines/miguel-torres-chile/vigno-carignan), [Emiliana](https://www.emiliana.cl/cms/wp-content/uploads/2025/06/VIGNO-2021-ESP.pdf), [De Martino](https://demartino.cl/wp-content/uploads/2025/07/DM_OVS_VIO_2022_ESP.pdf)
- Calor y envejecimiento: [The Drinks Business (2014)](https://www.thedrinksbusiness.com/2014/08/badly-kept-wine-ages-four-times-faster/), [Purdue Extension](https://www.extension.purdue.edu/extmedia/fs/fs-58-w.pdf)
- Mallen y otros (2023), *When Not to Trust Language Models*: [arXiv](https://arxiv.org/pdf/2212.10511v2)
- SommBench (2026): [arXiv](https://arxiv.org/abs/2603.12117)
- Liu, Zhang y Liang (2023), *Evaluating Verifiability in Generative Search Engines*: [arXiv](https://arxiv.org/abs/2304.09848)
- Pipeño e Itata: [New Worlder](https://www.newworlder.com/getting-to-know-pipeno/), [Wine Anorak](https://wineanorak.com/2024/03/03/dry-grown-chile-exploring-itata-a-historic-region-whose-time-has-now-come/)
- Apps que estiman ventanas: [InVintory](https://invintory.com/blog/drink-window-automation-how-apps-build-and-maintain-your-open-tonight-queue/)
- Verificación de etiquetas chilenas chicas: [González Bastías, Matorral](https://www.wine.com/product/vina-gonzalez-bastias-matorral-2020/4121436), [A Los Viñateros Bravos, Granítico](https://decanter.com/wine-reviews/chile/itata-valley/a-los-vinateros-bravos-granitico-cinsault-2021-86766), [Rogue Vine, Grand Itata Blanco](https://www.indigowine.com/wine/grand-itata-blanco/), [Laberinto, Cenizas](https://southamericawineguide.com/tasting-note/cenizas-de-laberinto-sauvignon-blanc/)
- Precios de la API: referencia de la API de Claude, precios de lista de noviembre de 2026.
