# Reglas y estados del juego

| Estado | Simulación | Salida |
| --- | --- | --- |
| Playing | Reloj y sistemas activos | Pausa, cierre o confianza cero |
| Paused | Tiempo de juego detenido | Continuar, controles, reporte, reiniciar, menú o salir |
| Closing | Tienda congelada; solo puede terminar el cobro permitido | Resumen al completar/cancelar o agotar tolerancia |
| DaySummary | Informe y simulación detenida | Siguiente jornada o victoria del desafío |
| Won | Resultado final | Nueva partida o menú |
| Lost | Despido y resultado final | Reintentar o menú |

## Cierre

Cada jornada tiene 300 segundos activos. Si al sonar el cierre ya se estaba cobrando un ticket válido, con cajero presente y espera disponible, se concede hasta tres segundos medidos con tiempo no escalado. No sirve para comenzar otro cobro. Terminado ese caso se produce el resumen.

En desafío, continuar desde el resumen del séptimo día lleva a victoria si queda confianza. En continuo comienza el día siguiente sin un final semanal obligatorio.

## Invariantes

- Una venta se registra una vez y solo por la cantidad efectivamente retirada.
- Un cliente no debe irse por un anaquel vacío si existe otro accesible con su mismo producto.
- Manos: caja, mopa o libres; nunca ambos objetos a la vez.
- Un anaquel acepta su producto exacto; básico y especialidad no son intercambiables.
- Confianza cero causa derrota; efectivo cero no la causa por sí solo.
- Visitar Warehouse no crea otra partida ni pausa la tienda.
- Las compras no permiten saldo negativo.

## Resultado semanal

La eficiencia determina rango y recompensa ficticia: S recibe PC Gamer Monster Beast; A/B una PC Gamer Gama Media; C una Computadora de Oficina Usada. No se trata de un premio físico ni una compra real.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
