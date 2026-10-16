# Seguridad y Riesgos Técnicos

## Riesgos

| Riesgo | Probabilidad cualitativa | Impacto | Mitigación |
|---|---|---|---|
| Perder referencias al mover recursos | Posible en reorganización | Alto | Mover con sus .meta y auditar escenas/prefabs |
| Rutas de NPC dentro de muebles | Posible al cambiar layout | Alto | Revisar cuadrícula, colisiones y destinos libres |
| Cobro o stock duplicado | Posible al modificar interacción | Alto | Una operación por acción y pruebas de límites |
| Pausa o transición que consume tiempo | Posible al modificar estados | Alto | Probar reloj y escala temporal en cada transición |
| Sprite con recorte o pivote incorrecto | Posible al importar arte | Medio | Auditar recortes y revisar movimiento real |
| Puntuaciones locales dañadas | Posible | Medio | Comprobar carga y conservar copia de datos al investigar |
| Rendimiento o HUD distinto por equipo | Sin medir en matriz completa | Medio | Pruebas de compilación y resoluciones |

Las probabilidades anteriores son evaluación de riesgo, no frecuencias medidas ni errores actuales confirmados.

## Datos y red

El juego guarda el nombre introducido por el jugador, puntuación, resultado y preferencia de audio. No requiere cuentas, correo, contraseñas ni datos de pago. El marcador es local y puede modificarse fuera del juego; no se presenta como competición protegida contra trampas.

No hay multijugador ni backend activo, por lo que no se diseñan autenticación o autoridad de servidor para esta versión. El código de integración remota opcional no constituye un servicio desplegado.

## Recuperación

Un cierre inesperado pierde el turno actual porque no existe guardado de sesión. Los datos locales ya escritos pueden persistir; el fallo de exportación JSON no debe impedir seguir jugando. La corrupción del marcador requiere diagnóstico: no hay restauración automática completa implementada. Se conservan copias y control de versiones para recuperar el proyecto de desarrollo.

> **Navegación:** [[00 - Índice]] · ← [[04 - Datos y Persistencia]] · [[01 - Alcance]] →
