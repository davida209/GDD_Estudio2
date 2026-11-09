# Requisitos técnicos

## Objetivo de ejecución

Windows de escritorio, un jugador, teclado y mouse opcional. Relación de referencia 16:9 y 1280 × 720; revisar también 1920 × 1080. Meta de rendimiento: 60 FPS.

No hay un mínimo de procesador, tarjeta gráfica, memoria o disco medido y aprobado para el ejecutable; no se publican especificaciones deducidas del equipo de desarrollo. El tamaño final se obtiene de la build, no de la carpeta completa del proyecto.

## Red

Jugar, guardar negocio y consultar marcador local no requieren internet. Enviar un reporte necesita conexión HTTPS a la PWA. Una caída de red no debe bloquear la partida ni borrar el texto durante el intento de reporte.

## Compilación de entrega

En Build Profiles, seleccionar Windows y desactivar Development Build. Scene List: MainMenu, Game y Warehouse activadas, en ese orden. Generar fuera del repositorio y probar el ejecutable en un entorno sin Unity.

Se comparte toda la carpeta de salida, comprimida en ZIP; el .exe necesita su carpeta de datos y bibliotecas. No hay una build final auditada adjunta a esta revisión del GDD. La compilación C# previa no sustituye una prueba del paquete distribuible.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
