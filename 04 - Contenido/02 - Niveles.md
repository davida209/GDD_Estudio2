# Niveles

## Espacios de juego

Game contiene la tienda, los gestores y el jugador. Warehouse es una escena de bodega cargada aditivamente al cruzar su puerta. MainMenu contiene el acceso a modos e instrucciones. La lista de compilación conserva ese orden y las tres escenas activadas.

## Jornadas y dificultad

Todas duran 300 s de juego activo. Valores del recurso `DailyDifficultySettings.asset`; intervalos en segundos. La espera de visita es base a confianza 100: la confianza baja puede acortarla, con mínimo de 20 s.

| Día | Clientes cada | Suciedad cada | Manchas máx. | Robo cada | Intentos de robo máx. | Supervisor cada |
| --- | --- | --- | ---: | --- | ---: | --- |
| 1 | 14–18 | 45–60 | 2 | 150–190 | 1 | 180–210 |
| 2 | 12–16 | 40–55 | 2 | 120–150 | 1 | 150–180 |
| 3 | 11–14 | 35–50 | 3 | 80–100 | 2 | 90–110 |
| 4 | 10–12 | 30–45 | 4 | 60–80 | 3 | 75–95 |
| 5 | 9–11 | 25–40 | 4 | 45–60 | 4 | 60–80 |
| 6 | 8–10 | 25–35 | 5 | 40–50 | 5 | 50–65 |
| 7 | 7–9 | 20–30 | 5 | 30–40 | 6 | 45–60 |

El límite configurado del generador es seis clientes activos y la fila tiene seis puestos. Los intervalos no garantizan un número exacto de eventos: influyen el límite activo, la disponibilidad y la duración de cada visita. El continuo usa desde el día ocho los valores del séptimo.

## Distribución

La tienda deja libre el recorrido acceso–anaqueles–fila y separa el puesto tras el mostrador en L. La bodega organiza básicos a la derecha, especialidades a la izquierda y pasillo central. Muebles de trabajo ocupan bordes; las marcas amarillas ayudan a leer circulación y almacenamiento. No hay colocación libre de objetos por el jugador.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
