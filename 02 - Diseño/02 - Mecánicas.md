# Mecánicas

## Movimiento y equipo

WASD o flechas mueven al encargado en ocho direcciones. En la escena Game la velocidad base es 2.3 unidades/s; llevar caja aplica 0.75 antes de la habilidad de transporte. Solo puede sostener una caja o la mopa. Q o G sueltan el objeto en una posición libre del suelo; un intento de soltar sin espacio no debe perderlo.

## Cajas y reposición

Cada rack vende cajas de cinco unidades de un producto. Exige manos libres, existencias, dinero suficiente y no tener otra caja del mismo producto abandonada fuera. El costo se descuenta al retirar la caja y las unidades dejan la reserva.

E o Espacio sobre un anaquel compatible transfiere `min(espacio libre, unidades de caja)` en una interacción. Si sobran unidades permanecen en la caja; si queda vacía se consume. **La reposición actual es instantánea por pulsación**, no una transferencia animada unidad a unidad. El anaquel no acepta otra categoría ni otro producto básico/especialidad de la misma categoría.

## Limpieza

La mopa se recoge en la tienda. Con ella se puede caminar sobre la mancha y mantener E o Espacio para limpiarla. Base del prefab: 2 s; duración efectiva `2 / (1 + 0.15 × rango de limpieza)`. Soltar la interacción cancela el proceso; el sonido se detiene al cancelar o completar.

## Cobro

El encargado debe estar en su puesto, con manos libres y un ticket listo. Mantener E o Espacio completa el cobro; base 1.5 s y duración efectiva `1.5 / (1 + 0.10 × rango de cobro)`. No es automático por proximidad. El progreso se representa con un círculo.

## Puertas, pausa y mejoras

La puerta industrial a bodega exige E. El acceso de clientes responde a su circulación. Esc pausa o vuelve desde una subvista. Tab abre y cierra Anaqueles, Ampliación y Habilidades. La pausa detiene la simulación; visitar el almacén no la pausa.

## Seguridad

La presencia del encargado en el puesto evita que el ladrón continúe robando. La regla actual no usa combate ni una acción de captura con E; un robo completado sustrae el efectivo disponible. Véase [03 - Enemigos y NPC](../04%20-%20Contenido/03%20-%20Enemigos%20y%20NPC.md).

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
