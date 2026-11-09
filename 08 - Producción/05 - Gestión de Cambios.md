# Gestión de cambios

## Flujo

Solicitud → revisar impacto sobre reglas, arte, colisiones y guardado → implementar cambio acotado → probar → actualizar bitácora y GDD → publicar cuando el responsable lo autorice.

## Control de versiones

Se utiliza una rama de trabajo cuando hay una función en desarrollo, pull request hacia develop y publicación de la versión probada desde develop a main. No se crea una rama de release para cada ajuste pequeño. Los recursos binarios se gestionan con Git LFS.

| Publicación | Resultado |
| --- | --- |
| PR #31 | Audio, interacción de menús y reportes a develop |
| PR #32 | Versión probada de develop a main |
| Revisión de referencia | b28eaa1, 9 de noviembre de 2026 |

## Documentación

La bitácora personal permanece fuera del repositorio del juego. Este GDD tiene su propia carpeta y no cambia scripts al actualizar reglas documentadas. Los anexos históricos no se sustituyen silenciosamente por supuestas pruebas nuevas.

Si cambia duración, precio, control, límite o requisito de una compra, se actualizan todas las páginas que lo mencionan y el historial. El esquema de guardado se revisa si se altera la estructura de datos. No se cambia un dato administrativo o crédito por deducción.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
