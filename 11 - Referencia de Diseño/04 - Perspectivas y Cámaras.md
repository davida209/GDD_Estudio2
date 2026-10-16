# Perspectivas y Cámaras

## Decisión del proyecto

**Perspectiva:** top-down 2D estilizada. **Cámara:** ortográfica fija, encuadrando el local para observar tareas y recorridos. El jugador no la gira ni cambia a primera persona.

## Justificación

La vista general permite comparar rápidamente fila, anaqueles, manchas, ladrón y dueño. Los sprites muestran volumen de forma dibujada, pero el juego sigue funcionando en un espacio 2D. No se clasifica como isométrico ni 3D por la apariencia frontal de los muebles.

## Configuración y restricciones

StoreCameraFrame mantiene el encuadre; la configuración actual utiliza tamaño ortográfico 6.15 y referencia 16:9. El layout y posibles bandas de encuadre deben preservar toda la tienda y el HUD. PixelPerfectCamera está deshabilitada en el estado actual debido al encuadre y mezcla de escalas de recursos.

## Cambios durante la partida

Pausa, transición y resultado añaden paneles sobre el juego; no introducen una cámara libre o un modo de exploración distinto. Los avisos deben dejar visible la información necesaria para jugar.

> **Navegación:** [[00 - Índice]]
