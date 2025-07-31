# Forecasting Financiero Mensual con Prophet y SARIMA

Este proyecto implementa un sistema completo de **predicción de ingresos mensuales** utilizando dos de los modelos más populares en series temporales: **Prophet** (Meta/Facebook) y **SARIMA** (Statsmodels).

## Objetivo

Predecir la evolución de KPIs financieros (ej. ingresos) de una empresa SaaS / fintech / ecommerce, incorporando efectos estacionales, tendencia y variabilidad realista.  
Esto permite a **CFOs, controllers y ejecutivos de negocio** planificar mejor sus decisiones.

## Técnicas utilizadas

- **Simulación realista de ingresos mensuales** con tendencia + estacionalidad + ruido
- **SARIMA** (Seasonal ARIMA): modelo clásico y robusto para series temporales
- **Prophet**: modelo flexible con estacionalidad y festivos
- Evaluación con métricas: `RMSE`, `MAE`
- Comparación visual SARIMA vs Prophet
- Análisis avanzado de errores residuales

## Tecnologías

- Python 3
- Prophet (`prophet`)
- SARIMAX (`statsmodels`)
- Numpy, Pandas
- Matplotlib, Seaborn
- Scikit-learn

## Resultados (ejemplo)

SARIMA → RMSE: 1483.89 | MAE: 1179.46
Prophet → RMSE: 1453.68 | MAE: 923.49


### Análisis avanzado de errores:
- Evolución de errores en el tiempo
- Distribución de errores → ¿normalidad o sesgo?
- Gráfica de dispersión: ¿subestima en ingresos altos?

## ¿Por qué es importante este análisis?

Apoya decisiones estratégicas de negocio  
Detecta posibles sesgos en el modelo (por ejemplo, subestimar ingresos altos)  
Aporta transparencia y confianza al cliente  

## Cómo usar este proyecto

1. Ejecuta el notebook en [Google Colab](https://colab.research.google.com/)
2. Reemplaza los datos simulados por tus datos reales
3. Analiza y ajusta los modelos según tus necesidades

## Casos de uso

- Forecasting para SaaS (MRR, ARR)
- Previsión de ventas ecommerce
- Predicción de KPIs financieros en startups o scaleups
- Reportes de dirección y planificación de recursos

