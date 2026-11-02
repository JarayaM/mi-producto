# Mi Cava (nombre provisorio)

mode: new · commercial

Una cava digital para aficionados al vino: registras tus botellas escribiendo solo
el nombre, y el producto completa desde internet sus características, cómo servirlas
y sus maridajes. El stock se mantiene al día con altas y bajas rápidas. Su función
central es recomendar qué vino abrir, de entre los que tienes, según la ocasión o
el plato ("voy a comer pasta, ¿qué abro?").

## Para quién

Aficionados al vino con 10 o más botellas en casa, que compran por impulso o para
guarda. Hoy no llevan registro de su stock, o lo llevan en apps como Vivino, que no
recomiendan qué abrir de entre las botellas propias.

Segmento a explorar más adelante: negocios (restaurantes, vinotecas) que lo usarían
para su propio stock.

## Creencias no verificadas

Ordenadas por impacto × incertidumbre. La primera es la siguiente a atacar.

1. [product] [value] Los aficionados no llevan registro porque cargarlo y mantenerlo
   cuesta demasiado. Si dar de alta un vino requiere solo su nombre y dar de baja es
   inmediato, mantendrían el stock al día por al menos 2 meses.
   — weakened by [product/insights/2026-11-02-1809-entrevistas-eleccion-y-registro.md] (2026-11-02)
2. [product] [value] Los aficionados con 10+ botellas tienen, al menos un par de veces
   al mes, la duda de cuál de sus propias botellas abrir para una comida, y hoy la
   resuelven mal (con la memoria, al azar o abriendo "la de siempre").
   — weakened by [product/insights/2026-11-02-1805-eleccion-y-registro-de-vino.md] (2026-11-02)
   — contradicted by [product/insights/2026-11-02-1809-entrevistas-eleccion-y-registro.md] (2026-11-02)
3. [opportunity: elegir-vino-de-mi-stock] [viability] Al menos el 25% de los usuarios
   activados (cargaron su stock y recibieron al menos una recomendación) sigue pidiendo
   recomendaciones basadas en su propio stock al menos 2 veces al mes después de 3
   meses — claramente más de lo que retuvieron Vivino u otros registros abandonados.
   *(Umbral recalibrado desde 40% el 2026-10-27 por decisión del fundador, con el
   benchmark de [product/research/2026-10-19-1711-mercado-cava-recomendacion-stock.md]
   (2026-10-19): rango defendible 20–30% sobre usuarios activados; el 40% quedaba
   fuera de rango.)*
4. [product] [value] Una recomendación limitada a su propio stock vale más para ellos
   que una de maridaje genérica (Google, Vivino, preguntarle a ChatGPT), al punto
   de que la prefieren y vuelven a usarla.
   — weakened by [product/insights/2026-11-02-1809-entrevistas-eleccion-y-registro.md] (2026-11-02)
5. [product] [viability] Los aficionados pagarían una suscripción baja (≈ USD 2–4 al
   mes) si el registro es rápido y las recomendaciones son buenas. Con un plan
   gratuito sin límites, no pagarían. *(Cifra inicial: revalidar con benchmark de
   mercado.)* — benchmark en [product/research/2026-10-19-1711-mercado-cava-recomendacion-stock.md]
   (2026-10-19): USD 2–4 está en el extremo bajo del mercado; el mercado regala el
   inventario y cobra la IA con límite de uso.
   — weakened by [product/insights/2026-11-02-1805-eleccion-y-registro-de-vino.md] (2026-11-02)
6. [opportunity: perder-botellas-sin-abrir-a-tiempo] [value] Entre quienes compran y tienen
   21–100 botellas, al menos la mitad perdió en los últimos 12 meses al menos una botella
   que quería tomar, porque la olvidó o no supo hasta cuándo aguantaba, y le importó lo
   bastante para cambiar algo: llevar una lista, abrirlas antes o gastar en evitarlo.
7. [opportunity: perder-botellas-sin-abrir-a-tiempo] [viability] Al menos el 25% de los
   usuarios activados sigue usando el producto al menos 1 vez al mes después de 3 meses,
   aunque la pérdida ocurra pocas veces al año. *(Umbral provisional: el benchmark de
   20–30% es para ≥2 veces al mes.)*
8. [opportunity: stock-incierto-en-la-cava] [value] Quienes tienen un stock compartido o
   difícil de ver pierden tiempo o dinero al menos 3 veces al año por creer que tienen o
   no tienen una botella, y hoy hacen algo para evitarlo.
9. [opportunity: stock-incierto-en-la-cava] [viability] Al menos el 25% de los usuarios
   activados mantiene un stock que coincide en al menos un 90% con lo que tiene después
   de 3 meses, y sigue consultándolo al menos 1 vez al mes.
10. [opportunity: sugerencia-maridaje-sin-botella-propia] [value] Quienes buscan maridaje
    al menos una vez al mes pierden tiempo o abren una botella peor por no poder llevar la
    sugerencia a su stock, y les importa lo bastante como para dejar de hacerlo a mano.
11. [opportunity: perder-botellas-sin-abrir-a-tiempo] [feasibility] Se puede estimar con
    precisión útil hasta cuándo aguanta cada botella del segmento, incluidos vinos chilenos
    de productores chicos, sin saber cómo se guardó.
12. [feature: revision-de-cava] [value] Al menos la mitad de quienes hicieron una revisión
    pide la segunda y abre al menos una de las botellas señaladas antes de esa segunda
    revisión. *(Umbral provisional.)*
13. [feature: revision-de-cava] [viability] Al menos el 25% de quienes hicieron una revisión
    paga por la siguiente. *(Umbral provisional, sin benchmark para este modelo.)*
14. [feature: recordatorio-por-lote] [value] En al menos la mitad de los avisos, la persona
    abre la botella o toma una decisión explícita sobre ella dentro de 30 días.
    *(Umbral provisional.)*
