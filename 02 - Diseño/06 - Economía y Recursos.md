# Economía y recursos

## Estado inicial y límites

| Recurso | Valor actual |
| --- | --- |
| Efectivo inicial | $600, pesos del juego |
| Confianza | 100; rango de 0 a 100 |
| Anaqueles iniciales | Cuatro; 12 unidades por anaquel, capacidad de 20 |
| Reservas iniciales | 30 por producto básico; 120 unidades básicas en total |
| Reabastecimiento diario | +10 por producto desbloqueado desde el día 2, hasta 30 por producto |
| Caja de mercancía | Cinco unidades; un objeto en manos |
| Extra de anaquel | $220 por categoría; máximo cuatro extras |

## Catálogo y márgenes

Los importes son por unidad, salvo costo de caja y mejora. Margen bruto unitario es venta menos costo; no descuenta pérdidas ni multas.

| Producto | Venta | Costo/unidad | Caja de 5 | Margen/unidad | Mejora del extra | Peso de demanda |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Agua | $40 | $12 | $60 | $28 | — | 1.00 |
| Papas | $40 | $14 | $70 | $26 | — | 1.00 |
| Conservas | $40 | $16 | $80 | $24 | — | 1.00 |
| Limpiador | $40 | $18 | $90 | $22 | — | 1.00 |
| Refresco | $72 | $28 | $140 | $44 | $220 | 0.65 |
| Gourmet | $78 | $30 | $150 | $48 | $260 | 0.60 |
| Despensa+ | $88 | $35 | $175 | $53 | $300 | 0.55 |
| Concentrado | $100 | $40 | $200 | $60 | $340 | 0.50 |

El peso es relativo entre productos elegibles, no una probabilidad porcentual garantizada. La mercancía se paga al comprar la caja. Un rack agotado no vende hasta el suministro siguiente. Desbloquear una especialidad concede su reserva inicial de 30 unidades.

## Pérdidas y confianza

Un robo completado toma todo el efectivo disponible y resta 50 de confianza una sola vez, incluso si la caja estaba sin dinero. No existe recuperación del robo mediante una captura posterior. Una espera agotada penaliza 5 de confianza. La inspección detecta manchas y anaqueles críticos (≤2 unidades): resta 5/10 de confianza y multa $20/$40 respectivamente por infracción. La multa no crea deuda; se limita al efectivo disponible. Al comenzar otro día se recuperan hasta 10 de confianza, sin superar 100.

## Indicadores del informe

`Neto = ventas − robos − multas − suministros`. Las inversiones se muestran aparte y sí reducen el efectivo. `Eficiencia = (ventas − robos − multas) / ventas potenciales × 100`, limitada a 0–100; con demanda cero da 0. No debe confundirse eficiencia con margen ni efectivo con ventas.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
