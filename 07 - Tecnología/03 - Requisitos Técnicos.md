# Requisitos Técnicos

## Ejecución

| Elemento | Mínimo verificable actual | Recomendación de validación |
|---|---|---|
| Sistema operativo | Windows, plataforma objetivo | Confirmar versión concreta en la compilación de entrega |
| CPU | Mínimo no medido | Medir en los equipos disponibles de evaluación |
| GPU | Mínimo no medido | Comprobar compatibilidad con la configuración URP 2D utilizada |
| RAM | Mínimo no medido | Registrar consumo real de la compilación |
| Almacenamiento | Tamaño final no medido | Medir la carpeta del ejecutable final |
| Pantalla | Referencia 1280 × 720, 16:9 | Evaluar también 1920 × 1080 |
| Entrada | Teclado y mouse | Comprobar teclado español y foco de ventanas |
| Internet | No necesario para la partida local | Probar sin conexión |

No se publican cifras de hardware inventadas. La intención de usar equipos de gama media es una meta de diseño, no un requisito mínimo certificado.

## Desarrollo

Para abrir el proyecto se necesita Unity 6000.6.3f1, sus paquetes y soporte de compilación Windows. Se requiere acceso de escritura para importar recursos y guardar puntuaciones durante las pruebas. El editor no es necesario para el futuro jugador de una compilación independiente.

## Objetivos de rendimiento

Se busca 60 FPS con la tienda, HUD y máxima fila operativos. No se han fijado umbrales medidos de carga o memoria. Deben tomarse mediciones en una compilación Windows, porque una prueba dentro del editor no representa todos los equipos de destino.

## Restricciones

No hay compilación de distribución validada ni matriz de hardware completa. El encuadre prioriza 16:9; otras relaciones requieren revisión. La calidad de animación debe comprobarse en movimiento, además de auditar claves y referencias.

> **Navegación:** [[00 - Índice]] · ← [[02 - Motor y Herramientas]] · [[04 - Datos y Persistencia]] →
