# Niveles

## Nivel único — Tienda Turno Rosso

**Objetivo principal:** completar siete jornadas con reputación. **Objetivos secundarios:** metas diarias de reposición y limpieza. **Duración:** 210 segundos por día, más transiciones. **Dificultad:** creciente según [[05 - Progresión]]. **Entrada:** iniciar una partida desde el menú. **Salida:** victoria, derrota o regreso al menú.

Todas las mecánicas de operación se utilizan en este escenario. Los obstáculos son muebles, paredes, falta de mercancía y tareas simultáneas; el ladrón aporta riesgo económico. Las recompensas son ingresos por ventas, mantenimiento de reputación y avance diario. No hay puntos de guardado para continuar una sesión.

## Distribución funcional

La bodega reúne las cuatro categorías y la estación de limpieza. La sala de ventas distribuye anaqueles distintos con pasillos transitables. La caja y su fila ocupan una zona de atención conectada con la entrada. Este esquema describe relaciones de circulación, no coordenadas exactas:

```text
Bodega de cuatro categorías ↔ Pasillos y anaqueles ↔ Caja y fila
Estación de limpieza        ↔ Manchas del local   ↔ Entrada/salida
```

## Flujo y eventos

`Entrar al turno → evaluar tienda → atender tareas y eventos → cierre diario → siguiente día → resultado al terminar el séptimo`.

Los clientes recorren la tienda, el ladrón busca la caja y el dueño utiliza un punto de inspección libre. Los eventos no trasladan al jugador a otro nivel.

## Criterios de calidad

Los pasillos deben permitir circular y atender anaqueles sin quedar atrapado. La fila de hasta seis clientes debe evitar muebles. Mostrador, contadores y avisos no deben ocultar por completo al empleado. La categoría de cada anaquel y caja debe ser reconocible por texto e imagen. Las transiciones deben distinguir claramente el fin de una jornada.

> **Navegación:** [[00 - Índice]] · ← [[01 - Estructura del Contenido]] · [[03 - Enemigos y NPC]] →
