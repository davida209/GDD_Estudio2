# Turno Rosso: avance jugable

**GDD 0.3.0 · 9 de noviembre de 2026 · revisión b28eaa1.**

El encargado atiende una tienda con cuatro productos básicos y puede comprar cuatro anaqueles adicionales, especializarlos y mejorar su eficacia. La bodega separada conserva los sistemas de la tienda activos: ir por cajas deja clientes esperando y obliga a organizar la ruta.

## Recorrido de una sesión

Menú → Invitado o editar nombre → desafío / tienda continua / continuar → tienda y bodega → informe de jornada → siguiente día o resultado.

| Área | Contenido vigente |
| --- | --- |
| Tiempo | Jornadas de cinco minutos; desafío de siete días o continuo |
| Oferta | Agua, Papas, Conservas y Limpiador; Refresco, Gourmet, Despensa+ y Concentrado |
| Suministro | Comprar cajas de cinco desde racks; básicos a derecha y especialidades a izquierda |
| Atención | Tres arquetipos, demanda real, búsqueda de otro anaquel válido, fila y cobro sostenido |
| Vida del local | Visitas ambientales a exhibidores sin venta ficticia de esos artículos |
| Incidencias | Manchas transitables, mopa, supervisor y ladrón |
| Crecimiento | Cuatro extras por $220, especialización con stock conservado, diez niveles y tres habilidades |
| Interfaz | Foco a color, teclado, nombre opcional, progreso circular, pausa y volumen |
| Sonido | Tres pistas y 26 efectos, con grabaciones de acciones físicas |
| Continuidad | Guardado del negocio continuo al cerrar; marcador local |
| Soporte | Reporte de problema a la PWA desde pausa |

## Estado de verificación

La versión pasó por pruebas funcionales antes de su publicación en main. Se verificaron compilación C#, referencias de audio y envío/reintento de reportes a la API. La build Windows, su rendimiento y una matriz de casos de entrega todavía requieren registro específico; no se acredita una build auditada por esa confirmación general.

## Lectura recomendada

[01 - Jugabilidad](02%20-%20Dise%C3%B1o/01%20-%20Jugabilidad.md) → [02 - Mecánicas](02%20-%20Dise%C3%B1o/02%20-%20Mec%C3%A1nicas.md) → [05 - Progresión](02%20-%20Dise%C3%B1o/05%20-%20Progresi%C3%B3n.md) → [06 - Economía y Recursos](02%20-%20Dise%C3%B1o/06%20-%20Econom%C3%ADa%20y%20Recursos.md). Para arte: [02 - Personajes y Animación](05%20-%20Arte%20y%20Audio/02%20-%20Personajes%20y%20Animaci%C3%B3n.md) y [06 - Registro visual](05%20-%20Arte%20y%20Audio/06%20-%20Registro%20visual.md). Para entrega: [02 - Pruebas](09%20-%20Calidad/02%20-%20Pruebas.md) y [04 - Criterios de Aceptación](09%20-%20Calidad/04%20-%20Criterios%20de%20Aceptaci%C3%B3n.md).
