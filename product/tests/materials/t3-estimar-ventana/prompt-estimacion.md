# Procedimiento de estimación con IA (T3)

El procedimiento queda fijo antes de correr la prueba. No se ajusta el prompt después de ver alguna respuesta del sommelier: si se cambia, se descartan las estimaciones anteriores y se vuelven a correr las 30 con el prompt nuevo, y el cambio se anota en `product/corrections.md`.

## Cómo se corre

- **Herramienta:** un asistente de IA con búsqueda web activada. Se usa el mismo modelo y la misma configuración para las 30 botellas, y se anotan en `hoja-comparacion.csv` (columna `modelo`).
- **Una conversación nueva por botella**, para que una respuesta no influya en la siguiente.
- **Entrada:** solo las columnas de identificación de `set-de-botellas.csv` (productor, nombre, cepa, cosecha, país, región, tipo). No se pasa la foto ni el origen de la botella.
- **Tiempo:** se mide desde que se pega el prompt hasta que llega la respuesta final. Se anota en minutos.
- **Costo:** si la herramienta muestra tokens o costo, se anota. Si no, se deja vacío y se anota el plan usado.
- **Si la IA no responde con un año** (pide más datos o dice que no sabe), se repite una sola vez la misma pregunta. Si vuelve a no dar un año, se anota `sin estimación`, y esa botella cuenta como **fuera de ±1 año**.

## Prompt

Copiar tal cual, reemplazando lo que está entre llaves:

```
Necesito estimar hasta qué año conviene tomar este vino antes de que empiece a decaer.

Vino:
- Productor: {productor}
- Nombre: {nombre_del_vino}
- Cepa o mezcla: {cepa_o_mezcla}
- Cosecha: {cosecha}
- País y región: {pais}, {region_o_valle}
- Tipo: {tipo}

Supuesto de guarda: la botella está en una casa, acostada, en un lugar fresco y oscuro, sin cava climatizada. No sé cómo se guardó antes de llegar a la casa.

Busca información sobre este vino y este productor (ficha técnica, notas de cata, críticas, recomendaciones de guarda). Si no encuentras este vino específico, razona a partir del productor, la cepa, la región, el estilo y la cosecha, y dilo.

Responde exactamente en este formato:
Abrir antes de: {un solo año, por ejemplo 2027}
Confianza: alta | media | baja
Encontré información de este vino específico: sí | no
Fuentes: {URLs consultadas, o "ninguna"}
Razón: {dos o tres líneas}
```

## Qué se anota

Por cada botella, en `hoja-comparacion.csv`: `ia_abrir_antes_de`, `ia_confianza`, `ia_encontro_el_vino`, `ia_minutos`, `ia_costo`, y las fuentes en `ia_fuentes`.
