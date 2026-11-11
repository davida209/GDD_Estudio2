# Arquitectura técnica

## Organización

Unity 2D y C#, con componentes por responsabilidad y eventos entre sistemas. No hay servidor de simulación: la partida se ejecuta localmente.

| Subsistema | Componentes principales |
| --- | --- |
| Estado y tiempo | GameManager, DailyDifficultyController, DailyDifficultySettings |
| Economía/confianza | EconomyManager, StoreReputationManager, OwnerInspectionManager |
| Crecimiento | StoreProgression, ProductCatalog, StoreUpgradeUI |
| Jugador | PlayerController, PlayerInteraction, PlayerCarrySystem |
| Mercancía | Shelf, StockBox, BoxSpawner, WarehouseStockManager |
| Clientes | CustomerSpawner, CustomerAI, CustomerQueue, CashRegisterZone |
| Incidencias | DirtSpawner, DirtSpot, ThiefSpawner, ThiefAI, SupervisorAI |
| Áreas y rutas | WarehouseDoor, StoreEntranceDoor, StoreNavigation, StoreGround |
| Presentación | HUDController, menús, reacciones y animadores |
| Sonido | GameAudio, GameAudioLibrary, FootstepAudio, GameAudioSettings |
| Datos | GameSession, StoreSave/StoreSaveData, ScoreManager |
| Soporte | BugReportPanel y API de la PWA |

## Escenas

MainMenu inicia el flujo. Game conserva gestores, jugador y tienda. Warehouse se carga mediante LoadSceneMode.Additive y permanece en el mismo entorno de simulación; el cambio desplaza jugador y cámara entre áreas. No se instancia otra economía al viajar.

## Datos de diseño

ProductCatalog y DailyDifficultySettings son ScriptableObjects. La escena y los prefabs pueden sobrescribir valores por defecto de los scripts; los valores de este GDD se tomaron de recursos y configuración activa cuando estaban serializados.

## Comunicación

Eventos de venta, reposición, limpieza, inspección e inicio/cierre alimentan HUD, XP, objetivos y audio. La UI valida el estado antes de permitir acciones. El reporte usa HTTPS como servicio opcional, separado del guardado y del bucle comercial.


## Gestión de la iluminación

El proyecto utiliza Built-in Render Pipeline y shaders personalizados. Cada área configura su iluminación mediante RoomLighting, que define el color ambiental, las zonas iluminadas, su intensidad, alcance y resplandor, además de las sombras de contacto del mobiliario seleccionado.

RoomLightingCamera aplica el efecto sobre la imagen del escenario y selecciona la configuración correspondiente a la tienda o la bodega según la posición de la cámara. La variación de tarde se calcula a partir del tiempo restante de la jornada.

Las sombras de contacto se generan tomando como referencia la base de los colliders configurados. El menú principal utiliza un shader independiente aplicado a su fondo ilustrado.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
