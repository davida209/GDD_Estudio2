# Seguridad y riesgos técnicos

## Límites y medidas

| Riesgo | Medida actual / acción necesaria |
| --- | --- |
| Saldo o stock inválido | Validar compra, capacidad y compatibilidad antes de modificar |
| Doble venta | Ticket y estado de cobro; registrar ingreso una vez |
| Archivo de guardado inválido | Validación de esquema, rangos y arrays; escritura temporal y respaldo |
| Referencias UI ocultas | Buscar componentes inactivos cuando se prepara la pausa |
| Reporte duplicado | UUID de envío reutilizado durante reintento idéntico |
| Conexión caída | Mensaje de error y borrador conservado durante la sesión |
| Exposición de administración | Clave de revisión y credenciales del backend permanecen en servidor |
| Datos personales en diagnóstico | Se envían solo texto voluntario, escena, versión y plataforma; no logs ni archivos |
| Derechos de recursos | Conservar créditos y verificar autorización de audios suministrados antes de distribución |

## Servicio externo

La PWA expone un envío HTTPS y una bandeja privada. La integración del juego no concede lectura administrativa. En WebGL se abre el formulario web por las restricciones del navegador; no se declara equivalencia técnica del cliente Windows.

## Riesgos pendientes

Rendimiento y memoria en build, recuperación ante interrupción durante guardado, migración con archivos reales de versiones previas y comportamiento de red lento. Los archivos locales de una partida individual no constituyen protección antitrampa; el juego no se presenta como competitivo online seguro.

Los controles del servidor, permisos y límites de abuso deben revisarse al ampliar la distribución pública de reportes. No se modifica el backend como parte de esta edición documental.

> **Navegación:** [00 - Índice](../00%20-%20%C3%8Dndice.md) · [00 - Avance jugable](../00%20-%20Avance%20jugable.md)
