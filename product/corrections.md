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
