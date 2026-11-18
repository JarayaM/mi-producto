# T2 recordatorio por lote: resultados sintéticos (ensayo)

> **Procedencia: `synthetic`.** Generado por Claude el 2026-11-18, para practicar el análisis. **No es evidencia.** No se cita en `product/insights/`, `product/overview.md` ni en la sección Resultados de `product/tests/2026-11-12-1239-perder-botellas-sin-abrir-a-tiempo.md`.

Simula T2 completa con el material de `product/tests/materials/t2-recordatorio-por-lote/`: las 8 llamadas, los avisos que agenda cada persona, lo que escriben entre medio y sus respuestas al seguimiento de cada aviso.

## Archivos

| Archivo | Qué simula |
|---|---|
| `llamadas.md` | Las notas del fundador en cada llamada de 15 minutos: qué botellas eligió la persona, por qué las guarda y qué fecha puso |
| `conversaciones.md` | Lo que escribe cada participante: la confirmación, los mensajes espontáneos y las respuestas al seguimiento, la repregunta y el recordatorio |
| `hoja-registro.csv` | La hoja del material, llena: una fila por aviso |

## Supuestos de la simulación

- **8 participantes y 22 avisos agendados,** dentro de los 16 a 24 que espera el diseño. Uno queda fuera de rango, así que entran 21 en la prueba.
- **Calendario.** Las llamadas son del 2026-11-30 al 2026-12-07 (semana 2, en paralelo con T1). Los avisos suenan entre el 15 de diciembre y el 17 de enero, y los seguimientos van del 14 de enero al 19 de febrero de 2027. Los avisos caen en Navidad, Año Nuevo y las vacaciones de verano en Chile, y eso se nota en qué se abre y en quién responde.
- **Reclutamiento.** Se alterna con T1 por orden de aceptación, y nadie está en las dos pruebas. 5 de las 8 personas tienen 51–100 botellas y 3 tienen 21–50 (plan B del filtro). Hay 2 de CAV, el máximo que permite el diseño. Una candidata quedó como `sin botellas` en la llamada y se reemplazó.
- **Personas.** Son ficticias. No corresponden a encuestados, a entrevistados ni a participantes del ensayo de T1.
- **Vinos.** Las etiquetas son reales y comunes en Chile. T2 no estima fechas, así que el único juicio sobre el estado de un vino es lo que cuenta la persona al abrirlo.
- **Cómo se llenó la hoja.** Cuando un caso es ambiguo, `resultado` y `cuenta` siguen al pie de la letra la tabla "Qué cuenta y qué no" del README del material, y el caso se explica en `notas`. Ninguna fila corrige la regla.
- **Resultado final.** Si la persona movió el aviso y después abrió la botella dentro de los 30 días, se registra `abrió`. Los días se cuentan desde la fecha original del aviso.
- **`sin respuesta`** entra en el denominador con `cuenta = no`, como pide el material.

## Cómo se calibró

Se buscaron datos públicos para que las proporciones fueran verosímiles. Las cifras salen de resúmenes y fuentes secundarias encontradas en una búsqueda web el 2026-11-18; no se leyeron los papers completos. Sirven para el orden de magnitud y **no son evidencia sobre el producto**.

