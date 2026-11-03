# Dirección de Arte

## Identidad visual

![[Logo.png|280]]

**Estilo:** pixel art 2D de tienda de conveniencia, con personajes de proporciones pequeñas y objetos claros. **Sensación:** local cálido y cotidiano bajo presión de trabajo. **Realismo:** estilizado; el menú debe guardar relación con los sprites del juego. **Formas:** rectángulos en muebles y tarjetas, siluetas reconocibles en personajes y herramientas.

La referencia directa es el arte integrado de Turno Rosso, junto con las indicaciones visuales del usuario para una tienda más detallada y legible. No se utiliza una estética medieval para el HUD.

## Paleta

| Función                             | Tratamiento                                             |
| ----------------------------------- | ------------------------------------------------------- |
| Base ambiental                      | Crema y tonos claros de piso y paredes                  |
| Identidad de mobiliario y tarjetas  | Verde salvia                                            |
| Acentos de anaqueles y señalización | Terracota                                               |
| Texto y separación                  | Oscuros contrastantes y bordes discretos                |
| Información jugable                 | Color acompañado de números, nombres, iconos o progreso |

No se fijan aquí códigos hexadecimales distintos de los recursos actuales; la referencia concreta son las texturas integradas.

## Iluminación y materiales

Iluminación cálida mediante URP 2D, ambiente global y luces locales. Los materiales representan metal pintado, cartón, vidrio y revestimientos mediante sprites. No se busca acabado fotorealista ni materiales 3D complejos.

## Reglas visuales

1. Mantener escala, perspectiva y apoyo de pies coherentes entre personajes.
2. Importar pixel art con filtrado Point, sin mipmaps y sin compresión que dañe el borde.
3. Recortar cada sprite sin fragmentos de poses u objetos vecinos.
4. Mostrar anaqueles vacíos cuando no tienen existencias y productos según stock real.
5. Conservar exactamente el logo original proporcionado por el usuario.
6. Evitar que decoración, luces o paneles oculten interacciones esenciales.

## Hojas de Sprites Originales y Referencias

### Hojas de Jugador
|                                Hoja Base                                |                                 Hoja de Mecánicas                                 |                          Animaciones de Limpieza                          |
| :---------------------------------------------------------------------: | :-------------------------------------------------------------------------------: | :-----------------------------------------------------------------------: |
| ![[player.png\|160]] | ![[player_mecanicas.png\|160]] | ![[Cleaning.png\|160]] |


### Hojas de NPCs y Amenazas
|                         Don Rosso (Dueño)                          |                              El Ladrón                              |                          Cliente 01 (Verde)                           |                         Cliente 02 (Morado)                          |                           Cliente 03 (Azul)                           |
| :----------------------------------------------------------------: | :-----------------------------------------------------------------: | :-------------------------------------------------------------------: | :------------------------------------------------------------------: | :-------------------------------------------------------------------: |
| ![[dueño.png\|120]] | ![[ladron.png\|120]] | ![[cliente1.png\|120]] | ![[client2.png\|120]] | ![[cliente3.png\|120]] |


## Referencia interna

Las capturas anexas del local y HUD muestran el estado documentado. El origen de recursos se registra en [[02 - Referencias e Inspiración]].

> **Navegación:** [[00 - Índice]] · ← [[05 - Misiones y Desafíos]] · [[02 - Personajes y Animación]] →
