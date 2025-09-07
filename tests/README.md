# Pruebas

Esta carpeta contendrá las pruebas unitarias e integración para el proyecto de detección de fraude.

## Estructura de Pruebas

### Pruebas Unitarias
- `test_data_processing.py`: Pruebas para funciones de procesamiento de datos
- `test_models.py`: Pruebas para modelos de machine learning
- `test_features.py`: Pruebas para feature engineering
- `test_utils.py`: Pruebas para funciones auxiliares

### Pruebas de Integración
- `test_pipeline.py`: Pruebas del pipeline completo
- `test_model_training.py`: Pruebas de entrenamiento end-to-end
- `test_prediction.py`: Pruebas de predicción

### Pruebas de Datos
- `test_data_quality.py`: Validación de calidad de datos
- `test_data_schemas.py`: Validación de esquemas de datos

## Ejecutar Pruebas

```bash
# Ejecutar todas las pruebas
pytest

# Ejecutar con cobertura
pytest --cov=src --cov-report=html

# Ejecutar pruebas específicas
pytest tests/test_models.py

# Ejecutar con verbose
pytest -v
```

## Estado Actual

🔄 **Pendiente**: Creación de pruebas después de completar notebooks
📋 **Plan**: Migrar lógica de notebooks a módulos testeable
🎯 **Objetivo**: Cobertura de código > 80%
