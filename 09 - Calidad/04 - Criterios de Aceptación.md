# Criterios de Aceptación

## Criterios verificables

| Característica | Dado que | Cuando | Entonces |
|---|---|---|---|
| Caja de categoría | Manos libres y cinco unidades en reserva | Se pulsa E en su estación | Se equipa caja de cinco de esa categoría y baja su reserva |
| Reposición | Caja correcta y anaquel con espacio | Se activa la reposición | Entra una unidad cada 0.18 s hasta límite o agotamiento |
| Sobrante | Anaquel 18/20 y caja de cinco | Termina la reposición | Queda 20/20, desaparece la caja y vuelven tres a bodega |
| Limpieza | Trapeador y mancha cercana | Se mantiene E el tiempo requerido | La mancha desaparece y se actualizan objetivo/reputación |
| Cobro | Primer cliente listo | Se pulsa E y termina el gesto | Se cobra una sola vez, $40 por unidad real |
| Robo | Ladrón completa sustracción con dinero disponible | Se resuelve el robo | Baja balance y reputación en 12; recalcular no borra esa pérdida |
| Inspección | Dos manchas o dos anaqueles vacíos | El dueño revisa | Se aplica multa y pérdida acumulada según las reglas |
| Pausa | Partida activa | Se pulsa Esc | Reloj y simulación se detienen hasta continuar |
| Cambio de día | Finaliza día 1–6 | Termina la transición | Comienza el siguiente con 210 s, sin tiempo consumido por la transición |
| Victoria | Finaliza día 7 con reputación | Se procesa el cierre | Aparece victoria y no comienza día 8 |
| Derrota | Reputación llega a cero | Se actualiza estado | Aparece derrota y se detiene la partida |
| Animación | Actor caminando en cada dirección | Se reproduce el ciclo | Alterna neutro/izquierdo/neutro/derecho sin recortes ni saltos de apoyo |

## Aceptación del prototipo y de la entrega

Los casos funcionales anteriores tienen evidencia de comprobación; los aspectos visuales necesitan también revisión humana en movimiento. La entrega completa requiere una build Windows funcional, una sesión continua de siete días, lectura de HUD e instrucciones, persistencia de resultados y mediciones de rendimiento.

Guardar el turno no es un criterio de esta versión porque esa función no forma parte del alcance. No se marca la entrega final como aprobada mientras las validaciones pendientes sigan abiertas.

> **Navegación:** [[00 - Índice]] · ← [[03 - Bugs y Seguimiento]] · [[01 - Glosario]] →
