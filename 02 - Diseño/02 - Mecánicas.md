# Mecánicas

## Movimiento y manos

**Propósito:** conectar tareas dentro de la tienda. **Entrada:** WASD o flechas. **Estado inicial:** jugador libre o equipado. **Reglas:** movimiento sujeto a colisiones; solo un objeto en manos. La velocidad base configurada es 3.1 unidades por segundo; con caja se multiplica por 0.8. **Estado final:** nueva posición y orientación. No hay salto, ataque ni consumo de energía.

## Recogida y devolución de cajas

**Activación:** pulsar E junto a una de las cuatro estaciones con manos disponibles. **Recurso:** cinco unidades de la categoría, descontadas de bodega. **Resultado:** caja equipada. Se requiere disponibilidad suficiente; una categoría no utiliza existencias de otra. La caja sin usar puede devolverse a su estación. Si se lleva trapeador, primero debe devolverse. No hay penalización por devolver una caja válida.

## Reposición progresiva

**Propósito:** mantener productos a la venta. **Activación:** E junto al anaquel de la misma categoría con una caja equipada. **Estado inicial:** anaquel con espacio y caja con unidades. **Procesamiento:** una unidad cada 0.18 segundos, con progreso visible. **Estado final:** caja agotada o anaquel lleno; la caja desaparece y el sobrante vuelve a bodega. **Recompensa:** existencias disponibles y recuperación de la penalización por anaquel vacío cuando deja de estarlo.

**Casos límite:** un anaquel en 18/20 recibe dos de las cinco unidades y devuelve tres a bodega. La categoría incorrecta no transfiere productos. Alejarse más del rango de continuidad interrumpe la transferencia; la caja conserva lo restante. Nunca se supera la capacidad de 20.

## Limpieza

**Activación:** equipar trapeador con E en su estación y mantener E junto a una mancha. **Estado inicial:** mancha activa y herramienta equipada. **Proceso:** interacción sostenida, aproximadamente 2.25 segundos en la configuración actual. **Resultado:** desaparece la mancha y se actualiza el objetivo diario. **Recursos:** tiempo y ocupación de manos. Se recupera la parte de reputación asociada a esa mancha; no elimina penalizaciones históricas de inspecciones.

## Cobro manual

**Activación:** E en la zona de caja cuando hay un cliente esperando. **Estado inicial:** compra preparada y primer cliente de la fila disponible. **Proceso:** animación de pago dirigida a la registradora y progreso de cobro de aproximadamente 2.4 segundos. **Resultado:** ingreso por unidades realmente compradas; el cliente sale y avanza la fila. **Caso límite:** alejarse cancela un cobro incompleto; hace falta E de nuevo. Una compra terminada se abona una sola vez.

## Intercepción del ladrón

**Activación:** E al estar cerca del ladrón durante aproximación, robo o huida. **Reglas:** puede robar hasta $150 disponibles en caja tras completar su acción de cuatro segundos. Un robo con dinero sustraído resta 12 de reputación. **Resultado:** se detiene al ladrón y se recupera el dinero que lleve. La recuperación no revierte automáticamente la penalización reputacional. La caja sin dinero no produce un robo monetario ni esa penalización.

## Mecánicas complementarias

Esc abre o cierra pausa durante el juego activo. Los objetivos diarios cuentan reposiciones y limpiezas. Las pantallas de resultado permiten repetir o volver al menú. Las inspecciones y la compra de NPC son procesos automáticos descritos en [[03 - Sistemas]].

> **Navegación:** [[00 - Índice]] · ← [[01 - Jugabilidad]] · [[03 - Sistemas]] →
