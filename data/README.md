# Data Directory

Esta carpeta contiene todos los datos utilizados en el proyecto de detección de fraude.

## Estructura

- **`raw/`**: Datos originales sin procesar
  - Aquí debe colocarse el archivo `creditcard.csv` descargado de Kaggle
  
- **`processed/`**: Datos procesados y preparados para el modelado
  - Datos después del preprocesamiento, balanceo y feature engineering
  
- **`external/`**: Fuentes de datos externas
  - Datos adicionales que puedan complementar el análisis

## Importante

- **NO subir datos al repositorio**: Asegúrate de que esta carpeta esté en `.gitignore`
- **Privacidad**: Los datos contienen información sensible de transacciones bancarias
- **Tamaño**: El dataset original tiene ~150MB

## Descarga de Datos

1. Ir a [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/mlg-ulb/creditcardfraud)
2. Descargar `creditcard.csv`
3. Colocar en la carpeta `data/raw/`
