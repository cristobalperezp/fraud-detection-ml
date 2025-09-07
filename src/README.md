# Código Fuente

Esta carpeta está destinada para el código fuente del proyecto de detección de fraude. Actualmente está vacía ya que el desarrollo se está realizando principalmente en notebooks de Jupyter.

## Estructura Futura

Cuando el proyecto madure y se requiera código de producción, esta carpeta contendrá:

### `data/`
- Módulos para extracción, carga y validación de datos
- Funciones para conexión a bases de datos
- Utilidades para limpieza de datos

### `features/`
- Módulos de feature engineering
- Transformaciones y escalado de datos
- Selección de características

### `models/`
- Clases para entrenamiento de modelos
- Funciones de evaluación
- Utilidades para serving de modelos

### `utils/`
- Funciones auxiliares
- Configuración y logging
- Utilidades comunes

### `main.py`
- Punto de entrada principal de la aplicación
- Orquestación del pipeline completo

## Migración desde Notebooks

Una vez que los notebooks estén completados y validados, el código se puede refactorizar y migrar a módulos reutilizables en esta carpeta para:

- Facilitar el mantenimiento
- Permitir testing automatizado
- Preparar para deployment en producción
- Mejorar la reutilización de código

## Estado Actual

📝 **En desarrollo**: Los notebooks contienen toda la lógica actual
🔜 **Próximo paso**: Refactorización a módulos Python
🎯 **Objetivo**: Código de producción limpio y mantenible
