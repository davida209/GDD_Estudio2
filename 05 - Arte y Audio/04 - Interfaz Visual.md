# Interfaz Visual

## HUD

La zona superior presenta día, tiempo restante, dinero y reputación, además de acceso a pausa e identidad del juego. La zona inferior contiene cuatro reservas de bodega, equipo actual, acción contextual/progreso y objetivos del turno.

Sobre cada anaquel se muestran existencias y capacidad. Las compras, reposiciones y limpiezas tienen retroalimentación cerca de la acción. Los avisos de ladrón, visita del dueño y cambio de día deben distinguirse de los contadores permanentes.

## Jerarquía visual

Primero se leen amenazas inmediatas, reputación y tiempo. Después, equipo y acción disponible. En tercer lugar, bodega y avance de objetivos. Esta jerarquía no debe ocultar la tienda ni competir con el gesto de pago o los pies de los personajes.

## Estados

| Estado | Comunicación |
|---|---|
| Normal | Tarjetas claras, cifras y nombres estables |
| Advertencia | Aviso explícito de riesgo y color de énfasis |
| Acción en curso | Barra o indicador de progreso |
| Acción completada | Cambio de contador, producto o mancha y sonido si está activo |
| Acción no disponible | Texto contextual sobre equipo, stock o categoría |
| Fin de jornada | Panel animado con balance, reputación y siguiente día |
| Resultado final | Victoria o derrota y opciones para continuar fuera de la partida |

## Convenciones

Las tarjetas usan sprites claros, verde salvia e iconos; los acentos terracota enlazan con el mobiliario. La tipografía debe conservar contraste y caracteres españoles. La referencia de layout es 1280 × 720; no se ha certificado un tamaño mínimo universal de letra, por lo que se debe revisar también a 1920 × 1080.

Los números y etiquetas acompañan a los colores. Las animaciones de paneles son breves y no deben bloquear repetidamente la visión. No hay barras de vida, munición, minimapa ni inventario por casillas.

## Pantallas

Menú principal, instrucciones, puntuaciones, acerca de, pausa, transición diaria y resultado. Su navegación se describe en [[02 - UI y Menús]].

> **Navegación:** [[00 - Índice]] · ← [[03 - Entornos]] · [[05 - Audio y Música]] →
