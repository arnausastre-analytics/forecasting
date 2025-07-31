# Forecasting de Demanda Multivariado con XGBoost

Este proyecto implementa un sistema completo de forecasting de demanda para múltiples productos, utilizando técnicas avanzadas de machine learning con **XGBoost** y un fuerte enfoque en el análisis de series temporales multivariadas.

## Características principales

 Simulación realista de ventas para múltiples productos  
 Ingeniería de features temporales: lags, rolling windows, calendario  
 Entrenamiento con XGBoost  
 Métricas de evaluación (RMSE, MAE)  
 Análisis de errores por producto  
 Visualizaciones interpretables para negocio

## Tecnologías utilizadas

- `Python`
- `XGBoost`
- `Pandas`, `NumPy`
- `Matplotlib`
- `Scikit-learn`

## Arquitectura del modelo

Simulación de entorno multiproducto estilo retail

Creación de variables predictoras:

Lags: t-1, t-7

Estadísticas móviles (media, std)

Variables calendario: día de la semana, mes, festivos

Entrenamiento de modelo XGBoost

Evaluación global y por producto

Visualización de predicciones y explicaciones

## Resultados (ejemplo)

📊 RMSE global: 12.95
📊 MAE global : 10.21

Errores por producto:
Producto RMSE MAE
Product_C 12.95 10.21


Visualizaciones:
-  Predicción vs Real
-  Importancia de variables
-  Error por producto

## Aplicaciones reales

- Retail: predicción de demanda por SKU
- Logística: planificación de envíos y almacenaje
- Producción: planificación de fabricación
- E-commerce: reabastecimiento inteligente

## ¿Por qué XGBoost?

- No necesita series perfectamente regulares
- Permite manejar múltiples variables de entrada
- Rápido, interpretable y potente para producción
- Ideal cuando hay múltiples productos, señales externas y datos tabulados

## Cómo ejecutar

1. Clona el repositorio
2. Abre el notebook en Google Colab o Jupyter
3. Ejecuta todas las celdas
4. Reemplaza los datos simulados por tus datos reales si deseas

