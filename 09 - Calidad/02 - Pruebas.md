# Pruebas

## Evidencia disponible

La última revisión del prototipo registró **90 comprobaciones sustantivas aprobadas, sin fallos**, más auditoría de 77 clips, escenas, prefabs, filtros y recortes. Los archivos fuente de evidencia son `pruebas-jornadas-y-estilo.txt`, `auditoria-jornadas-y-estilo.txt` y `dificultad-por-dia.txt`, conservados como anexos de esta documentación.

Las pruebas de jornadas adelantan el reloj a sus límites. No sustituyen una partida continua de aproximadamente 25 minutos ni una prueba de rendimiento del ejecutable final.

## Casos funcionales e integración

| ID | Precondición y pasos | Resultado esperado | Resultado registrado |
|---|---|---|---|
| T01 | Anaquel compatible con espacio; retirar caja y reponer | Caja de cinco, transferencia unitaria y contadores correctos | Aprobado en pruebas |
| T02 | Anaquel en 18/20; usar caja completa | Llega a 20 y devuelve tres a bodega | Aprobado en pruebas |
| T03 | Cliente preparado en caja; pulsar E y completar pago | Un ingreso por unidades disponibles, sin cobro automático | Aprobado en pruebas |
| T04 | Compra deseada mayor que stock disponible | Precio solo por unidades realmente retiradas | Aprobado en pruebas |
| T05 | Cliente en fila sin atención suficiente | Agota paciencia, abandona y registra insatisfacción | Aprobado en pruebas |
| T06 | Robo consumado con dinero disponible | Descuento monetario y −12 persistente en reputación | Aprobado en pruebas |
| T07 | Mancha activa; equipar trapeador y mantener E | Desaparece mancha y se actualizan reputación/objetivo | Aprobado en pruebas |
| T08 | Inspección con suciedad o vacíos suficientes | Penalización y multa correspondientes al día | Aprobado en pruebas |
| T09 | Pausar durante jornada; esperar y continuar | Reloj congelado y reanudación correcta | Aprobado en pruebas |
| T10 | Agotar reloj de días 1–6 | Transición congelada y siguiente día con 210 s completos | Aprobado mediante avance controlado |
| T11 | Agotar reloj del día 7 con reputación | Victoria; no existe día 8 | Aprobado mediante avance controlado |
| T12 | Fila máxima y recorridos de NPC | Seis posiciones libres de anaqueles y rutas válidas | Aprobado en comprobaciones |
| T13 | Inspeccionar ciclos de caminata y recortes | Alternancia de pasos, escala y apoyo estables | Comprobaciones técnicas aprobadas; revisión visual final pendiente |

## Pruebas pendientes

Sesión continua de siete jornadas, usabilidad con jugador nuevo, persistencia en ejecutable independiente, legibilidad a 720p/1080p y mediciones de rendimiento. Cada ejecución nueva debe registrar fecha, versión, equipo, pasos, resultado y evidencia; un fallo se transfiere a [[03 - Bugs y Seguimiento]].

> **Navegación:** [[00 - Índice]] · ← [[01 - Criterios de Calidad]] · [[03 - Bugs y Seguimiento]] →

## Reportes anexos

- [Comprobaciones funcionales](../Anexos/pruebas-jornadas-y-estilo.txt)
- [Auditoría de recursos](../Anexos/auditoria-jornadas-y-estilo.txt)
- [Parámetros por día](../Anexos/dificultad-por-dia.txt)
