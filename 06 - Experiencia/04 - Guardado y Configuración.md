# Guardado y Configuración

## Guardado

Se conservan automáticamente **nombre del jugador, puntuaciones locales y preferencia de sonido**. No se guardan día, reloj, posición, manos, mercancía ni manchas de una partida en curso. No existen ranuras manuales, checkpoints ni botón de continuar un turno abandonado.

Las puntuaciones se escriben al registrar el resultado. Se almacenan en PlayerPrefs y se exportan adicionalmente como JSON en `Application.persistentDataPath`. El fallo de exportación produce una advertencia; PlayerPrefs sigue siendo la fuente de lectura del marcador.

## Configuración

| Categoría | Opciones actuales |
|---|---|
| Audio | Sonido activado o silenciado desde pausa |
| Vídeo | Sin menú de ajustes gráficos propio; encuadre y escalado definidos en el proyecto |
| Controles | Esquema fijo; sin reasignación en menú |
| Accesibilidad | Facilidades descritas en su sección; sin panel específico |
| Jugabilidad | Nueva partida con siete días y dificultad progresiva fija |

## Restablecimiento y recuperación

Reintentar reinicia los recursos del turno y conserva las preferencias y registros locales. Volver al menú no guarda la partida actual. No existe botón general de restaurar todos los ajustes ni sincronización de progreso entre equipos. La recuperación ante datos locales dañados requiere revisión técnica; no se garantiza una reparación automática que el código no implementa.

> **Navegación:** [[00 - Índice]] · ← [[03 - Accesibilidad]] · [[01 - Arquitectura Técnica]] →
