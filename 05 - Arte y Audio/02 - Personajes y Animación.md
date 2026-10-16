# Personajes y Animación

## Requisitos por personaje

| Personaje                     | Sprites y estados                                                      | Retroalimentación                           | Estado                                     |
| ----------------------------- | ---------------------------------------------------------------------- | ------------------------------------------- | ------------------------------------------ |
| Empleado                      | Reposo y caminar direccional; transporte de caja y trapeador; limpieza | Herramienta visible, orientación y progreso | Integrado; revisión visual final pendiente |
| Clientes verde, morado y azul | Caminar, reposo, espera, molestia y pago                               | Gestos orientados a la registradora         | Integrado                                  |
| Ladrón                        | Aproximación, caminar, robo y huida                                    | Estado de amenaza y desplazamiento legible  | Integrado                                  |
| Dueño                         | Caminar, inspección y resultado                                        | Pausa de revisión, aviso y resultado        | Integrado                                  |

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
