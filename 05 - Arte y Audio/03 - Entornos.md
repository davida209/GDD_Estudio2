# Entornos

## Zonas y elementos

| Zona | Estética y elementos | Función |
|---|---|---|
| Sala de ventas | Piso claro modular; cuatro anaqueles crema/salvia y productos por categoría | Recorridos y compras |
| Bodega | Piso y divisores diferenciados; cajas identificadas | Acceso a las cuatro reservas |
| Caja | Mostrador, registradora y espacio de fila | Pago manual y riesgo de robo |
| Limpieza | Estación de trapeador y manchas distribuidas | Mantenimiento |
| Acceso | Puerta y marcos consistentes con la tienda | Entrada y salida de NPC |
| Paredes | Revestimiento claro y paneles verdes | Delimitar y unificar el local |

## Modularidad

El suelo y las paredes utilizan módulos reutilizables. Los anaqueles comparten estructura visual, pero sus productos, categoría y existencias los diferencian. La representación de producto está separada del mueble para mostrar vaciado y llenado progresivo.

## Iluminación

La escena utiliza luz ambiente cálida y cinco luces locales de tienda mediante URP 2D. Las variaciones son discretas para conservar lectura del pixel art. No existe un ciclo meteorológico ni un sistema exterior de día/noche.

## Efectos y recursos

El feedback principal son cambios de producto, puerta, gestos, avisos y textos de recursos. No se requieren fuego, magia, clima ni efectos de combate. Los recursos necesarios son tiles de piso y pared, divisores, muebles, productos, cajas, herramientas, manchas, puerta y sus variantes, luces y materiales 2D.

## Reglas de construcción

Los módulos deben alinearse sin cortes visibles y respetar las colisiones. Las rutas de jugador, clientes y dueño deben usar suelo transitable. No se modifica un collider solo para ocultar un fallo visual. La caja no debe tapar por completo al empleado y la fila debe mantenerse fuera de los anaqueles.

> **Navegación:** [[00 - Índice]] · ← [[02 - Personajes y Animación]] · [[04 - Interfaz Visual]] →
