# Datos y persistencia

## Negocio continuo

StoreSave serializa JSON en `Application.persistentDataPath/store-checkpoint.json`. Esquema actual 2: próximo día, dinero y acumulados económicos, confianza, nivel/XP/puntos, tres rangos, cuatro especialidades, cuatro extras, ocho productos/stock de anaquel y ocho reservas.

La carga valida rangos, tamaños de arrays, dinero finito no negativo, correspondencia de puntos con nivel y coherencia de especialidades. Existe migración del esquema 1 (seis anaqueles y cuatro reservas) al esquema 2. La escritura utiliza archivo temporal y reemplazo con respaldo .bak cuando ya existe destino.

## Marcador y preferencias

| Dato | Almacenamiento |
| --- | --- |
| Lista de puntuaciones | PlayerPrefs, TurnoRosso_Scores |
| Nombre del marcador | PlayerPrefs, TurnoRosso_PlayerName |
| Exportación adicional | turno_rosso_scores.json en persistentDataPath |
| Volumen y silencio | PlayerPrefs, TurnoRosso.MasterVolume y TurnoRosso.Muted |
| Sesión de reportes | Preferencia local TurnoRosso.ReportSession, sin clave administrativa |

El marcador local guarda nombre, puntuación y victoria. Existe RemoteScoreSync como cliente opcional, pero no se acredita un ranking remoto activo solo por tener ese script.

## Servicio de reportes

El formulario envía identificador, área Juego, sección/escena, título y descripción, con versión y plataforma. Una sesión propia permite asociar el envío; un reintento idéntico reutiliza identificador para evitar duplicados. No sincroniza la partida ni el inventario con la PWA.

La ruta concreta de almacenamiento local depende de compañía/producto y plataforma. No se fijan rutas personales del equipo en la documentación pública.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
