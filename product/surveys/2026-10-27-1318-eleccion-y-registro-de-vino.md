# Encuesta: cómo eligen, maridan y registran su vino los aficionados

- **Objetivos de aprendizaje:**
  - **G1.** Con qué frecuencia aparece la duda de qué botella propia abrir y cómo se resuelve hoy (creencia 2). Decide si la oportunidad sigue o se descarta, y si el subgrupo "botellas regaladas" (Tomás) queda dentro del segmento o en el borde.
  - **G2.** Cuántas botellas abren al mes (creencia 3). Decide si la retención se mide con "≥2 veces al mes" o con "≥1", y permite segmentar por tamaño de cava.
  - **G3.** Cómo registran hoy su stock y, entre quienes lo abandonaron, si fue por el alta o por la baja (creencia 1). Decide si la propuesta de valor se centra en el alta escribiendo solo el nombre o en la baja sin esfuerzo.
  - **G4.** Cuánto gastan hoy en apps o servicios de vino, en CLP (creencia 5). Decide si USD 2–4 al mes calza con lo que el segmento ya paga.
  - **G5.** Cómo buscan maridaje hoy y si la respuesta termina en una botella propia (creencia 4; señal `unverified` del brief). Decide si recomendar desde el stock propio resuelve un vacío real o si las herramientas actuales bastan.
- **Respondentes:** aficionados con 10 o más botellas en casa que abrieron al menos una en los últimos 3 meses (segmento de [product/opportunities/2026-10-19-1642-elegir-vino-de-mi-stock.md]). Dos subgrupos según S3: quienes compran sus botellas (Carolina) y quienes las reciben de regalo (Tomás).
- **Largo estimado:** 3 filtros + 14 preguntas (4 condicionales) + edad + bloque de reclutamiento, ~6 min.
- **Límite:** no hubo entrevistas previas; las opciones salen de supuestos y de foros de coleccionistas grandes. Toda pregunta de opción lleva escape y hay preguntas abiertas. La encuesta cuenta; el *por qué* queda para `/design-interview`.

## Filtros

S1. ¿Cuántas botellas de vino tienes hoy en tu casa? [opción única] → queda fuera si "Menos de 10"
   - Menos de 10
   - 10–20
   - 21–50
   - 51–100
   - Más de 100
   > Goal: segmento; tamaño de cava para G2 y para detectar perfiles tipo Elena (negative)

S2. En los últimos 3 meses, ¿abriste en casa alguna de tus botellas para una comida, una visita o una ocasión? [opción única] → queda fuera si "No"
   - Sí
   - No
   > Goal: segmento (sin descorche no hay duda de qué abrir)

S3. La mayoría de tus botellas… [opción única]
   - Las compré yo
   - Me las regalaron
   - Más o menos mitad y mitad
   - Otro: ___
   > Goal: separar subgrupos (compra / regaladas) para G1

## Preguntas

Q1. En el último mes, ¿cuántas botellas de las que tenías en casa abriste? [opción única]
   - 0
   - 1
   - 2–3
   - 4–6
   - 7 o más
   > Goal: G2

Q2. Piensa en la última vez que abriste una de tus botellas para una comida u ocasión. ¿Cómo elegiste cuál abrir? [opción múltiple]
   - Abrí la que estaba más a mano
   - Ya tenía pensada una botella para esa ocasión
   - Revisé las botellas una por una
   - Busqué maridaje en Google o ChatGPT
   - Usé una app de vino (Vivino u otra)
   - Le pregunté a alguien
   - La eligió otra persona
   - Otro: ___
   > Goal: G1 (cómo se resuelve hoy)

Q3. En el último mes, ¿cuántas veces te costó decidir cuál de tus botellas abrir? [opción única]
   - Ninguna
   - 1 vez
   - 2–3 veces
   - 4 o más
   - No recuerdo
   > Goal: G1 (frecuencia; creencia 2 dice "un par de veces al mes")

Q4. En los últimos 3 meses, ¿te pasó alguna de estas situaciones? [opción múltiple]
   - Abrí una botella y después me di cuenta de que otra combinaba mejor
   - Abrí una botella que quería guardar para otra ocasión
   - Una botella pasó su mejor momento sin que la abriera
   - Compré una botella que ya tenía
   - Creí tener una botella que ya no estaba
   - Ninguna de estas
   > Goal: G1 (costo concreto de elegir mal)

Q5. Elegir qué vino de tu casa abrir es para ti… [likert-5, no obligatoria]
   - Muy molesto
   - Algo molesto
   - Ni molesto ni placentero
   - Algo placentero
   - Muy placentero
   > Goal: G1 (contraevidencia del research: elegir como parte del placer)

Q6. En los últimos 3 meses, ¿buscaste qué vino combina con un plato o una comida? [opción única]
   - Sí, varias veces
   - Sí, una vez
   - No
   > Goal: G5 (frecuencia de búsqueda de maridaje)

Q7. (Solo si respondió "Sí" en Q6) ¿Dónde lo buscaste? [opción múltiple]
   - Google
   - ChatGPT u otra IA
   - App de vino (Vivino u otra)
   - Vendedor o vinoteca
   - Amigo o familiar
   - Etiqueta o contraetiqueta
   - Otro: ___
   > Goal: G5 (fuentes actuales; alternativas con las que compite el producto)

