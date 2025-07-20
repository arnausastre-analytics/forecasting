# Forecasting Sales

## Introducción

El objetivo de este proyecto es construir un modelo de predicción de ventas utilizando datos históricos. Antes de plantear cualquier modelo predictivo, es necesario realizar un análisis descriptivo riguroso para entender la naturaleza de la serie temporal objeto de estudio. Esto permite identificar posibles patrones de tendencia, estacionalidad o variaciones en la varianza que podrían condicionar la elección del modelo.

## Metodología

En primer lugar, se realiza una representación gráfica de la serie temporal. Esta visualización inicial es fundamental para obtener una percepción global del comportamiento de los datos, identificar patrones temporales recurrentes y valorar la necesidad de aplicar transformaciones previas (como logaritmos, raíces cuadradas o diferenciaciones de primer y segundo orden). El análisis gráfico también permite detectar cambios estructurales o rupturas en la serie que podrían afectar a los modelos de forecasting.

Posteriormente, se lleva a cabo un análisis estadístico descriptivo que proporciona información sobre la media, dispersión y distribución de la serie, aspectos relevantes para entender las características generales de los datos.

A continuación, se evalúa la estacionariedad de la serie temporal mediante el test de Dickey-Fuller aumentado (ADF). La estacionariedad es un requisito fundamental para la aplicación de modelos clásicos como ARIMA o SARIMA, por lo que resulta imprescindible comprobar su cumplimiento antes de proceder.

En función del resultado del test ADF y de las características observadas en la visualización, se define la estrategia de modelado. En este proyecto, se opta por construir un modelo ARIMA o SARIMA según proceda, dado que estos modelos permiten capturar tanto componentes autorregresivos como de medias móviles, incluyendo la posibilidad de contemplar estacionalidad. En el entorno R, funciones como `auto.arima` facilitan la identificación automática de los parámetros óptimos; en Python, existen herramientas análogas como `auto_arima` del paquete `pmdarima`, que cumplen la misma función y permiten determinar de manera sistemática los valores de p, d y q más adecuados.

Finalmente, se estiman las predicciones futuras y se representan gráficamente junto a los datos históricos, permitiendo visualizar la capacidad predictiva del modelo y validar su adecuación.

## Herramientas utilizadas

- Python
- pandas
- matplotlib / seaborn
- statsmodels
- pmdarima (para selección automática de modelos)

## Estructura del proyecto

/sales-forecasting/

├── forecasting_sales.ipynb # Notebook con el desarrollo completo del análisis

├── dataset.csv # Dataset histórico de ventas utilizado

└── README.md # Este documento


## Conclusiones

Este proyecto constituye un ejemplo básico de forecasting de series temporales aplicado al contexto de ventas, pero la metodología expuesta es extrapolable a múltiples contextos donde existan datos temporales (demanda de productos, tráfico web, ocupación hotelera, entre otros). La aplicación rigurosa de un análisis previo antes de la modelización es esencial para garantizar la validez de las predicciones y asegurar que los supuestos estadísticos requeridos se cumplen.


