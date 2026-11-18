# Correcciones

Registro vivo de lo que el fundador corrigió de las propuestas de la IA, y por qué.
Cada `/review-evidence` agrega una entrada fechada al final.

## 2026-10-27

Primera revisión de evidencia (cubre del 2026-10-13 al 2026-10-27).

- **Artifact:** product/overview.md
  **AI proposed:** La sección "Para quién" incluía el caso del fundador como referencia (30–35 botellas, Vivino y AppSheet abandonados).
  **Human decided:** Describir el segmento de forma genérica, sin el caso personal del fundador.
  **Why:** El overview describe al segmento, no al fundador; el caso del fundador es n=1 y el más sesgado.

- **Artifact:** product/overview.md
  **AI proposed:** Orden de creencias con "la duda de qué botella abrir" en primer lugar y "la carga del stock" en segundo.
  **Human decided:** Subir la creencia de la carga y el mantenimiento del stock al primer lugar.
  **Why:** Si cargar y mantener el stock sigue siendo trabajoso, nadie llega a usar las recomendaciones; es el riesgo que hay que atacar primero.

- **Artifact:** product/personas/lucas-fernandez.md, product/personas/elena-valdivia.md
  **AI proposed:** Tertiary como "Lucía", la pareja que no entiende de vino y desordena la cava; negative como "Ernesto", coleccionista experto, hombre y mayor.
  **Human decided:** Cuestionó si el género era relevante; se invirtieron los géneros (Lucas y Elena) sin cambiar rol, tipo ni conducta.
  **Why:** El género no influye en ninguna creencia, y las asignaciones originales calzaban con estereotipos que pueden sesgar las entrevistas sintéticas.

- **Artifact:** product/opportunities/2026-10-19-1642-elegir-vino-de-mi-stock.md
  **AI proposed:** Centrar el segmento en Carolina y tratar a Tomás (pocas botellas, mayormente regaladas) como borde.
  **Human decided:** Incluir a Tomás en el segmento.
  **Why:** También sufre el problema, aunque de forma esporádica; la investigación debe distinguir los dos subgrupos.

- **Artifact:** product/opportunities/2026-10-19-1642-elegir-vino-de-mi-stock.md
  **AI proposed:** Construcción low code como restricción de recursos.
  **Human decided:** Low code es deseable, no obligatorio.
  **Why:** El fundador no quiere cerrar opciones técnicas; además agregó como restricción el costo en tokens de las recomendaciones.

- **Artifact:** product/overview.md (creencia 3)
  **AI proposed:** Umbral de retención de 40% a 3 meses sobre quienes reciben recomendaciones, elegido por la IA como punto de partida.
  **Human decided:** Recalibrar a ≥25% de los usuarios activados.
  **Why:** El benchmark de mercado (product/research/2026-10-19-1711-mercado-cava-recomendacion-stock.md) da un rango defendible de 20–30% sobre usuarios activados; el 40% quedaba fuera de rango.

## 2026-11-02

- **Artifact:** product/personas/carolina-mendez.md
  **AI assumed:** Carolina era `primary`.
  **Human decided:** Cambiarla a `secondary`.
  **Why:** Calzan 5/30 de quienes compran en la encuesta, 4 de ellos de la red del fundador, y ninguno de los 6 entrevistados que compran. Teresa Ibáñez representa mejor la oportunidad priorizada.

## 2026-11-12

- **Artifact:** product/solutions/2026-11-02-1857-perder-botellas-sin-abrir-a-tiempo.md (A4, `revision-de-cava`)
  **AI proposed:** Revisión dos veces al año, con lista para los próximos 6 meses. En T1, medir a las 8 semanas el compromiso de agendar la segunda revisión como indicador adelantado.
  **Human decided:** Revisión cada 3 meses, con lista para los próximos 3 meses.
  **Why:** Permite que T1 mida la creencia 12 completa (la segunda revisión real ocurre dentro de la prueba) y hace la lista más concreta. Riesgo asumido: listas casi vacías por la baja frecuencia de la pérdida; T1 lo registra. Cambio hecho antes de probar A4, así que no invalida resultados.

- **Artifact:** product/tests/2026-11-12-1239-perder-botellas-sin-abrir-a-tiempo.md (T3)
  **AI proposed:** Pasa si al menos 80% de las estimaciones cae dentro de ±1 año del experto en total y al menos 70% en vinos chilenos de productores chicos.
  **Human decided:** 75% en total y 60% en el subconjunto chileno.
  **Why:** Decisión del fundador al fijar los umbrales, antes de correr la prueba.
