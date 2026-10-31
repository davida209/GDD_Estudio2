# Personajes y Animación

## Requisitos por personaje

| Personaje                     | Sprites y estados                                                      | Retroalimentación                           | Estado                                     |
| ----------------------------- | ---------------------------------------------------------------------- | ------------------------------------------- | ------------------------------------------ |
| Empleado                      | Reposo y caminar direccional; transporte de caja y trapeador; limpieza | Herramienta visible, orientación y progreso | Integrado; revisión visual final pendiente |
| Clientes verde, morado y azul | Caminar, reposo, espera, molestia y pago                               | Gestos orientados a la registradora         | Integrado                                  |
| Ladrón                        | Aproximación, caminar, robo y huida                                    | Estado de amenaza y desplazamiento legible  | Integrado                                  |
| Dueño                         | Caminar, inspección y resultado                                        | Pausa de revisión, aviso y resultado        | Integrado                                  |

---

## Catálogo Visual de Sprites Direccionales

### 1. El Empleado (Jugador)
![[player.png|180]] ![[player_mecanicas.png|180]] ![[Cleaning.png|180]]

| Dirección | Reposo (Idle) | Caminar - Paso 1 | Caminar - Paso 2 |
| :--- | :---: | :---: | :---: |
| **Abajo (Frontal)** | ![[Jugador_Reposo_Abajo_01.png\|50]] | ![[Jugador_Caminar_Abajo_01.png\|50]] | ![[Jugador_Caminar_Abajo_03.png\|50]] |
| **Arriba (Espalda)** | ![[Jugador_Reposo_Arriba_01.png\|50]] | ![[Jugador_Caminar_Arriba_01.png\|50]] | ![[Jugador_Caminar_Arriba_02.png\|50]] |
| **Izquierda** | ![[Jugador_Reposo_Izquierda_01.png\|50]] | ![[Jugador_Caminar_Izquierda_01.png\|50]] | ![[Jugador_Caminar_Izquierda_03.png\|50]] |
| **Derecha** | ![[Jugador_Reposo_Derecha_01.png\|50]] | ![[Jugador_Caminar_Derecha_01.png\|50]] | ![[Jugador_Caminar_Derecha_03.png\|50]] |

### 2. Don Rosso (Dueño)
![[dueño.png|180]]

| Dirección | Reposo (Idle) | Caminar - Paso 1 | Caminar - Paso 2 |
| :--- | :---: | :---: | :---: |
| **Abajo (Frontal)** | ![[Dueno_Reposo_Abajo_01.png\|50]] | ![[Dueno_Caminar_Abajo_01.png\|50]] | ![[Dueno_Caminar_Abajo_03.png\|50]] |
| **Arriba (Espalda)** | ![[Dueno_Reposo_Arriba_01.png\|50]] | ![[Dueno_Caminar_Arriba_01.png\|50]] | ![[Dueno_Caminar_Arriba_02.png\|50]] |
| **Izquierda** | ![[Dueno_Reposo_Izquierda_01.png\|50]] | ![[Dueno_Caminar_Izquierda_01.png\|50]] | ![[Dueno_Caminar_Izquierda_03.png\|50]] |
| **Derecha** | ![[Dueno_Reposo_Derecha_01.png\|50]] | ![[Dueno_Caminar_Derecha_01.png\|50]] | ![[Dueno_Caminar_Derecha_03.png\|50]] |

### 3. El Ladrón
![[ladron.png|180]]

