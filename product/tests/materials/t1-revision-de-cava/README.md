# Material de T1: revisión de cava hecha a mano

Prueba: `product/tests/2026-11-12-1239-perder-botellas-sin-abrir-a-tiempo.md`, T1.
Creencia 12: "Al menos la mitad de quienes hicieron una revisión pide la segunda y abre al menos una de las botellas señaladas antes de esa segunda revisión."

**Señal y umbral (fijados antes de correr):** por persona, (a) si abrió al menos una botella de su lista antes de la segunda revisión, y (b) si mandó su foto o lista dentro de los 14 días del mensaje de la semana 12. Pasa si al menos 4 de 8 cumplen (a) y (b).

## Archivos

| Archivo | Para qué |
|---|---|
| `reclutamiento.md` | Filtro del segmento y mensajes para invitar. Es común a T1 y T2 |
| `reclutamiento.csv` | Registro de candidatos, con la columna `asignado_a` para que nadie quede en T1 y T2 a la vez. Común a T1 y T2 |
| `mensajes.md` | Todos los mensajes de T1, en orden y con su texto fijo |
| `armar-la-lista.md` | Cómo arman la lista el fundador y el sommelier, y la plantilla que recibe la persona |
| `hoja-registro.csv` | Hoja de registro por persona: de aquí salen (a), (b) y el conteo de botellas por lista |
| `hoja-listas.csv` | Cada botella señalada, con su motivo y si se abrió |

## Calendario por persona

| Semana | Qué pasa | Mensaje |
|---|---|---|
| 0 | Acepta participar. Recibe las instrucciones | M1, M2 |
| 0–1 | Manda su foto o lista | — |
| ≤ 5 días hábiles después | Recibe su lista | M3 |
| 2 | Un único contacto para dudas | M4 |
| 12 | Ofrecimiento de la segunda revisión, sin insistir | M5 |
| 12 + 14 días | Contacto final: qué abrió de la lista | M6 |

## Reglas que protegen la señal

- **Ningún recordatorio de botellas entre la semana 2 y la 12.** Si la persona escribe, se responde lo que pregunta, pero no se le recuerda la lista. Recordar sería probar A2.
- **No se rellena la lista.** Si una cava no tiene nada que convenga abrir en 3 meses, la lista va con 0 o 1 botella y se anota así. Ese conteo es lo que dice si la frecuencia de 3 meses sirve.
- **El mensaje de la semana 12 es uno solo.** No se manda un segundo aviso si no responde. Pedir la segunda revisión tiene que salir de la persona.
- **"Me interesa" no cuenta como (b).** Solo cuenta si manda la foto o la lista.
- **La segunda revisión sí se entrega** a quien la pida, aunque la prueba ya haya medido lo suyo. Es parte de lo que se le ofreció.
- **Gratis durante la prueba.** No se habla de precio hasta el paso siguiente (creencia 13).

## Carga para el sommelier

Son 8 cavas de 21–100 botellas, más las segundas revisiones. Conviene acordar con él de antemano unas 8 sesiones de 30–45 minutos repartidas en las semanas 1–3, y otras tantas en las semanas 13–15.
