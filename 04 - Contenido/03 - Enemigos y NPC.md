# Enemigos y NPC

## Clientes

**Función:** consumir existencias y generar ventas. **Ubicación:** entrada, anaqueles, fila y salida. **Comportamiento:** entrar → caminar a producto → retirar unidades disponibles → formar fila → esperar cobro → pagar → salir. Si falta producto o se agota la paciencia, se registra insatisfacción y el cliente se retira.

Su velocidad configurada es 1.65 unidades por segundo. La compra deseada aumenta de una a dos y tres unidades en días 1, 4 y 7 respectivamente. Cada unidad efectivamente comprada vale $40 al cobrar. Los límites diarios de clientes son 3, 3, 4, 4, 5, 5 y 6. No tienen vida, daño ni recompensas de combate.

## Ladrón

**Rol:** amenaza a dinero y reputación. **Estados:** entrar → aproximarse a caja → robar si puede → huir; la intercepción puede detenerlo. **Velocidad:** 1.65, con multiplicador de huida 1.12, aproximadamente 1.85 unidades por segundo. **Acción:** robo de hasta $150 tras cuatro segundos; resta 12 de reputación si hubo dinero sustraído. **Debilidad:** E en proximidad. No hay ataques ni defensas de combate.

La generación limita su presencia simultánea. La dificultad aumenta su frecuencia de aparición, conservando una velocidad alcanzable. Recuperar dinero no borra la pérdida reputacional del robo ya consumado.

## Dueño

**Función:** evaluar el estado del local. **Estados:** aviso → entrada y recorrido → inspección → resultado → salida. **Velocidad configurada:** aproximadamente 1.35 unidades por segundo. El punto de revisión se ubica en espacio libre y la navegación debe rodear los muebles.

Puede multar por reputación insuficiente, dos manchas o dos anaqueles vacíos. La inspección añade una pérdida reputacional de tres por mancha y dos por anaquel vacío. No es un jefe de combate ni requiere diálogo del jugador.

## Navegación y animación

Los recorridos usan StoreWalker y búsqueda de rutas sobre el espacio transitable. La orientación visual sigue la dirección real del desplazamiento. La fila se pliega para seis clientes sin ocupar los anaqueles. Pago y revisión son estados de interacción, no desplazamientos rápidos sobre el mobiliario.

> **Navegación:** [[00 - Índice]] · ← [[02 - Niveles]] · [[04 - Objetos y Coleccionables]] →
