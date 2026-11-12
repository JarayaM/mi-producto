# Material de T2: aviso agendado

Prueba: `product/tests/2026-11-12-1239-perder-botellas-sin-abrir-a-tiempo.md`, T2.
Creencia 14: "En al menos la mitad de los avisos, la persona abre la botella o toma una decisión explícita sobre ella dentro de 30 días."

**Señal y umbral (fijados antes de correr):** el porcentaje de avisos que terminan en "abrió" o "tomó una decisión explícita" dentro de los 30 días posteriores al aviso. Pasa si es al menos el 50%.

## Archivos

| Archivo | Para qué |
|---|---|
| `../t1-revision-de-cava/reclutamiento.md` y `reclutamiento.csv` | Filtro, invitación y asignación, compartidos con T1 |
| `guion-llamada.md` | La llamada de 15 minutos en la que la persona agenda sus avisos |
| `mensajes.md` | Confirmación tras la llamada y seguimiento a los 30 días de cada aviso |
| `hoja-registro.csv` | Hoja de registro por aviso: de aquí sale el porcentaje |

## Calendario por persona

| Cuándo | Qué pasa |
|---|---|
| Semana 0 | Llamada de 15 minutos: elige 2 o 3 botellas y agenda los avisos (entre 2 y 6 semanas más adelante) |
| Semana 0 | Mensaje de confirmación con lo que agendó |
| Cada aviso + 30 días | Mensaje de seguimiento sobre esa botella |

## Qué cuenta y qué no

| Lo que hizo con la botella | Cuenta para la señal |
|---|---|
| La abrió | sí |
| Decidió cuándo abrirla: una fecha o una ocasión concreta ("el cumpleaños de mi papá, el 14") | sí |
| La regaló, la vendió o la cocinó | sí |
| Pospuso el aviso o "la voy a abrir pronto", sin fecha ni ocasión | no |
| Ignoró el aviso o no lo vio | no |
| No responde al seguimiento | no (se anota `sin respuesta`) |

## Reglas que protegen la señal

- **La persona elige las botellas y la fecha.** No se le sugiere qué botella ni se le estima cuándo conviene abrirla: eso sería A4.
- **El aviso va en su propio calendario,** creado por ella durante la llamada. Nosotros no mandamos el aviso.
- **Nada entre la llamada y el seguimiento.** Si escribe, se responde, pero no se le recuerdan las botellas.
- **Un seguimiento por aviso, a los 30 días.** Si no responde, un solo recordatorio 3 días después. Si tampoco responde, `sin respuesta`.
- **Inconclusive si se registran menos de 12 avisos** con resultado.
