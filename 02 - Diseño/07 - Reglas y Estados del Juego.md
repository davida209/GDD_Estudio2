# Reglas y Estados del Juego

## Estados

La escena de menú ofrece acceso a instrucciones, puntuaciones y acerca de. En la escena de juego el gestor usa `Playing`, `Paused`, `DayTransition`, `Won` y `Lost`.

| Origen | Evento | Destino | Condición |
|---|---|---|---|
| Menú principal | Jugar | Playing, día 1 | Nueva partida |
| Playing | Esc o botón de pausa | Paused | Partida activa |
| Paused | Continuar o Esc | Playing | Misma partida |
| Playing | Reloj a cero | DayTransition | Días 1–6 |
| DayTransition | Termina animación de 4.2 s | Playing | Día siguiente, reloj nuevo de 210 s |
| Playing | Termina día 7 | Won | Reputación no agotada |
| Playing | Reputación llega a cero | Lost | Condición de derrota |
| Won o Lost | Reintentar | Playing, día 1 | Reinicio de recursos y escena |
| Pausa o resultado | Volver al menú | Menú principal | Se abandona la partida actual |

## Reglas globales

1. Siete jornadas utilizan el mismo mapa y conservan recursos de la partida.
2. Los objetivos diarios informan progreso; no son una puerta obligatoria al día siguiente.
3. Pausa y transición congelan reloj y simulación; el intervalo entre días no resta tiempo al siguiente.
4. El día siete termina en resultado; nunca comienza un día ocho.
5. Reintentar inicia una nueva partida; no recupera un turno abandonado.
6. Una multa o balance agotado no sustituyen la condición de reputación cero.

## Casos especiales

Esc no interrumpe la transición entre días. Al regresar al menú se restaura la escala temporal para evitar que una nueva partida quede congelada. El cobro incompleto se cancela al abandonar su zona. Las operaciones de stock y pago deben ejecutarse una sola vez por acción válida.

> **Navegación:** [[00 - Índice]] · ← [[06 - Economía y Recursos]] · [[01 - Premisa y Trama]] →