| Hallazgo | Cómo se usó en la simulación |
|---|---|
| **Brecha entre intención y conducta:** cerca de la mitad de quienes tienen la intención de hacer algo no lo hace (Sheeran 2002; Rhodes y de Bruijn 2013). | Sin el aviso, la base de "abrir la botella que pensaba abrir" ronda el 50%. |
| **Planes de cuándo y dónde** ("implementation intentions"): el meta-análisis de 2006 dio d = 0,65, pero la actualización de 2024, corregida por sesgo de publicación, lo baja a entre 0,15 y 0,35. | El aviso agendado suma poco sobre esa base. |
| **Se posterga lo que se disfruta:** con un vale de plazo largo se canjea menos que con uno de plazo corto, aunque al recibirlo la gente cree que el de plazo largo es mejor (Shu y Gneezy 2010). | Las botellas que se guardan "para disfrutar" tienden a posponerse. |
| **La ocasión ideal:** se sube tanto la vara de la ocasión que la botella especial no se abre, y se lamenta más abrirla demasiado pronto que no abrirla nunca (Sharif y Shu; Open That Bottle Night). | Las botellas especiales terminan en "pospuso" o en decisiones lejanas. Los lotes "para tener" se abren más. |
| **Estacionalidad en Chile:** diciembre pesa entre 9% y 12% de la facturación anual de vino y espumante, más del 60% del espumante se vende en el segundo semestre, y en verano se toma más blanco. | Los avisos de fin de año se abren mucho, los espumantes van a Año Nuevo y los blancos a enero. |
| **Respuesta a seguimientos por mensaje:** en estudios largos con SMS, entre 69% y 77% sigue respondiendo. | Aquí es un solo mensaje corto por aviso, con personas cercanas, así que responde más: 17 de 21 al primer mensaje, 3 más con el recordatorio y 1 nunca. |

**Lo que no se encontró:** tasas de cumplimiento de recordatorios que la propia persona agenda para algo placentero. El análisis de recordatorios de Cortana (Graus y otros, 2016) describe cuándo y para qué se crean, pero no si se cumplen.

## Casos borde incluidos a propósito

Aparecen en los datos para practicar el análisis. Lo que muestran se lee en los datos mismos:

- Una candidata `sin botellas` que se reemplaza.
- Un aviso fuera del rango de 2 a 6 semanas.
- Avisos puestos en fechas en que la persona ya pensaba abrir la botella.
- Una botella abierta antes de que sonara el aviso.
- Una botella abierta después de los 30 días.
- Un aviso que se movió y después terminó en apertura.
- Un aviso que se movió y no terminó en nada.
- Una decisión explícita de guardar la botella muchos años más.
- Un "la voy a abrir pronto" que con la repregunta se vuelve fecha, y otro que no.
- Un aviso en el calendario del trabajo, uno que sonó en vacaciones y uno que se perdió con el teléfono.
- Una persona que pide que le digan si su botella está lista.
- Un lote donde la cantidad anotada no era la real.
- Botellas que se abrieron y estaban pasadas.
- Una botella regalada.
- Una persona que deja de responder.

## Fuentes

- Sheeran y Webb (2016), *The intention–behavior gap*: [PDF](https://content.workplacegivingaustralia.org.au/app/uploads/2020/10/Intention-Behaviour-Gap-Full-Article-SheeranWebb2016.pdf)
- Frontiers in Psychology (2022), que cita a Sheeran (2002) y a Rhodes y de Bruijn (2013): [artículo](https://www.frontiersin.org/journals/psychology/articles/10.3389/fpsyg.2022.923464/full)
- Implementation intentions, cifras de 2006 y 2024 (fuentes secundarias): [The Behavioral Scientist](https://www.thebehavioralscientist.com/glossary/implementation-intentions), [ID Tips](https://idtips.substack.com/p/implementation-intentions-the-science)
- Shu y Gneezy (2010), *Procrastination of Enjoyable Experiences*: [University of California](https://universityofcalifornia.edu/news/dont-wait-have-fun-science-says)
- Sharif y Shu, la ocasión ideal y Open That Bottle Night: [Grape Collective](https://grapecollective.com/articles/open-that-bottle-night-academics-agree-that-selfcontrol-may-be-overapplied)
- Estacionalidad del vino y el espumante en Chile: [El Mostrador (2020)](https://www.elmostrador.cl/generacion-m/2020/12/19/mas-del-60-de-la-comercializacion-de-espumantes-se-centra-en-el-segundo-semestre-por-las-fiestas-de-fin-de-ano/)
- Seguimiento por SMS: [retención a 12 meses (PMC3757960)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3757960/), [diario por SMS (PMC1550628)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1550628/)
- Graus, Bennett, White y Horvitz (2016), *Analyzing and Predicting Task Reminders*: [PDF](https://www.erichorvitz.com/Cortana-reminders_UM_2016.pdf)
