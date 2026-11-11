# Sistemas

| Sistema      | Entrada                                  | Transformación                                  | Salida                                   |
| ------------ | ---------------------------------------- | ----------------------------------------------- | ---------------------------------------- |
| Jornada      | Modo, día y reloj                        | Simulación de 300 s y cierre                    | Informe diario o resultado final         |
| Demanda      | Arquetipo y productos instalados         | Selección ponderada, visita y búsqueda de stock | Ticket o abandono                        |
| Fila y caja  | Cliente con mercancía                    | Espera y cobro manual                           | Venta, salida o descontento              |
| Inventario   | Reservas, dinero y cajas                 | Compra y transferencia compatible               | Stock visible de anaquel                 |
| Limpieza     | Mopa, proximidad e interacción sostenida | Progreso de limpieza                            | Mancha eliminada y XP                    |
| Supervisión  | Confianza y estado del local             | Visita e infracciones observadas                | Multas y confianza perdida               |
| Robo         | Caja sin atender y temporizador          | Intento, sustracción y huida                    | Pérdida económica y reputacional         |
| Progresión   | Ventas y tareas                          | Experiencia, niveles y puntos                   | Habilidades e inversión en anaqueles     |
| Persistencia | Cierre de modo continuo                  | JSON local validado                             | Continuación al siguiente día            |
| Audio        | Eventos y posición respecto a cámara     | Mezcla y prioridad                              | Música contextual y efectos              |
| Reportes     | Título y descripción voluntarios         | Envío HTTPS                                     | Reporte de Juego en la bandeja de la PWA |

## Acoplamiento

Los componentes comparten eventos de inicio/cierre, venta, limpieza, reposición e inspección. La bodega se carga de forma aditiva y conserva los gestores de la tienda. No hay un segundo reloj ni un segundo inventario independiente.

## Decisiones de integración

Los clientes buscan otro anaquel con el mismo producto cuando el primero está vacío. Agua y Refresco son productos diferentes: no se sustituyen solo por pertenecer a bebidas. Los artículos de exhibición no generan tickets ficticios. Los paneles detienen o permiten interacción según el estado global y la disponibilidad real.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
