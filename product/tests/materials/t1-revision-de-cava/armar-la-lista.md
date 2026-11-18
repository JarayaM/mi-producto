# Cómo armar la lista (fundador y sommelier)

## Pasos

1. **Identificar las botellas** a partir de las fotos o la lista: productor, vino, cepa, cosecha y cantidad. Las que no se puedan identificar se anotan como "no identificada" y quedan fuera.
2. **Revisar cada botella identificada** con el sommelier, con el mismo supuesto de guarda de T3: en casa, acostada, lugar fresco y oscuro, sin cava climatizada.
3. **Señalar las que conviene abrir en los próximos 3 meses:** las que ya están en su mejor momento y empezarían a decaer en menos de un año, o las que ya podrían estar pasándose. Máximo 6 botellas; si hay más, se priorizan las más cerca de pasarse y las de mayor valor para la persona.
4. **No rellenar.** Si no hay ninguna que cumpla el criterio, la lista dice eso. Se anota `botellas_en_lista = 0`.
5. **Anotar** cada botella señalada en `hoja-listas.csv` y el total en `hoja-registro.csv`.

No se usa la IA de T3 para armar la lista: aquí se prueba si la lista sirve, no quién la arma.

## Plantilla que recibe la persona (M3)

> Hola {nombre}, aquí va tu revisión. Revisamos {N} botellas de tu cava.
>
> **Conviene abrir en los próximos 3 meses:**
> 1. **{productor} {vino} {cosecha}**{si hay varias: " (tienes {n})"} — {motivo en una línea, por ejemplo: "Está en su mejor momento y desde el próximo año empezaría a perder fruta."}
> 2. …
>
> {Si no hay ninguna:} **Buenas noticias:** no vimos ninguna botella que necesite abrirse en los próximos 3 meses. Las que más se acercan son {1–2 botellas}, que conviene mirar en la próxima revisión.
>
> {Si hubo botellas no identificadas:} No pudimos leer {n} botellas; si quieres, mándanos una foto más de cerca.
>
> Pasados 3 meses te escribo por si quieres repetir la revisión.

Se entrega solo la lista. No se agregan maridajes, puntajes ni el inventario completo, porque eso no es parte de lo que se prueba.
