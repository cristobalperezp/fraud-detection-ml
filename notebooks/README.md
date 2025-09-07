# Notebooks Directory

Esta carpeta contiene todos los notebooks de Jupyter para el desarrollo del proyecto de detección de fraude.

## Notebooks Principales

### 1. `01_EDA.ipynb` - Análisis Exploratorio de Datos
- Exploración inicial del dataset
- Análisis de la distribución de clases
- Identificación de patrones y correlaciones
- Visualizaciones de variables clave
- Detección de valores atípicos

### 2. `02_Data_Preprocessing.ipynb` - Preprocesamiento de Datos
- Limpieza y validación de datos
- Normalización/estandarización de features
- Balanceo de clases (SMOTE, undersampling)
- División en conjuntos de entrenamiento, validación y prueba
- Feature engineering

### 3. `03_Model_Training.ipynb` - Entrenamiento de Modelos
- Implementación de diferentes algoritmos:
  - Logistic Regression
  - Random Forest
  - XGBoost
  - LightGBM
- Configuración de hiperparámetros
- Validación cruzada

### 4. `04_Model_Evaluation.ipynb` - Evaluación de Modelos
- Métricas de evaluación (Precision, Recall, F1, ROC-AUC)
- Matrices de confusión
- Curvas ROC y Precision-Recall
- Comparación de modelos
- Optimización de umbrales

### 5. `05_Model_Interpretability.ipynb` - Interpretabilidad con SHAP
- Análisis SHAP para explicabilidad
- Feature importance
- Interpretación de predicciones individuales
- Identificación de patrones de fraude

## Orden de Ejecución

Los notebooks están diseñados para ejecutarse en orden secuencial (01 → 02 → 03 → 04 → 05), aunque cada uno puede ejecutarse independientemente si los datos necesarios están disponibles.

## Notas

- Todos los notebooks incluyen documentación detallada
- Se recomienda usar un entorno virtual con todas las dependencias instaladas
- Los resultados se guardan automáticamente en la carpeta `results/`
