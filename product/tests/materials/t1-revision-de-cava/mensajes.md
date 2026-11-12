# Mensajes de T1

Se mandan por el canal que la persona prefiera (WhatsApp o correo). El texto es fijo: se puede adaptar el saludo, pero no lo que se pide ni lo que se ofrece. La fecha de envío de cada mensaje se anota en `hoja-registro.csv`.

## M1. Bienvenida (semana 0, al aceptar)

> ¡Gracias, {nombre}! Te cuento cómo funciona:
> 1. Nos mandas fotos de tu cava o una lista de lo que tienes (te explico abajo cómo).
> 2. En un máximo de 5 días hábiles te mandamos una lista corta con las botellas que conviene abrir en los próximos 3 meses, y por qué.
> 3. Pasados 3 meses, si quieres, repetimos la revisión.
> No tienes que registrar nada entre una revisión y otra.

## M2. Instrucciones para mandar la cava (semana 0, junto con M1)

> Lo que nos sirva más fácil a ti:
> - **Fotos:** de las etiquetas de frente, de a varias botellas por foto si se leen. Las que estén acostadas, basta con que se vea el cuello o la etiqueta lateral; si no se lee, saca esa aparte.
> - **Lista:** productor, nombre del vino y año, si lo tienes. Una planilla, una nota del teléfono o una foto de tu cuaderno sirven.
> - **Si tienes varias botellas iguales,** dinos cuántas.
> No hace falta que sea perfecto. Si falta alguna, no pasa nada.

## M3. Entrega de la lista (≤ 5 días hábiles desde que llegó la cava)

Se manda la plantilla de `armar-la-lista.md`, completa.

## M4. Contacto de la semana 2

> Hola {nombre}, ¿te quedó alguna duda con la lista que te mandamos? Si algo no se entiende, o alguna botella no la tienes, cuéntame.

Solo se responde lo que pregunte. No se le recuerda abrir botellas.

## M5. Ofrecimiento de la segunda revisión (semana 12, una sola vez)

> Hola {nombre}, se cumplen 3 meses de tu revisión. Si quieres tu segunda revisión, mándanos tu foto o lista, igual que la vez anterior.

No se manda un segundo aviso si no responde.

## M6. Contacto final (14 días después de M5)

Se manda a todos, hayan pedido o no la segunda revisión:

> Hola {nombre}, una última pregunta para cerrar la prueba. De la lista que te mandamos en {mes}, ¿abriste alguna botella? Si fue así, ¿cuáles y más o menos cuándo? Y si no, también me sirve saberlo.

Si responde algo ambiguo ("creo que una"), se repregunta una sola vez: "¿Te acuerdas cuál era?". Se anota tal cual en `hoja-listas.csv`.

Si no pidió la segunda revisión, se puede agregar al final, sin insistir: "¿Hubo algo que te hizo no pedir la segunda?". La respuesta va en `notas`, no cambia (b).
