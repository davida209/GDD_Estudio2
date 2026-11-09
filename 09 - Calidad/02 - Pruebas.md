# Pruebas

## Evidencia y alcance

La versión se publicó en main el 9 de noviembre de 2026 después de la validación funcional del proyecto. La validación técnica disponible incluye revisión de escenas en Play, compilación C#, referencias de los 29 clips y envío/consulta/eliminación de reportes temporales contra la API publicada; repetir un mismo identificador devolvió el reporte existente sin duplicarlo.

El 9 de noviembre se revisó el proyecto abierto en Play: menú, tienda, pausa, entrada/salida de bodega y muestra temporal de cuatro extras/especialidades. Se capturó la UI real y la consola no registró errores durante ese recorrido. Se verificó avance del reloj y de fotogramas; la entrega del ejecutable conserva sus pruebas específicas pendientes.

Los anexos de la revisión 0.2.0 contienen 90 comprobaciones declaradas y una auditoría de 77 clips. **Son evidencia histórica de otro balance**, no resultados nuevos de esta versión ni sustituto de una sesión completa.

## Matriz de verificación vigente

| ID | Caso | Resultado esperado | Estado de evidencia |
| --- | --- | --- | --- |
| T01 | Abrir pausa al iniciar partida | Panel visible y tiempo detenido | Verificado en Play el 9 de noviembre; captura actual |
| T02 | Volumen 0/50/100 y silencio | Cursor en extremos correctos, ajuste persistente | 100% y recorrido comprobados visualmente en Play; build pendiente |
| T03 | Crear y reintentar reporte idéntico | Un reporte en bandeja, borrador conservado si falla | API probada; integración del ejecutable pendiente |
| T04 | Comprar extra de cada categoría | Producto básico correcto, costo $220 | Confirmación funcional general; registrar caso específico en build |
| T05 | Mejorar extra con stock | Unidades conservadas, nuevo producto y rack | Implementación revisada; registrar caso específico |
| T06 | Un anaquel vacío y otro abastecido del mismo producto | Cliente utiliza el abastecido | Regla en código; caso dirigido pendiente de registro |
| T07 | Limpiar y cancelar | Mancha se elimina solo al completar; sonido se detiene | Integrado; confirmar mezcla del ejecutable |
| T08 | Cierre con cobro ya iniciado | Finaliza una vez dentro de tolerancia de 3 s | Implementación revisada; caso dirigido pendiente |
| T09 | Siete jornadas del desafío | Resultado semanal; no octava jornada | Prueba completa con tiempos/equipo por registrar |
| T10 | Continuo: guardar, salir y cargar | Próximo día con inventario y mejoras conservados | Prueba de distribución por registrar |
| T11 | Recorridos y manos equipadas | Sin paso por muebles ni encogimiento de actor | Revisado en iteraciones; regresión final pendiente |

## Cómo registrar nuevas pruebas

Anotar fecha, revisión, equipo, plataforma, modo, pasos, resultado y captura/log pertinente. No marcar Aprobado únicamente por encontrar un método en código. Los fallos se registran en [03 - Bugs y Seguimiento](03%20-%20Bugs%20y%20Seguimiento.md).

## Anexos históricos

- [Comprobaciones 0.2.0](../Anexos/pruebas-jornadas-y-estilo.txt).
- [Auditoría 0.2.0](../Anexos/auditoria-jornadas-y-estilo.txt).
- [Balance histórico](../Anexos/dificultad-por-dia.txt).

Sus tiempos y penalizaciones pueden diferir de [02 - Niveles](../04%20-%20Contenido/02%20-%20Niveles.md) y [06 - Economía y Recursos](../02%20-%20Dise%C3%B1o/06%20-%20Econom%C3%ADa%20y%20Recursos.md), que describen la revisión vigente.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
