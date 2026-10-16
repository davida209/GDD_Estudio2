# Arquitectura Técnica

## Organización

El juego utiliza componentes MonoBehaviour en escenas y prefabs, gestores de estado y eventos de cambio. La entrada conduce a movimiento e interacción; estas acciones modifican inventario, stock, dinero y reputación; la presentación escucha los cambios y actualiza HUD, sprites y sonido.

```text
Input System → Movimiento / interacción del empleado
                         ↓
Inventario ↔ Bodega ↔ Anaqueles ↔ Clientes / fila ↔ Cobro / economía
                         ↓
Suciedad + robos + inspección → Reputación → derrota
GameManager / DayDifficulty → reloj, estados, eventos y victoria
                         ↓
HUD + animaciones + sonido + resultados → ScoreManager
```

## Componentes principales

| Componente o área | Responsabilidad | Dependencias |
|---|---|---|
| GameManager | Día, reloj, pausa, transición y resultado | Eventos de jornada y reputación |
| DayDifficulty | Parámetros escalados por día | Día actual |
| WarehouseStockManager | Reservas por categoría y suministro | Eventos de inicio de jornada |
| EconomyManager | Balance, ventas, robos y multas | Caja, ladrón y dueño |
| OwnerInspectionManager | Aviso y evaluación del negocio | Reputación, manchas y stock |
| Inventario e interactuables | Caja/trapeador y acciones cercanas | Entrada y objetos de escena |
| StoreWalker | Rutas de NPC por zonas transitables | Mobiliario, obstáculos y destinos |
| ActorSpriteStability | Apoyo y escala visual de actores | SpriteRenderer y animación |
| SoundBank | Efectos y preferencia de sonido | Eventos y PlayerPrefs |
| ScoreManager | Puntuaciones y último nombre | PlayerPrefs, JSON y resultado |
| RemoteScoreSync | Punto de integración remota opcional | Backend sin configurar; no activo en el alcance |

## Comunicación y principios

Las referencias de escena enlazan objetos concretos; los eventos notifican cambios como stock o jornada. Los valores configurables se serializan en componentes. Debe considerarse el valor de la escena/prefab, no solo el predeterminado escrito en C#.

Mantener categorías explícitas, una sola ejecución por cobro, límites de inventario y coherencia de estados. El código temporal de construcción y pruebas permanece fuera de Assets; la entrega debe contener únicamente los recursos y herramientas necesarios.

> **Navegación:** [[00 - Índice]] · ← [[04 - Guardado y Configuración]] · [[02 - Motor y Herramientas]] →
