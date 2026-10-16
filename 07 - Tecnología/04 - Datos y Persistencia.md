# Datos y Persistencia

## Modelo de datos

| Entidad | Campos o información | Vida útil |
|---|---|---|
| Partida | Día, reloj, estado, balance y reputación | Memoria de la sesión |
| Inventario | Equipo y unidades de caja | Memoria de la sesión |
| Tienda | Stock por anaquel, reservas, manchas y NPC | Memoria de la sesión |
| Penalizaciones | Insatisfacción, robos e inspecciones | Durante la partida, según sus reglas |
| ScoreEntry | playerName, score y won | Persistente local |
| Preferencias | Último nombre y sonido | Persistente local |

## Formato y ubicación

ScoreManager serializa una lista de ScoreEntry mediante JsonUtility en PlayerPrefs con la clave `TurnoRosso_Scores`. Guarda el último nombre bajo `TurnoRosso_PlayerName`. SoundBank utiliza `RossoSoundEnabled`.

Además exporta `turno_rosso_scores.json` en `Application.persistentDataPath`. La ubicación exacta depende de los nombres de compañía/producto configurados en Unity; no se sustituye por una ruta inventada. En Windows PlayerPrefs utiliza almacenamiento propio de la plataforma. El marcador ordena registros por puntuación descendente. El marcador utiliza el balance monetario final como puntuación y registra por separado si la partida terminó en victoria o derrota.

## Persistencia de progreso

No se serializa el estado completo de tienda ni existe recuperación del día en curso. Empezar de nuevo carga recursos iniciales. El marcador registra resultados; no equivale a guardar una partida.

## Versionado y migraciones

El formato actual no tiene un sistema de migraciones versionadas. Si se cambian campos, se deben comprobar registros anteriores antes de distribuir la nueva versión. La exportación JSON es un archivo de consulta adicional; la lectura actual del marcador se hace desde PlayerPrefs. No hay sincronización remota configurada.

> **Navegación:** [[00 - Índice]] · ← [[03 - Requisitos Técnicos]] · [[05 - Seguridad y Riesgos Técnicos]] →
