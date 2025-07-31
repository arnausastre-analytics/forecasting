# Forecasting de Series Temporales con LSTM

Este proyecto aplica modelos de deep learning (LSTM) para predecir series temporales complejas con patrones no lineales. Ideal para datos como:

- Ventas históricas
- Consumo energético
- KPIs operativos

## Objetivo

Predecir la evolución futura de una serie temporal univariada (por ejemplo, ventas o demanda energética) utilizando redes neuronales recurrentes (LSTM), y comparar su rendimiento con técnicas clásicas.

## Técnicas empleadas

- Simulación de serie temporal realista (tendencia + estacionalidad + ruido)
- Preprocesamiento y normalización con `MinMaxScaler`
- Construcción de secuencias temporales para entrenamiento
- Red neuronal `LSTM` con Keras/TensorFlow
- Evaluación con RMSE, MAE y MAPE
- Análisis avanzado de errores:
  - Errores residuales
  - Distribución de errores
  - Dispersión: error vs valor real

## Tecnologías

- Python
- NumPy, Pandas, Scikit-learn
- TensorFlow / Keras
- Matplotlib

## Resultados (ejemplo)

📊 RMSE: 21.48
📊 MAE : 17.63
📌 MAPE: 3.82%

## Casos de uso reales

- Forecasting de ventas minoristas o ecommerce
- Predicción de consumo eléctrico o de gas
- Previsión de demanda logística o transporte
- Modelado de métricas operativas o financieras

## Cómo usar

1. Ejecuta el notebook en Google Colab o Jupyter
2. Cambia los datos simulados por tus datos reales
3. Ajusta el tamaño de ventana y parámetros de red
4. Exporta resultados o integra en dashboards

## ¿Por qué usar LSTM para forecasting?

 Capacidad de capturar **dependencias largas**  
 Excelente para datos **no lineales y ruidosos**  
 Demuestra alto nivel técnico en tu portfolio  
 Escalable a multivariado y multistep forecasting
