# Análisis de encuesta: elección y registro de vino

- **source:** survey
- **Diseño:** product/surveys/2026-10-27-1318-eleccion-y-registro-de-vino.md
- **Resultados:** Notas/Ensayo/respuestas_encuesta_50_reclutamiento.csv
- **n:** 50 filas: 5 descalificadas, 42 completas y 3 parciales, 45 válidas
- **Procedencia:** el fundador confirmó el 2026-11-02 que los datos son reales. Quedan sin explicar tres cosas: 31 de las 50 filas son anteriores al archivo de diseño (2026-10-27 13:18), los correos de R3 usan `example.com` y la carpeta se llama `Ensayo`. Este análisis reemplaza los hechos sobre `respuestas_encuesta.csv` y `respuestas_encuesta_50.csv`.

## Límites

- **Tasa de respuesta:** no se puede calcular; el alcance es desconocido en los 5 canales.
- **Válidas por canal:** CAV 14, Facebook 10, LinkedIn 8, WhatsApp 7, Instagram 6.
- **Meta de ≥30 por subgrupo:** quienes compran llegan justo a 30, con 14 de CAV. Regaladas tiene 8, así que ese corte es direccional.
- **Muestra autoseleccionada:** todo el análisis es direccional y no representa al segmento.

## Diferencia entre canales

| | Red del fundador (WhatsApp, LinkedIn, Instagram) | Comunidades externas (CAV, Facebook) |
|---|---|---|
| Dudan ≥2 veces al mes | 9/21 | 1/24 |
| Les molesta elegir | 8/20 | 1/22 |
| Pagan una app premium | 1/19 | 7/22 |

Es primero un hallazgo sobre la muestra. El plan advertía que en WhatsApp algunos responden por cariño, y R01 lo declara. CAV, a su vez, sobrerrepresenta a socios comprometidos y a quienes ya pagan. La frecuencia de la duda queda sin resolver.

## Resultados por objetivo

### G1. Duda (creencia 2)

- **Se creía:** un par de veces al mes con 10+ botellas.
- **Los datos muestran:** 10/45 dudan ≥2 veces y 19/45 una vez. A 24/42 les gusta elegir y a 9/42 les molesta. En quienes compran, dudan ≥2 veces 5/30. En regaladas, 4/8, los 4 de WhatsApp (0/3 fuera de ese canal).
- **Decisión:** la oportunidad sigue, pero hay que replantearla. Tomás pasa a borde (decisión del fundador, 2026-11-02).

### G2. Botellas abiertas (creencia 3)

- **Los datos muestran:** abren ≥2 al mes 29/45, con 25/30 en compra y 0/8 en regaladas. Solo 5/45 abren ≥2 y además dudan ≥2 veces.
- **Decisión:** mantener ≥2 y reportar regaladas aparte.

### G3. Registro (creencia 1)

- **Los datos muestran:** 26/43 no llevan registro, y 17 de esos 26 nunca lo intentaron. De quienes lo dejaron (11): alta 5, baja u otros que sacan botellas 6. Los 11 citan una de las dos.
- **Decisión:** no elegir entre alta y baja; la propuesta debe resolver ambas.

### G4. Pago (creencia 5)

- **Los datos muestran:** 8/42 pagan una app, 7 de CAV: 3 bajo $2.000, 2 en $2.000–4.000, 2 en $4.001–8.000 y 1 no sabe.
- **Decisión:** no validar el precio. USD 2–4 queda en o sobre lo que paga la mayoría, en el canal que infla este dato.

### G5. Maridaje (creencia 4)

- **Los datos muestran:** buscaron 30/44. 25/30 terminaron adivinando (17) o con algo que no tenían (8), y 2/30 abrieron una botella propia sugerida. El patrón se repite en los 5 canales.
- **Decisión:** el vacío existe; falta probar que prefieran y vuelvan a usar la solución.

## Insights

## El costo es real, pero elegir no molesta

35/45 sufrieron un costo concreto, y lo más citado es que una botella pasara su mejor momento (19/45). En CAV, 13/14 disfrutan elegir y 13/14 tuvieron un costo. La propuesta quizás no sea "te digo qué abrir", sino "no pierdas botellas", algo que hoy no está en el overview.

> Evidence: "las que me regalan quedan al fondo y ahi se mueren" — R31

## Con 51–100 botellas hay un candidato distinto, poco medido

Tienen 7/7 compras repetidas y 6/7 botellas pasadas, y solo 1/7 duda seguido. Además ya pagan: 5/7 club y 3/7 app. Son pocos casos y 4 vienen de CAV, pero justifica probar esa propuesta con ellos.

