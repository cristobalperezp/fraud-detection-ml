# 🚨 Fraud Detector para Transacciones Bancarias

## 📖 Descripción del Proyecto

Este proyecto implementa un sistema de detección de fraude para transacciones bancarias utilizando técnicas de Machine Learning. El objetivo es construir un pipeline robusto que pueda identificar transacciones fraudulentas con alta precisión y recall, minimizando tanto los falsos positivos como los falsos negativos.

## 🎯 Objetivos

- **Objetivo Principal**: Desarrollar un modelo de clasificación binaria para detectar fraude en transacciones con tarjeta de crédito
- **Dataset**: Credit Card Fraud Detection de Kaggle
- **Métricas de Evaluación**: Precision, Recall, F1-Score, ROC-AUC
- **Interpretabilidad**: Utilización de SHAP para explicar las predicciones del modelo

## 🛠️ Stack Tecnológico

- **Python**: Lenguaje principal
- **Pandas**: Manipulación y análisis de datos
- **Scikit-learn**: Algoritmos de ML y preprocesamiento
- **XGBoost**: Gradient Boosting optimizado
- **LightGBM**: Gradient Boosting eficiente
- **SHAP**: Explicabilidad e interpretabilidad de modelos
- **Matplotlib/Plotly**: Visualizaciones
- **Imbalanced-learn**: Técnicas de balanceo de datos (SMOTE)

## 🧮 Metodología

### 1. Análisis Exploratorio de Datos (EDA)
- Análisis de la distribución de clases (fraude vs no fraude)
- Identificación de patrones y correlaciones
- Detección de valores atípicos y faltantes

### 2. Preprocesamiento de Datos
- **Balanceo de Clases**: 
  - SMOTE (Synthetic Minority Oversampling Technique)
  - Undersampling de la clase mayoritaria
- **Normalización/Estandarización** de features
- **División de datos** (train/validation/test)

### 3. Modelado
- **Logistic Regression**: Modelo baseline
- **Random Forest**: Ensemble de árboles
- **XGBoost**: Gradient Boosting optimizado
- **LightGBM**: Gradient Boosting eficiente

### 4. Evaluación
- **Métricas apropiadas para datos desbalanceados**:
  - Precision: TP / (TP + FP)
  - Recall: TP / (TP + FN)
  - F1-Score: Media armónica de Precision y Recall
  - ROC-AUC: Área bajo la curva ROC
- **Matriz de Confusión**
- **Análisis de curvas ROC y Precision-Recall**

### 5. Interpretabilidad
- **SHAP Values**: Explicación de predicciones individuales
- **Feature Importance**: Variables más importantes para la detección
- **Análisis de patrones de fraude**

## 📁 Estructura del Proyecto

```
├── README.md                # Documentación principal
├── requirements.txt         # Dependencias (pip)
├── environment.yml          # Entorno Conda (opcional)
├── config/                  # Configuraciones (YAML/JSON)
│   └── config.yaml
├── src/                     # Código fuente (actualmente vacío)
│   ├── data/                # Extracción / carga / validaciones
│   ├── features/            # Feature engineering / escalado
│   ├── models/              # Entrenamiento / evaluación / serving
│   ├── utils/               # Utilidades y helpers
│   └── main.py              # Punto de entrada (si aplica)
├── notebooks/               # Exploración y prototipos (desarrollo principal)
├── tests/                   # Pruebas unitarias e integración
├── data/                    # Datos (respetar .gitignore)
│   ├── raw/                 # Datos brutos
│   ├── processed/           # Datos procesados
│   └── external/            # Fuentes externas
├── models/                  # Modelos entrenados / artefactos
├── results/                 # Resultados, métricas, gráficos
├── logs/                    # Logs y tracking de ejecuciones
└── docs/                    # Documentación adicional
```

## 🚀 Guía de Inicio Rápido

### 1. Instalación de Dependencias

```bash
# Opción 1: Con pip
pip install -r requirements.txt

# Opción 2: Con conda
conda env create -f environment.yml
conda activate fraud-detector
```

### 2. Descarga de Datos

1. Descargar el dataset "Credit Card Fraud Detection" desde [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud)
2. Colocar el archivo `creditcard.csv` en la carpeta `data/raw/`

### 3. Ejecución del Análisis

El desarrollo principal se encuentra en los notebooks de Jupyter en la carpeta `notebooks/`:

1. **01_EDA.ipynb**: Análisis Exploratorio de Datos
2. **02_Data_Preprocessing.ipynb**: Preprocesamiento y balanceo de datos
3. **03_Model_Training.ipynb**: Entrenamiento de modelos
4. **04_Model_Evaluation.ipynb**: Evaluación y comparación de modelos
5. **05_Model_Interpretability.ipynb**: Análisis de interpretabilidad con SHAP

## 📊 Resultados Esperados

- **Precision alta**: Minimizar falsos positivos (transacciones legítimas marcadas como fraude)
- **Recall alto**: Minimizar falsos negativos (transacciones fraudulentas no detectadas)
- **F1-Score balanceado**: Equilibrio entre precision y recall
- **ROC-AUC > 0.95**: Excelente capacidad discriminativa
- **Interpretabilidad**: Identificación clara de variables que indican fraude

## 🔍 Características del Dataset

- **284,807 transacciones** con tarjeta de crédito
- **492 casos de fraude** (0.172% - altamente desbalanceado)
- **30 variables** (28 features PCA + Time + Amount + Class)
- **Anonimización**: Features principales son resultado de PCA por privacidad

## ⚠️ Consideraciones Importantes

1. **Desbalance de Clases**: Solo 0.172% de las transacciones son fraudulentas
2. **Costo de Errores**: Los falsos negativos pueden ser más costosos que los falsos positivos
3. **Privacidad**: Las features están anonimizadas por seguridad
4. **Tiempo Real**: El modelo debe ser eficiente para deployment en producción

## 📈 Métricas de Negocio

- **Reducción de pérdidas** por fraude no detectado
- **Mejora en la experiencia del cliente** (menos falsos positivos)
- **Tiempo de respuesta** del modelo en producción
- **Interpretabilidad** para cumplimiento regulatorio

## 🤝 Contribuciones

Este proyecto está diseñado como un portafolio personal de Data Science. Las contribuciones y mejoras son bienvenidas.

## 📄 Licencia

MIT License - Ver archivo LICENSE para más detalles.

## 📧 Contacto

**Desarrollador**: Cristóbal Pérez P.  
**Email**: cristobal.perez.p99@gmail.com  
**LinkedIn**: [Cristóbal Pérez P.](https://www.linkedin.com/in/cristobal-perez-palma/)
