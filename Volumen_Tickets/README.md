# Forecasting de Volumen de Tickets de Soporte y Planificación de Agentes (SLA)

Este proyecto aplica modelos de forecasting para anticipar el volumen diario de tickets de soporte y convertir esa previsión en el número óptimo de agentes requeridos para cumplir un SLA objetivo mediante cálculos basados en la fórmula de Erlang C.

## Objetivo

- Predecir la cantidad diaria de tickets/incidencias entrantes en un centro de soporte.
- Incorporar efectos de **estacionalidad semanal**, **festivos** y **eventos especiales** (campañas, lanzamientos).
- Calcular automáticamente el **número de agentes necesarios** para cumplir un SLA definido (ej. 80% de respuestas en <60s).
- Visualizar el plan de capacidad requerida de forma clara y ejecutiva.

## Técnicas aplicadas

- Simulación realista de datos de tickets diarios (tendencia, estacionalidad, eventos).
- Modelo de forecasting: **Prophet** con regresores adicionales.
- Validación temporal y métricas: MAE, RMSE, MAPE.
- Cálculo de agentes requeridos mediante **Erlang C** y probabilidad de servicio.
- Visualizaciones: forecast vs real, descomposición de componentes, curva de agentes requeridos.

## Tecnologías utilizadas

- Python
- Prophet
- NumPy, Pandas, Matplotlib
- Fórmulas de Erlang C implementadas en Python

## Ejemplo de resultados

MAE : 3.12  
RMSE : 4.25  
MAPE : 4.10%  
Agentes requeridos (media próxima semana): 18

### Visualizaciones destacadas

- Forecast vs real en ventana de test.
- Componentes del modelo (tendencia, semanal, regresores).
- Gráfico de capacidad requerida (agentes/día).
- Evolución prevista de tickets con intervalos de confianza.

## Casos de uso reales

- **Customer Experience**: planificación de personal en centros de soporte.
- **Operaciones**: prevención de incumplimiento de SLA por falta de capacidad.
- **Producto/Marketing**: evaluar el impacto de lanzamientos y campañas en la carga de soporte.

## ¿Cómo usar?

1. Ejecuta el notebook en Google Colab o Jupyter.  
2. Sustituye los datos simulados por tus tickets históricos.  
3. Ajusta parámetros: AHT, SLA objetivo, horas/día, festivos y eventos.  
4. Exporta las tablas y gráficos a tu dashboard o planificación interna.

## Valor añadido

- **Planificación proactiva** para mantener SLA.  
- **Modelo interpretable** y adaptable a cada negocio.  
- Integrable con herramientas de BI para seguimiento continuo.
