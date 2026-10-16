# Sistemas

## Inventario de sistemas

| Sistema | Entradas y procesamiento | Salidas y dependencias | Estado |
|---|---|---|---|
| Jornadas | Reloj activo de 210 s y número de día | Transición, nuevo día, victoria; coordina la simulación | Implementado |
| Inventario de manos | Interacciones con cajas y trapeador | Equipo actual y modificador de movimiento | Implementado |
| Existencias | Retiro de bodega, transferencia y compras | Stock de cada categoría, productos visibles y contadores | Implementado |
| Clientes | Generación, rutas, compra y espera | Fila, ventas o insatisfacción | Implementado |
| Caja y economía | Cobros terminados, multas y robos | Balance y avisos monetarios | Implementado |
| Suciedad | Aparición limitada y limpieza | Manchas activas, objetivos y reputación | Implementado |
| Reputación | Manchas, vacíos, insatisfacción, robos y auditorías | Valor 0–100 y posible derrota | Implementado |
| Ladrón | Aparición, acceso a caja y tiempo de robo | Sustracción, huida y recuperación | Implementado |
| Dueño | Temporizador, aviso y recorrido | Inspección, multa y penalización reputacional | Implementado |
| Presentación | Eventos de todos los sistemas | HUD, animaciones, sonidos y transiciones | Implementado |
| Puntuaciones | Fin de partida y nombre del jugador | Registro local y lista ordenada | Implementado; servicio remoto sin configurar |

## Reputación

La reputación se limita entre 0 y 100. Se calcula a partir de una base de 100, menos **8 por mancha activa**, **10 por anaquel vacío**, **3 por cliente insatisfecho registrado**, **12 por robo monetario consumado** y las pérdidas acumuladas de inspección.

Limpiar y reponer eliminan las penalizaciones temporales correspondientes. Cada inspección agrega una pérdida acumulada de **3 por mancha y 2 por anaquel vacío**. El registro de clientes insatisfechos se reinicia después de evaluar la inspección; las pérdidas por robos e inspecciones permanecen durante la partida.

## Inspección del dueño

El dueño avisa, camina hasta un punto libre, revisa el local, comunica el resultado y sale. En el día d, multa si la reputación evaluada es menor que `50 + 1.5 × (d − 1)`, o hay al menos dos manchas, o al menos dos anaqueles vacíos. La multa es `$200 + $20 × (d − 1)`. El aviso previo empieza en 10 segundos y baja medio segundo por día hasta siete.

## Relaciones y riesgos

La bodega abastece cajas; las cajas abastecen anaqueles; los clientes retiran existencias y pagan mediante el sistema de caja. Suciedad, ventas fallidas, robos y auditorías alimentan reputación. El gestor de jornadas determina cuándo todos estos sistemas pueden avanzar. Los eventos de cambio actualizan HUD y objetivos.

Se deben evitar cobros duplicados, recursos negativos, penalizaciones perdidas al recalcular y NPC que atraviesen muebles. Los criterios verificables están en [[04 - Criterios de Aceptación]].

> **Navegación:** [[00 - Índice]] · ← [[02 - Mecánicas]] · [[04 - Controles]] →
