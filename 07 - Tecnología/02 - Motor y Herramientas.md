# Motor y Herramientas

## Motor y paquetes

| Elemento | Configuración documentada |
|---|---|
| Motor | Unity 6000.6.3f1 |
| Lenguaje de lógica | C# |
| Renderizado | Universal Render Pipeline 17.6, Renderer 2D |
| Física | Rigidbody2D y colisiones 2D |
| Entrada | Input System 1.20 |
| Interfaz | uGUI, Canvas, RectTransform y componentes de UI |
| Navegación | StoreWalker, rutas sobre cuadrícula y búsqueda A* propia |
| Datos locales | PlayerPrefs y JsonUtility |

## Herramientas

Unity Editor se utiliza para escenas, prefabs, animación y ejecución. Git organiza versiones del proyecto; el repositorio registrado está en la ficha. Obsidian organiza este GDD mediante Markdown y enlaces internos. Se han usado herramientas de generación de imágenes para parte del arte, además de recursos aportados por el usuario. No se fija una versión de Obsidian o Git que no esté registrada.

## Convenciones

La raíz del contenido del juego es `Assets/TurnoRosso`, con Art, Animations, Prefabs, Scenes, Scripts y Settings. Los scripts se agrupan por subsistema. Se deben preservar archivos .meta y referencias al reorganizar recursos.

Los sprites utilizan transparencia y recortes aislados, filtrado Point y sin mipmaps. La cámara es ortográfica; PixelPerfectCamera permanece deshabilitada en la configuración actual para conservar el encuadre completo con recursos de distintas escalas. Por ello no se afirma un escalado pixel perfect universal.

## Dependencias de servicios

El juego local no necesita servicios de red. La presencia de RemoteScoreSync no implica que exista backend conectado. La versión objetivo no usa cuentas, anuncios, compras integradas ni servicios multijugador.

> **Navegación:** [[00 - Índice]] · ← [[01 - Arquitectura Técnica]] · [[03 - Requisitos Técnicos]] →
