# Personajes y animación

## Recursos comprobados

Las imágenes de esta sección se extrajeron de los sprites referenciados por los clips del proyecto abierto en Unity el 9 de noviembre de 2026. Los GIFs reproducen sus fotogramas y tiempos de clave, alineados por el pivote exportado del sprite. Son previsualizaciones de los clips, no capturas de movimiento en la escena: la velocidad del Animator y los ajustes de apoyo del actor pueden modificar la presentación durante el juego.

No se utilizan hojas de personajes de otra versión. Las capturas de la partida actual están en [Registro visual](06%20-%20Registro%20visual.md).

| Personaje | Sprite de referencia | Función |
| --- | --- | --- |
| Encargado | ![[Media/Revision_2026-11-09/Player.png\|100]] | Jugador, cajas y limpieza |
| Cliente 01 | ![[Media/Revision_2026-11-09/Customer01.png\|100]] | Comprador |
| Cliente 02 | ![[Media/Revision_2026-11-09/Customer02.png\|100]] | Comprador |
| Cliente 03 | ![[Media/Revision_2026-11-09/Customer03.png\|100]] | Comprador |
| Supervisor | ![[Media/Revision_2026-11-09/Owner.png\|100]] | Inspección |
| Ladrón | ![[Media/Revision_2026-11-09/Thief.png\|100]] | Intento de robo y huida |

## Caminatas del proyecto

| Personaje  | Frente                                                       | Espalda                                                    | Izquierda                                                    | Derecha                                                       |
| ---------- | ------------------------------------------------------------ | ---------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------- |
| Encargado  | ![[Media/Revision_2026-11-09/Player_Walk_Down.gif\|100]]     | ![[Media/Revision_2026-11-09/Player_Walk_Up.gif\|100]]     | ![[Media/Revision_2026-11-09/Player_Walk_Left.gif\|100]]     | ![[Media/Revision_2026-11-09/Player_Walk_Right.gif\|100]]     |
| Cliente 01 | ![[Media/Revision_2026-11-09/Customer01_Walk_Down.gif\|100]] | ![[Media/Revision_2026-11-09/Customer01_Walk_Up.gif\|100]] | ![[Media/Revision_2026-11-09/Customer01_Walk_Left.gif\|100]] | ![[Media/Revision_2026-11-09/Customer01_Walk_Right.gif\|100]] |
| Cliente 02 | ![[Media/Revision_2026-11-09/Customer02_Walk_Down.gif\|100]] | ![[Media/Revision_2026-11-09/Customer02_Walk_Up.gif\|100]] | ![[Media/Revision_2026-11-09/Customer02_Walk_Left.gif\|100]] | ![[Media/Revision_2026-11-09/Customer02_Walk_Right.gif\|100]] |
| Cliente 03 | ![[Media/Revision_2026-11-09/Customer03_Walk_Down.gif\|100]] | ![[Media/Revision_2026-11-09/Customer03_Walk_Up.gif\|100]] | ![[Media/Revision_2026-11-09/Customer03_Walk_Left.gif\|100]] | ![[Media/Revision_2026-11-09/Customer03_Walk_Right.gif\|100]] |
| Supervisor | ![[Media/Revision_2026-11-09/Owner_Walk_Down.gif\|100]]      | ![[Media/Revision_2026-11-09/Owner_Walk_Up.gif\|100]]      | ![[Media/Revision_2026-11-09/Owner_Walk_Left.gif\|100]]      | ![[Media/Revision_2026-11-09/Owner_Walk_Right.gif\|100]]      |
| Ladrón     | ![[Media/Revision_2026-11-09/Thief_Walk_Down.gif\|100]]      | ![[Media/Revision_2026-11-09/Thief_Walk_Up.gif\|100]]      | ![[Media/Revision_2026-11-09/Thief_Walk_Left.gif\|100]]      | ![[Media/Revision_2026-11-09/Thief_Walk_Right.gif\|100]]      |

## Equipo y limpieza del encargado

| Con caja | Con mopa | Limpieza frontal |
| --- | --- | --- |
| ![[Media/Revision_2026-11-09/Player_CarryWalk_Down.gif\|130]] | ![[Media/Revision_2026-11-09/Player_MopWalk_Down.gif\|130]] | ![[Media/Revision_2026-11-09/Player_CleanDown.gif\|130]] |

Estos clips pertenecen a Assets/Animations/Player/Actions. La caja y el equipo pueden combinar su representación con otros renderers durante la partida; el GIF muestra la pista de sprites del clip, sin añadir componentes de la escena.

## Reglas de integración

La secuencia alterna apoyo neutro y pasos. Los recortes, pivotes y altura del actor se conservan entre poses; caminar con equipo no debe encogerlo. La cadencia de clientes utiliza WalkRate para acompañar su desplazamiento. Las capas de caja/mopa dependen de la orientación.

Se retiraron las poses sentadas y el sistema de mesa/sillas. No hay salto, ataque, daño físico ni muerte animada. El despido se comunica por interfaz.

> **Navegación:** [Índice](../00%20-%20%C3%8Dndice.md) · [Avance jugable](../00%20-%20Avance%20jugable.md)