> Evidence: "No saber si ya es momento de alguna que compre para guardar" — R21

## Quien sufre no paga una app

De los 9 que dudan ≥2 veces y respondieron Q12, ninguno paga una app y 7 no pagan nada. De los 8 con app premium, ninguno duda ≥2 veces. Las señales de pago no sirven como prueba para quienes tienen el problema. La excepción más útil es R24: duda seguido, paga club y cursos, y viene de un canal externo.

> Evidence: "Cargar las botellas me aburrio, ahora miro la app solo de vez en cuando" — R23, paga una app premium

## ChatGPT no resuelve el último paso, pero el vacío no siempre duele

Solo 1 de 13 usuarios de ChatGPT terminó en una botella propia, y 11 tuvieron que adivinar. De los 17 que adivinaron, a 8 les gusta elegir y a 8 les molesta. Conviene probar la recomendación desde el stock propio contra el uso de ChatGPT, sin suponer que quien adivina quiere cambiar.

> Evidence: "Tengo muchas parecidas y cuando busco maridaje igual adivino" — R24

## El registro falla por ambos lados

La carga y la baja pesan parecido. Con 11 casos no se puede priorizar una; la carga pesa más en CAV y la baja en LinkedIn.

> Evidence: "Cargarlas todas me tomo un fin de semana y lo deje" — R24; "Planifico la cena con un vino que ya no esta" — R44

## Temas de Q14 (29 respuestas, una puede tener varios)

| Tema | Menciones | Cita |
|---|---|---|
| No me cuesta o no es un problema | 8 | "En verdad no me complico, tomo lo que hay" (R32) |
| No saber qué tengo o que el registro no calza | 7 | "nunca se que queda" (R35) |
| Ocasión, visitas o combinar con la comida | 7 | "El problema es cuando invito gente" (R26) |
| Ventana de guarda o botellas que se pierden | 6 | "No se si siguen buenas, algunas tienen muchos años" (R46) |
| Cargar las botellas | 3 | "cargar una a una es lento" (R34) |
| Poco conocimiento | 2 | "yo no cacho nada" (R11) |

## Preguntas para entrevistas

- ¿Por qué dudar pesa en la red del fundador y casi nada en comunidades externas? ¿Es perfil o cortesía?
- ¿Quienes disfrutan elegir pagarían por no perder botellas?
- ¿Por qué 17 de los 26 sin registro nunca lo intentaron? Q11 no se les mostró.
- ¿Qué significa "costó decidir" para quien abre una botella al mes? R01, R02, R05, R11 y R38 reportan más dudas que botellas abiertas.
- ¿Quienes no pagan nada hoy pagarían por esto?

## Reclutamiento

Aceptaron conversar 19. Los datos de contacto están en el archivo de resultados y no se copian aquí. Antes de escribirles hay que verificarlos, porque los correos usan `example.com`.

| Prioridad | Quiénes | Por qué |
|---|---|---|
| 1. Contradicen | R21, R33, R18, R10, R15 | Dudan poco y disfrutan elegir. R21 además lleva registro, paga una app y abrió una botella propia sugerida; R33 es el único de Facebook |
| 2. Mixtos | R50, R35 | Dudan poco, pero dejaron el registro por la baja |
| 3. Confirman | R24, R44, R27, R38, R11, R07 | Dudan seguido; R24 primero, por venir de un canal externo |
| 4. Con cautela | R01 | Declara responder por cariño |

- **Excluido:** R37 marcó que no trabaja en la industria, pero en Q14 dice que trabajó años en una distribuidora.
- **Sin contacto:** R05, R28 y R47 no dejaron contacto, y a R02 solo se le puede ubicar por el grupo de WhatsApp.
- **No candidatos:** R20, R31 y R45 trabajan o trabajaron en la industria; R20, R29 y R40 tienen más de 100 botellas.
- **Sesgo del grupo:** solo 4 de los 14 con contacto directo vienen de canales externos (R21, R24, R33 y R50). Los candidatos de regaladas vienen solo de WhatsApp (R01 y R11).

## Calidad de los datos

- **Respuestas rápidas:** R48 (110 s) y R49 (95 s). R49 además dice no llevar registro y que lo sigue llevando.
- **Ambigüedad de Q9 y Q10:** R23, R31, R34 y R50 usan hoy una herramienta y dicen haber dejado un registro.
- **Industria:** R20, R31, R45 y R37 siguen en la base porque R1 solo filtra entrevistas. Sin ellos, G1 queda en 10/41.
- **Parciales:** R09, R17 y R42. Las bases cambian según la pregunta.
