# Forecasting + Detección de Anomalías Basado en Residuales

Este proyecto aplica modelos de forecasting con Prophet para prever la evolución de una métrica clave del negocio y detectar desviaciones inesperadas a través del análisis de errores residuales.

## Objetivo

- Predecir el comportamiento normal de un KPI (ventas, ingresos, usuarios activos, etc.)
- Detectar automáticamente **anomalías** o desviaciones inusuales
- Visualizar alertas de forma clara y profesional

## Técnicas aplicadas

- Simulación de datos tipo KPI diario (tendencia + estacionalidad + ruido)
- Modelo de forecasting: **Prophet**
- Cálculo de errores residuales y umbrales automáticos
- Identificación de **outliers** basada en estadística (2σ rule)
- Visualizaciones avanzadas: evolución del error, histogramas, patrones semanales

## Tecnologías utilizadas

- Python
- Prophet
- NumPy, Pandas, Matplotlib
- Scikit-learn

## Ejemplo de resultados

📌 MAE : 2.91
📌 RMSE : 3.44
📌 MAPE : 2.83%
🚨 Anomalías detectadas: 14 días


### Visualizaciones destacadas

- Forecast vs real + puntos de anomalía
- Distribución de errores
- Análisis temporal de desviaciones
- Gráfico de anomalías por día de la semana

## Casos de uso reales

- **Dirección financiera**: seguimiento de ingresos vs objetivo
- **Operaciones**: detección de caídas o picos de actividad
- **Ecommerce**: alertas de cambios drásticos en tráfico o conversiones
- **Producto**: monitoreo de DAUs/MAUs con alertas tempranas



## ¿Cómo usar?

1. Ejecuta el notebook en Colab o Jupyter
2. Sustituye los datos simulados por tus propios KPIs
3. Ajusta el modelo para adaptarlo al contexto (diario, horario, semanal)
4. Exporta los resultados a dashboards o sistemas de alerta

## Valor añadido

 **Seguimiento automatizado** de KPIs clave  
 **Alertas proactivas** para tomar decisiones a tiempo  
 **Modelo interpretable y explicable** (no caja negra)  
 Listo para dashboards empresariales (Power BI, Looker, etc.)