| Dirección | Reposo (Idle) | Caminar - Paso 1 | Caminar - Paso 2 |
| :--- | :---: | :---: | :---: |
| **Abajo (Frontal)** | ![[Ladron_Reposo_Abajo_01.png\|50]] | ![[Ladron_Caminar_Abajo_01.png\|50]] | ![[Ladron_Caminar_Abajo_03.png\|50]] |
| **Arriba (Espalda)** | ![[Ladron_Reposo_Arriba_01.png\|50]] | ![[Ladron_Caminar_Arriba_01.png\|50]] | ![[Ladron_Caminar_Arriba_02.png\|50]] |
| **Izquierda** | ![[Ladron_Reposo_Izquierda_01.png\|50]] | ![[Ladron_Caminar_Izquierda_01.png\|50]] | ![[Ladron_Caminar_Izquierda_03.png\|50]] |
| **Derecha** | ![[Ladron_Reposo_Derecha_01.png\|50]] | ![[Ladron_Caminar_Derecha_01.png\|50]] | ![[Ladron_Caminar_Derecha_03.png\|50]] |

### 4. Clientes (Verde, Morado y Azul)
![[cliente1.png|140]] ![[client2.png|140]] ![[cliente3.png|140]]

| Cliente | Reposo (Abajo) | Caminar 1 (Abajo) | Caminar 2 (Abajo) | Reposo (Espalda) | Caminar 1 (Espalda) | Caminar 2 (Espalda) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Cliente 01 (Verde)** | ![[Cliente01_Reposo_Abajo_01.png\|45]] | ![[Cliente01_Caminar_Abajo_01.png\|45]] | ![[Cliente01_Caminar_Abajo_03.png\|45]] | ![[Cliente01_Reposo_Arriba_01.png\|45]] | ![[Cliente01_Caminar_Arriba_01.png\|45]] | ![[Cliente01_Caminar_Arriba_02.png\|45]] |
| **Cliente 02 (Morado)** | ![[Cliente02_Reposo_Abajo_01.png\|45]] | ![[Cliente02_Caminar_Abajo_01.png\|45]] | ![[Cliente02_Caminar_Abajo_03.png\|45]] | ![[Cliente02_Reposo_Arriba_01.png\|45]] | ![[Cliente02_Caminar_Arriba_01.png\|45]] | ![[Cliente02_Caminar_Arriba_02.png\|45]] |
| **Cliente 03 (Azul)** | ![[Cliente03_Reposo_Abajo_01.png\|45]] | ![[Cliente03_Caminar_Abajo_01.png\|45]] | ![[Cliente03_Caminar_Abajo_03.png\|45]] | ![[Cliente03_Reposo_Arriba_01.png\|45]] | ![[Cliente03_Caminar_Arriba_01.png\|45]] | ![[Cliente03_Caminar_Arriba_02.png\|45]] |

---

## Ciclo de caminar

La secuencia es **neutro → paso izquierdo → neutro → paso derecho → neutro de cierre del bucle**. Los ciclos revisados utilizan claves en 0, 0.14, 0.28, 0.42 y 0.56 segundos. La última pose permite enlazar con el inicio. No debe sostenerse una zancada como si el personaje flotara.

La posición de los pies y la altura visual deben permanecer estables; el recorte no debe cambiar arbitrariamente la escala entre poses. ActorSpriteStability mantiene la referencia de apoyo y altura de los actores. La orientación y el volteo se mantienen consistentes durante un ciclo.

## Interacciones

La caja y el trapeador se corresponden con el equipo real. La limpieza debe tener gesto y progreso. El pago apunta hacia la registradora, con duración legible y sin reproducirse como caminata acelerada. El ladrón debe mirar hacia su desplazamiento o acción. El dueño inspecciona en suelo libre, sin animarse encima de muebles.

## Estados no aplicables

No hay animaciones de salto, caída, ataques, daño físico o muerte. La derrota se comunica por interfaz al agotarse la reputación.

## Convenciones y validación

Sprites y clips se agrupan bajo Art y Animations. Las hojas se recortan por pose, con pivotes consistentes, transparencia e importación Point. La auditoría actual revisó 77 clips; 32 ciclos de caminata fueron ajustados a la alternancia de pasos. Estos controles técnicos no sustituyen la aprobación visual del equipo en movimiento real.

> **Navegación:** [[00 - Índice]] · ← [[01 - Dirección de Arte]] · [[03 - Entornos]] →
