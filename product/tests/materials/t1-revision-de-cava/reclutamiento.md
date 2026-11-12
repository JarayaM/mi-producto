# Reclutamiento para T1 y T2

Se recluta una sola vez para las dos pruebas. Cada persona queda en **una** de ellas, anotado en `reclutamiento.csv`, columna `asignado_a`.

## Filtro del segmento

Entra quien cumple todo esto:

1. **Compra** la mayoría de sus botellas (no son mayormente regaladas).
2. Tiene **51–100 botellas** en casa. Si no se completan 16 personas, se acepta **21–50**, y se anota.
3. **No trabaja ni trabajó** en la industria del vino (incluye distribuidoras y restaurantes).
4. **No fue entrevistado** en octubre–noviembre de 2026 y no participa en la otra prueba.
5. Como máximo **2 de cada 8 personas por prueba vienen de CAV**.

## Orden de búsqueda

1. Encuestados con R2 = Sí en `Notas/Ensayo/respuestas_encuesta_50_reclutamiento.csv`, que cumplan el filtro con sus respuestas (S1, S3 y R1) y no tengan problemas de calidad anotados en `product/insights/2026-11-02-1805-eleccion-y-registro-de-vino.md`.
2. Si faltan, un nuevo llamado por Facebook o la red del fundador, con las preguntas de filtro de abajo.

## Asignación

Se alternan las personas que entran, por orden de aceptación: 1.ª a T1, 2.ª a T2, 3.ª a T1, y así sucesivamente. Así ninguna prueba se queda con los más entusiastas. Si una prueba ya tiene 2 personas de CAV, la siguiente de CAV va a la otra prueba o queda en espera.

## Preguntas de filtro (para un llamado nuevo)

1. ¿Cuántas botellas de vino tienes hoy en tu casa? (menos de 20 / 21–50 / 51–100 / más de 100)
2. Esas botellas, ¿la mayoría las compraste tú o te las regalaron?
3. ¿Trabajas o trabajaste en la industria del vino (viña, distribuidora, restaurante, vinoteca)?
4. ¿Cómo te enteraste de esto? (para el canal)

## Mensaje de invitación a T1 (revisión de cava)

> Hola {nombre}, soy {fundador}. Hace unas semanas respondiste una encuesta sobre vino y nos dijiste que podíamos contactarte. Estoy probando un servicio para quienes guardan botellas en casa: nos mandas fotos de tu cava, y un sommelier y yo te devolvemos una lista corta con las que conviene abrir en los próximos 3 meses, con el porqué. Es gratis y te toma unos 15 minutos sacar las fotos. ¿Te interesa?

## Mensaje de invitación a T2 (recordatorio)

> Hola {nombre}, soy {fundador}. Hace unas semanas respondiste una encuesta sobre vino y nos dijiste que podíamos contactarte. Estoy probando una forma simple de no olvidar botellas que uno guarda para más adelante. Es una llamada de 15 minutos en la que dejas agendados un par de avisos en tu propio calendario, y un mensaje mío un mes después de cada aviso para saber cómo te fue. ¿Te interesa?

Las dos invitaciones no dicen qué se mide. No se menciona que nos interesa si abre las botellas ni si pide otra revisión.
