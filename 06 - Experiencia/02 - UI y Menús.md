# UI y Menús

## Mapa de navegación

```text
Menú principal
├── Nombre del jugador
├── Jugar → Tienda
├── Cómo jugar → instrucciones → regresar
├── Puntuaciones → marcador local → regresar
├── Acerca de → información del juego → regresar
└── Salir

Tienda → Pausa: continuar / sonido / volver al menú
Tienda → Cierre diario → siguiente día
Tienda → Victoria o derrota: repetir / menú
```

## Pantallas y funciones

| Pantalla | Propósito y elementos | Acciones y transiciones |
|---|---|---|
| Principal | Imagen de tienda estilizada, logo original, nombre y botones | Iniciar partida, abrir paneles o salir |
| Cómo jugar | Controles, tareas, cajas de cinco, días y reputación | Leer y volver al menú |
| Puntuaciones | Registros locales, lista con desplazamiento | Consultar y cerrar |
| Acerca de | Identidad y créditos disponibles | Consultar y cerrar, incluido Esc |
| HUD | Tiempo, día, dinero, reputación, bodega, equipo y objetivos | Jugar y abrir pausa |
| Pausa | Estado detenido, controles y sonido | Continuar con botón/Esc, alternar sonido o ir al menú |
| Cierre de jornada | Resumen y anuncio animado | Avance automático tras 4.2 segundos |
| Resultado | Victoria/derrota y balance final | Repetir desde día uno o ir al menú |

## Confirmaciones y acciones que terminan sesión

Volver al menú abandona el turno; reintentar inicia una partida nueva. No hay guardado del turno para restaurarlo después. No se documenta una ventana de confirmación adicional como si ya existiera: se debe comprobar el comportamiento de los botones en la entrega y que su texto sea inequívoco.

No hay pantallas independientes de vídeo, inventario, mapa o accesibilidad. El control de sonido actual se encuentra en la pausa; no representa un menú completo de ajustes gráficos.

> **Navegación:** [[00 - Índice]] · ← [[01 - UX y Flujo del Jugador]] · [[03 - Accesibilidad]] →
