# Material de T3: estimar hasta cuándo aguanta cada botella

Prueba: `product/tests/2026-11-12-1239-perder-botellas-sin-abrir-a-tiempo.md`, T3.
Creencia 11: "Se puede estimar con precisión útil hasta cuándo aguanta cada botella del segmento, incluidos vinos chilenos de productores chicos, sin saber cómo se guardó."

**Señal y umbral (fijados antes de correr):** el porcentaje de botellas cuya estimación cae dentro de ±1 año de la del sommelier. Pasa si es al menos el 75% en total y al menos el 60% en el subconjunto de vinos chilenos de productores chicos.

## Archivos

| Archivo                      | Para qué                                                                  | Quién lo usa           |
| ---------------------------- | ------------------------------------------------------------------------- | ---------------------- |
| `set-de-botellas.csv`        | Las 30 botellas: identificación y origen. Sin estimaciones                | Fundador (lo completa) |
| `prompt-estimacion.md`       | Procedimiento y prompt fijos para la estimación con IA                    | Fundador o tech        |
| `instrucciones-sommelier.md` | Qué se le pide al sommelier y cómo, sin mostrarle la estimación de la IA  | Sommelier              |
| `hoja-sommelier.csv`         | Donde el sommelier anota su respuesta (clave de respuestas)               | Sommelier              |
| `hoja-comparacion.csv`       | Hoja de registro: la estimación de la IA, la del sommelier y si coinciden | Fundador o tech        |

## Pasos

1. **Armar el set (días 1–4).** Completar `set-de-botellas.csv` según las cuotas de abajo. Solo botellas reales que alguien del segmento tenga o haya tenido, identificadas al menos por productor, nombre del vino, cepa y cosecha. Una foto de la etiqueta (frente y atrás) por botella, en `fotos/` con el `id` como nombre.
2. **Congelar el set.** Una vez completas las 30 filas, no se agregan ni se cambian botellas. Si una botella no se puede identificar, se reemplaza **antes** de este paso.
3. **Estimación con IA (días 5–7).** Correr `prompt-estimacion.md` botella por botella, en una conversación nueva para cada una. Anotar el resultado, el tiempo y el costo en `hoja-comparacion.csv`. Quien estima no ve la hoja del sommelier.
4. **Clave del sommelier (en paralelo, días 5–10).** Enviar `instrucciones-sommelier.md`, `hoja-sommelier.csv` (con las columnas de identificación ya copiadas desde el set) y las fotos. El sommelier no ve las estimaciones de la IA.
5. **Comparar (días 11–14).** Copiar el año del sommelier en `hoja-comparacion.csv`, calcular la diferencia y si cae dentro de ±1 año, y sacar los dos porcentajes: total y subconjunto chileno chico.
6. **Anotar en la prueba.** El resultado y la decisión se registran con `/analyze-solution-tests`. Los umbrales no se mueven después de ver los datos; si se cambian, se registra en `product/corrections.md`.

## Cuotas del set (30 botellas)

- **Al menos 10 de productores chilenos chicos.** Definición operativa: viña chilena que **no** pertenece a un grupo grande (Concha y Toro, VSPT/San Pedro, Santa Rita, Santa Carolina, Errázuriz, Montes, Undurraga, Ventisquero, Luis Felipe Edwards, Morandé, Emiliana, Cono Sur, Viu Manent, De Martino u otros de tamaño similar) **y** cuyo vino no se vende en cadenas de supermercado. En caso de duda, se marca `no` y no cuenta para el subconjunto.
- **Al menos 10 chilenos de viñas medianas o grandes**, para que el total no dependa solo de vinos difíciles.
- **El resto, hasta 30, importados** que aparezcan en cavas del segmento (Argentina, España, Francia u otros).
- **Mezcla de estilos:** al menos 6 blancos o rosados, al menos 4 de alta gama o hechos para guarda, y cosechas repartidas entre 2010 y 2024.

## De dónde salen las botellas, en este orden

1. **Entrevistados que compran** y aceptaron seguir en contacto: pedirles fotos de 5 a 10 etiquetas de su cava. Marcela (bodegas chicas del Maule), Felipe y Hernán son los mejores candidatos para los productores chicos.
2. **Encuestados del segmento** que aceptaron una conversación (R2 = Sí en `Notas/Ensayo/respuestas_encuesta_50_reclutamiento.csv`), sin repetir a quienes se recluten para T1 o T2.
3. **Último recurso, máximo 8 botellas:** vinos de la carta del restaurante que el sommelier no haya seleccionado ni catado. Se marcan con `origen = carta-restaurante`, porque el sommelier podría conocerlos mejor que un vino de cava particular.

Para pedir las fotos alcanza con un mensaje como este:

> Hola {nombre}, estoy probando si se puede estimar hasta cuándo conviene tomar un vino solo a partir de su etiqueta. ¿Me mandarías fotos del frente y de atrás de 5 a 10 botellas que tengas guardadas? Ojalá alguna de viñas chicas. No te pido nada más, y si quieres te cuento después qué salió para tus botellas.

## Supuesto común de guarda

La creencia dice "sin saber cómo se guardó". La IA y el sommelier estiman con el mismo supuesto: **guardada en una casa, acostada, en un lugar fresco y oscuro, sin cava climatizada**. Así se compara la estimación y no las condiciones de guarda.

## Qué queda fuera deliberadamente

- La lectura automática de fotos: la IA recibe la botella ya identificada en texto. Leer fotos se prueba aparte si T3 pasa.
- El estado real de las botellas: no se abre ninguna.
- Una interfaz o una app: todo se hace en conversaciones y planillas.
