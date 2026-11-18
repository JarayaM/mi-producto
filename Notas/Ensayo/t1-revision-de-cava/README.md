# T1 revisión de cava: resultados sintéticos (ensayo)

> **Procedencia: `synthetic`.** Generado por Claude el 2026-11-17, para practicar el análisis. **No es evidencia.** No se cita en `product/insights/`, `product/overview.md` ni en la sección Resultados de `product/tests/2026-11-12-1239-perder-botellas-sin-abrir-a-tiempo.md`.

Simula T1 completa con el material de `product/tests/materials/t1-revision-de-cava/`. Incluye lo que mandan 8 participantes, el trabajo del fundador y el sommelier con `armar-la-lista.md`, las listas que se entregan y lo que pasa después (M4, M5 y M6).

## Archivos

| Archivo | Qué simula |
|---|---|
| `conversaciones.md` | Lo que escribe cada participante: el envío de la cava y sus respuestas a M4, M5 y M6 |
| `revision-sommelier.csv` | Cada cava línea por línea: qué se identificó, el "abrir antes de" del sommelier, su estado, su confianza y si entró en la lista |
| `sesiones-sommelier.csv` | Cada sesión de trabajo: minutos del sommelier y del fundador, botellas evaluadas y cuántas cumplían el criterio |
| `listas-entregadas.md` | El M3 que recibió cada persona, hecho con la plantilla |
| `hoja-registro.csv` | La hoja del material, llena: una fila por persona |
| `hoja-listas.csv` | La hoja del material, llena: una fila por botella señalada |

## Supuestos de la simulación

- **8 participantes, como pide el diseño.** La primera versión tenía 10 y se ajustó al diseño quitando los dos casos que no aportaban un caso borde propio. Los demás se renumeraron P1-01…P1-08 por orden de aceptación.
- **Calendario.** T1 parte el 2026-11-23. Las listas se entregan a comienzos de diciembre, M5 sale a mediados de febrero de 2027 y M6 a comienzos de marzo. Las semanas 2 a 12 coinciden con Navidad, Año Nuevo y las vacaciones de verano en Chile, y eso se nota en cuándo se abren las botellas y en quién responde.
- **Reclutamiento.** 4 de las 8 personas tienen 51–100 botellas. Las otras 4 tienen 21–50 y entraron por el plan B del filtro. Hay 2 de CAV, el máximo que permite el diseño.
- **Personas.** Son ficticias. No corresponden a encuestados ni a entrevistados.
- **Vinos.** Las etiquetas son reales y comunes en Chile. Las ventanas de guarda salen del conocimiento general sobre estilos y gamas (entrada, reserva, gran reserva, ícono, naturales), con el supuesto de guarda de T3. **No se hizo investigación web ni se consultó a un sommelier real**, así que las fechas son aproximadas y no sirven como clave para T3.
- **Criterio para señalar una botella.** Su estado es "pasándose" (abrir antes de ≤ 2026) o "decae <1 año" (está en su mejor momento y abrir antes de = 2027), con un máximo de 6 por lista. El sommelier aplica criterio en los bordes, y cuando lo hace queda anotado en `comentario_sommelier`.
- **"Antes de la 2.ª revisión".** Si la persona no pidió la segunda revisión, se cuenta hasta M6.

## Casos borde incluidos a propósito

Aparecen en los datos para practicar el análisis. Lo que muestran se lee en los datos mismos:

- Fotos borrosas y botellas no identificadas.
- Una lista sin año en varias botellas.
- Una cava con más candidatas que el tope de 6.
- Una lista vacía.
- Vinos naturales de productores chicos, con baja confianza del sommelier.
- Una respuesta ambigua en M6, con su repregunta.
- Un "me interesa" sin material.
- Un envío fuera del plazo de 14 días.
- Una persona que abandona la prueba.
