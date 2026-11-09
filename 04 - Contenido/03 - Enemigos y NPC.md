# Enemigos y NPC

## Cliente

Secuencia principal: entrar → visitar exhibidores opcionales → buscar producto → retirar mercancía → formar fila → esperar cobro → salir. Puede retirarse molesto si no encuentra stock válido o agota la espera. El ticket contiene solo la cantidad retirada y su precio real.

Los arquetipos Vecino, Estudiante y Oficinista restringen categorías y cantidades; véase [03 - Personajes](../03%20-%20Historia%20y%20Mundo/03%20-%20Personajes.md). El producto se escoge entre oferta instalada elegible. Al acercarse a un anaquel vacío debe buscar otro accesible con el mismo producto antes de desistir. La demanda potencial se registra una vez al entrar, incluso si no se concreta la venta.

Las visitas al café, pan y refrigeradores son ambientales: no consumen esos sprites ni elevan el ticket. No hay clientes sentados.

## Ladrón

Estados: aproximación → robo → huida → salida. Su temporizador base de código es 4 s, configurable en prefab. Si el cajero ocupa el puesto al aproximarse o durante el intento, huye. Al completar el robo sustrae todo el efectivo disponible y aplica −50 de confianza una vez; la caja vacía no evita la pérdida de confianza. No hay barra de vida ni recompensa por capturarlo.

## Supervisor

Entra, recorre puntos de inspección, comprueba su entorno y sale. Cada mancha o anaquel crítico observado se registra una vez por visita. Criterio crítico: dos unidades o menos. Multas: $20 por mancha y $40 por anaquel crítico; confianza: −5 y −10 respectivamente. No es una multa fija que aumente automáticamente cada día.

La periodicidad depende del perfil diario y de la confianza actual: menor confianza implica visitas más frecuentes. No hay combate ni jefes.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
