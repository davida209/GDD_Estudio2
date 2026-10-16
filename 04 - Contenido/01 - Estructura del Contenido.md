# Estructura del Contenido

## Estructura

```text
Turno Rosso
├── MainMenu: jugar, instrucciones, puntuaciones y acerca de
└── Game: tienda única
    ├── Jornadas 1 a 7 con dificultad creciente
    ├── Caja, cuatro anaqueles, bodega y limpieza
    ├── Clientes, ladrón e inspecciones
    ├── Pausa y transición entre jornadas
    └── Resultado de victoria o derrota
```

## Inventario de contenido

| Tipo | Cantidad y alcance |
|---|---|
| Escenas de juego y menú | 2: MainMenu y Game |
| Mapas jugables | 1 tienda |
| Jornadas | 7; no son siete mapas distintos |
| Categorías de producto | 4: bebidas, snacks, abarrotes y limpieza |
| Anaqueles funcionales | 4, uno por categoría |
| Estaciones de cajas | 4, una por categoría |
| Herramienta de limpieza | 1 trapeador, con su estación |
| Protagonistas controlables | 1 empleado |
| Variantes visuales de cliente | 3 |
| Tipos de amenaza/supervisión | 1 ladrón y 1 dueño |
| Tipos de objetivos diarios | 2: reponer y limpiar |
| Combate, jefes y coleccionables | No forman parte del contenido |

## Dependencias

La tienda y sus colisiones preceden a rutas de NPC. Las existencias alimentan compras y reposiciones. El cobro depende de cliente y fila. Reputación integra limpieza, stock, insatisfacción, robo y auditoría. Menú, instrucciones y resultado deben describir estas mismas reglas.

> **Navegación:** [[00 - Índice]] · ← [[04 - Diálogos y Narrativa]] · [[02 - Niveles]] →
