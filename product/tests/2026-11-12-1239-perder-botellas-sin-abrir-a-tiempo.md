---
opportunity: perder-botellas-sin-abrir-a-tiempo
solutions: product/solutions/2026-11-02-1857-perder-botellas-sin-abrir-a-tiempo.md
status: ready
---

# Pruebas de solución para: Pierden botellas por no abrirlas a tiempo

## Por qué probar

Están en prueba A4 (`revision-de-cava`) y A2 (`recordatorio-por-lote`). La evidencia muestra el dolor (7/24 en el segmento, 4/5 en 51–100), pero nadie ha reaccionado todavía a ninguna de las dos soluciones: ambas tienen `pain evidenced, relief not tested`. Además, A4 depende de poder estimar hasta cuándo aguanta cada botella (creencia 11), algo que no se ha probado.

**Orden:** T3 primero (semanas 1–2), porque es la más barata y puede tumbar A4. T1 (semanas 2–16) y T2 (semanas 2–12) corren en paralelo, con grupos distintos.

**Reclutamiento común a T1 y T2:** personas que compran vino, con 51–100 botellas (se aceptan 21–50 si no alcanza) y que no trabajan en la industria. Como máximo 2 de cada 8 pueden venir de CAV, porque ahí la señal está sobrerrepresentada. Primero se recluta entre quienes respondieron la encuesta y aceptaron ser contactados (`Notas/Ensayo/respuestas_encuesta_50_reclutamiento.csv`), sin repetir a los entrevistados. Nadie participa en T1 y en T2 a la vez.

## T1. revision-de-cava: revisión hecha a mano

- **Estado de la prueba:** ready
- **Creencia en prueba:** "Al menos la mitad de quienes hicieron una revisión pide la segunda y abre al menos una de las botellas señaladas antes de esa segunda revisión." *(creencia 12, `product/overview.md`)*
- **Riesgo:** [value]
- **Tipo de prueba:** concierge
- **Qué hacemos:**
  1. La persona manda fotos de su cava o una lista, en el formato que prefiera.
  2. En 5 días hábiles recibe, por WhatsApp o correo, una lista corta: "conviene abrir en los próximos 3 meses", con el motivo de cada botella en una línea. Esa lista la arman a mano el fundador y el sommelier de restaurante (el mismo de T3).
  3. En la semana 2 se hace un único contacto para resolver dudas. No se mandan recordatorios de las botellas: eso sería probar A2.
  4. En la semana 12 se envía un solo mensaje: "Se cumplen 3 meses. Si quieres tu segunda revisión, mándanos tu foto o lista". No se insiste.
  5. A los 14 días de ese mensaje se pregunta qué botellas de la primera lista abrió y cuándo.
- **Con quién:** 8 personas del segmento, reclutadas como se indica arriba.
- **Material necesario:** el mensaje de reclutamiento, las instrucciones para mandar la foto o la lista, la plantilla de la lista entregada, el mensaje de la semana 12, el guion del contacto final y una hoja de registro por persona: cantidad de botellas recibidas, **cuántas botellas trae su lista**, cuáles abrió y cuándo, y si mandó material para la segunda revisión y en cuántos días. Quedan fuera deliberadamente una app, una planilla compartida y cualquier aviso automático.
- **Material:** [product/tests/materials/t1-revision-de-cava/](materials/t1-revision-de-cava/README.md)
- **Duración:** unas 14 semanas por persona (3 meses hasta la segunda revisión, más 14 días para responder).
- **Señal y umbral:** se miden dos cosas por persona: (a) si abrió al menos una botella señalada antes de la segunda revisión, y (b) si pidió la segunda revisión, es decir, si mandó su foto o lista dentro de los 14 días del mensaje. Decir "me interesa" no cuenta. Pasa si al menos 4 de 8 cumplen (a) y (b).
- **Regla de decisión:**
  - **continue** si al menos 4/8 cumplen (a) y (b).
  - **change** si al menos 4/8 cumplen (a) pero menos de 4/8 cumplen (b): la lista sirve pero no hay repetición, así que hay que revisar el formato. Si además al menos 5 de 8 listas traían 0 o 1 botella, el problema es la frecuencia, y se prueba una versión cada 6 meses o con la frecuencia que elija cada persona.
  - **discard** si 1/8 o menos cumple (a).
  - **inconclusive** si menos de 6 personas completan la prueba.
- **Procedencia esperada:** real
- **Siguiente paso si pasa:** hacer la segunda revisión y ofrecer la tercera con precio, como prueba de la creencia 13 (viabilidad).

## T2. recordatorio-por-lote: aviso agendado