Q8. (Solo si respondió "Sí" en Q6) Piensa en la última vez que buscaste. ¿Qué pasó después? [opción única]
   - Me sugirió un vino que tenía en casa, y lo abrí
   - Me sugirió un tipo de vino general ("un tinto con cuerpo") y tuve que adivinar cuál de los míos calzaba
   - Me sugirió algo que no tenía, y salí a comprar
   - Me sugirió algo que no tenía, y abrí otra cosa
   - No me sirvió
   - Otro: ___
   > Goal: G5 (clave: si domina "adivinar" o "no tenía", el vacío existe; si domina la primera opción, la creencia 4 se debilita)

Q9. Hoy, ¿cómo sabes qué botellas tienes? [opción única]
   - No llevo registro: lo veo en el mueble o de memoria
   - Planilla o notas (Excel, Google Sheets, notas del celular)
   - App de vino (Vivino, CellarTracker, InVintory u otra)
   - Otro: ___
   > Goal: G3

Q10. ¿Alguna vez llevaste un registro de tus botellas y lo dejaste? [opción única]
   - Sí, lo dejé
   - No, lo sigo llevando
   - Nunca llevé uno
   > Goal: G3

Q11. (Solo si respondió "Sí, lo dejé" en Q10) ¿Qué pasó? [opción múltiple]
   - Cargar cada botella nueva tomaba mucho tiempo
   - Me olvidaba de anotar las botellas que abría o regalaba, y el registro dejó de coincidir
   - Otras personas de la casa sacaban botellas sin anotarlas
   - No me servía para nada concreto
   - Cambié de celular o de app
   - Otro: ___
   > Goal: G3 (alta vs. baja; creencia 1)

Q12. En los últimos 12 meses, ¿pagaste por alguno de estos? [opción múltiple]
   - Versión premium de una app de vino (Vivino Premium u otra)
   - Club de vinos o suscripción de cajas
   - Cursos o catas
   - Ninguno
   - Otro: ___
   > Goal: G4 (gasto real, no intención)

Q13. (Solo si marcó "Versión premium de una app de vino" en Q12) ¿Cuánto pagas al mes por esa app? Si pagas al año, divide por 12. [opción única]
   - Menos de $2.000
   - $2.000–4.000
   - $4.001–8.000
   - Más de $8.000
   - No sé
   > Goal: G4 (USD 2–4 ≈ CLP 1.900–3.800)

Q14. ¿Qué es lo más difícil para ti a la hora de elegir qué vino de tu casa abrir? [abierta, opcional]
   > Goal: G1 y G5 (lenguaje real para las entrevistas)

D1. Edad [opción única]
   - 18–24
   - 25–34
   - 35–44
   - 45–54
   - 55–64
   - 65 o más
   > Goal: perfil de subgrupos (Tomás: 25–34)

## Screening + opt-in (reclutamiento para entrevistas)

R1. ¿Trabajas o trabajaste en la industria del vino (viña, distribución, vinoteca, sommelier)? [Sí / No] → no es candidato si "Sí". También quedan fuera quienes marcaron "Más de 100" en S1.
R2. ¿Aceptarías una conversación de 30 minutos sobre este tema? [Sí / No]
R3. Si respondiste que sí, ¿cómo te contactamos? [abierta, opcional]

## Distribution

| Canal | A quién llega y su sesgo | Alcance aprox. | Link |
|---|---|---|---|
| Comunidad del Club de Amantes del Vino (CAV) | Aficionados que compran seguido (Carolina). Sobrerrepresenta a socios comprometidos y con más conocimiento (cercanos a Elena) y a quienes ya pagan por vino, lo que infla G4 | unknown | link-cav |
| Grupos de Facebook de vino | Público amplio y mixto. Sobrerrepresenta a mayores y muy activos en la red; llega poco a jóvenes con Android (Tomás) | unknown | link-fb |
| Grupos de WhatsApp de colegas | Perfiles como Tomás: jóvenes, de tecnología, botellas regaladas. Canal propio: gente parecida al fundador; algunos responden por cariño | unknown | link-wsp |
| LinkedIn (publicación del fundador) | Profesionales de su red y de segundo grado. Sobrerrepresenta a profesionales urbanos de ingresos medios y altos | unknown | link-li |
| Instagram (publicación o historia del fundador) | Seguidores del fundador, perfil personal y mixto. Canal propio; las historias duran 24 h | unknown | link-ig |

- **Target n:** ≥30 respuestas válidas (pasan S1 y S2) por subgrupo: quienes compran sus botellas y quienes las reciben de regalo (S3). Con menos, los resultados son direccionales.
- **Alcance:** desconocido en todos los canales. Como mucha gente queda fuera en S1, probablemente se necesiten 150–300 respuestas en total para llegar a la meta; la primera revisión dirá si algún canal necesita refuerzo.
- **First review:** martes 2026-11-10.
- **Closes:** abierta hasta llegar a la meta, con tope el viernes 2026-12-04 (para analizar antes de mediados de diciembre, fecha del brief).
