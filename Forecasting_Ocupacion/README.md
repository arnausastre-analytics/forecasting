# Forecasting de Ocupación con Deep Learning (LSTM)

Este proyecto predice la ocupación diaria utilizando modelos de deep learning (LSTM) y detecta automáticamente días con alta demanda. Ideal para negocios donde anticipar la capacidad es clave: **hoteles, gimnasios, restaurantes, aerolíneas, coworkings**, etc.

## Objetivo

Predecir ocupación diaria a partir del histórico, con detección automática de picos (alta demanda) que pueden implicar:

- Refuerzo de personal
- Subida de precios (pricing dinámico)
- Activación de campañas

## Técnicas utilizadas

- Simulación de datos realistas: tendencia, estacionalidad semanal y mensual, ruido
- Modelo secuencial **LSTM (Long Short-Term Memory)**
- Normalización con `MinMaxScaler`
- Forecast de ocupación diaria
- Detección de **anomalías** por percentil (> 95%)
- Métricas: RMSE, MAE, MAPE
- Visualizaciones clave:
  - Ocupación real vs predicha
  - Errores residuales
  - Dispersión de predicciones
  - Promedio por día de la semana (heatmap)

## Tecnologías

- Python 3
- TensorFlow / Keras
- Scikit-learn
- Pandas, NumPy
- Matplotlib

## Resultados

 RMSE: 5.93
 MAE : 4.83
 MAPE: 9.71%
 36 días con ocupación prevista en el top 5%

## Casos de uso reales

- Previsión de reservas de hotel por día
- Anticipación de demanda de clases en gimnasios
- Predicción de ocupación por vuelo en aerolíneas low-cost
- Gestión de turnos en restaurantes en días de alta afluencia

## Cómo usar

1. Ejecuta el notebook en Google Colab o Jupyter
2. Sustituye los datos simulados por tus datos reales de ocupación
3. Ajusta el modelo si necesitas multivariado (ej: clima, eventos)
4. Usa las alertas de alta demanda para planificación o pricing

## Valor comercial

 **Anticipación operativa**: asignación de personal eficiente  
 **Revenue optimization**: detección de oportunidades para precios dinámicos  
 **Visión accionable**: dashboards e insights prácticos para el negocio