- **Estado de la prueba:** ready
- **Creencia en prueba:** "En al menos la mitad de los avisos, la persona abre la botella o toma una decisión explícita sobre ella dentro de 30 días." *(creencia 14, `product/overview.md`)*
- **Riesgo:** [value]
- **Tipo de prueba:** concierge
- **Qué hacemos:**
  1. En una llamada de 15 minutos, la persona elige 2 o 3 botellas o lotes que ya tiene y quiere tomar "en algún momento".
  2. Ella misma elige y agenda un aviso en su propio calendario, para una fecha entre 2 y 6 semanas más adelante. Nosotros solo la acompañamos y no le estimamos la fecha.
  3. A los 30 días de cada aviso le preguntamos qué hizo con esa botella: la abrió, decidió cuándo abrirla (con fecha o una ocasión concreta), la regaló o vendió, pospuso el aviso o lo ignoró.
- **Con quién:** 8 personas del segmento, distintas a las de T1. Se esperan entre 16 y 24 avisos.
- **Material necesario:** el mensaje de reclutamiento, el guion de la llamada, el texto sugerido para el evento de calendario ("Abrir o decidir: {vino}") y una hoja de registro por aviso (botella, fecha del aviso, qué hizo, en cuántos días). Queda fuera deliberadamente la estimación de fechas, porque eso es A4.
- **Material:** [product/tests/materials/t2-recordatorio-por-lote/](materials/t2-recordatorio-por-lote/README.md)
- **Duración:** 10 semanas (hasta 6 semanas para que suene el aviso y 30 días después).
- **Señal y umbral:** el porcentaje de avisos que terminan en "abrió" o "tomó una decisión explícita" dentro de los 30 días. "Lo posponemos" o "no hice nada" no cuentan. Pasa si es al menos el 50%.
- **Regla de decisión:**
  - **continue** si al menos el 50% de los avisos termina en apertura o decisión. En ese caso basta con la atención, y A4 tiene que mostrar que aporta algo más que eso: el criterio de qué abrir.
  - **change** si queda entre 25% y 49%: el aviso solo no alcanza. Se prueba una versión que combine el aviso con una lista visible (A3) o con el motivo de por qué abrirla.
  - **discard** si es menos del 25%.
  - **inconclusive** si se registran menos de 12 avisos.
- **Procedencia esperada:** real
- **Siguiente paso si pasa:** repetir con fechas reales de guarda (meses) y más personas, y verificar si alguien pagaría por que se lo hagan, que es la viabilidad de A2.

## T3. revision-de-cava: estimar hasta cuándo aguanta cada botella

- **Estado de la prueba:** ready
- **Creencia en prueba:** "Se puede estimar con precisión útil hasta cuándo aguanta cada botella del segmento, incluidos vinos chilenos de productores chicos, sin saber cómo se guardó." *(creencia 11, `product/overview.md`)*
- **Riesgo:** [feasibility]
- **Tipo de prueba:** technical-test
- **Qué hacemos:**
  1. Se arma un set de 30 botellas reales de cavas del segmento, identificadas con productor, cepa y cosecha, con al menos 10 de productores chilenos chicos. Como las entrevistas y la encuesta no identifican botellas, las fotos de etiquetas se piden a entrevistados y encuestados que aceptaron contacto. Como último recurso se usan hasta 8 vinos de la carta del restaurante que el sommelier no haya seleccionado ni catado.
  2. Para cada una se estima la fecha límite ("abrir antes de", el año) usando IA y fuentes públicas, sin ver la clave de respuestas. Se registran el tiempo y el costo por botella.
  3. Un sommelier de restaurante da su estimación por separado, sin ver la de la IA. Esa es la clave de respuestas.
  4. Se comparan las dos estimaciones.
- **Con quién:** las 30 botellas y un sommelier de restaurante. Responsable: tech o el fundador.
- **Material necesario:** el set de 30 botellas (nombre, cosecha, productor), el prompt o procedimiento de estimación, la clave del experto y una hoja de comparación por botella. Queda fuera deliberadamente la lectura de fotos, que se prueba aparte si T3 pasa.
- **Material:** [product/tests/materials/t3-estimar-ventana/](materials/t3-estimar-ventana/README.md)
- **Duración:** 2 semanas.
- **Señal y umbral:** el porcentaje de botellas cuya estimación cae dentro de ±1 año de la del experto, en total y en el subconjunto chileno chico. Pasa si es al menos el 75% en total y al menos el 60% en el subconjunto chileno.
- **Regla de decisión** (para A4):
  - **continue** si pasa.
  - **change** si el total queda entre 60% y 74%, o si el total pasa pero el subconjunto chileno queda bajo 60%: la fecha la valida un experto o la confirma la persona (al menos en los vinos chilenos chicos), y A4 pasa a ser una revisión asistida.
  - **discard** de la estimación automática si el total queda bajo 60%. A4 solo seguiría si la fecha la pone la persona, como ya anticipa la sección de decisión del archivo de soluciones.
- **Procedencia esperada:** real (botellas reales del segmento y un experto real)
- **Siguiente paso si pasa:** probar la lectura de fotos de cava con el set de T1 y medir el costo en tokens por revisión.

## Resultados

*(Lo agrega `/analyze-solution-tests`.)*

## Decisión

*(Lo agrega `/analyze-solution-tests`.)*
