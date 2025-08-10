# Forecasting de Demanda Intermitente por SKU + Punto de Pedido y Stock de Seguridad

Este proyecto implementa modelos específicos para demanda intermitente (Croston, SBA, TSB) para predecir la demanda futura por SKU y calcular automáticamente el Punto de Pedido (ROP) y el Stock de Seguridad necesarios para mantener un nivel de servicio objetivo.

## Objetivo

- Predecir la demanda futura de SKUs con ventas esporádicas.
- Seleccionar automáticamente el mejor método de forecasting para cada SKU según métricas de error.
- Calcular el **Punto de Pedido (ROP)** y el **Stock de Seguridad (SS)** para un nivel de servicio objetivo (ej. 95%).
- Opcionalmente, calcular la **Cantidad Económica de Pedido (EOQ)**.

## Técnicas aplicadas

- Simulación de demanda intermitente por SKU (con picos por campañas/eventos).
- Modelos de forecasting: **Croston**, **SBA** (Syntetos–Boylan Adjustment) y **TSB** (Teunter–Syntetos–Babai).
- Selección automática de modelo según sMAPE.
- Cálculo de ROP y SS con lead time definido y nivel de servicio objetivo.
- Visualizaciones: series históricas, pronósticos, ROP y SS por SKU.

## Tecnologías utilizadas

- Python
- NumPy, Pandas, Matplotlib

## Ejemplo de resultados

 Mejor método por SKU: Croston / SBA / TSB según caso  
 ROP medio: 45 unidades  
 Stock de Seguridad medio: 12 unidades

### Visualizaciones destacadas

- Serie histórica de demanda (últimos 120 días).
- Pronóstico a 30 días por SKU con referencia de ROP.
- Comparativa de ROP y SS entre SKUs.
- Métricas de error por método y SKU.

## Casos de uso reales

- **Inventarios de repuestos** (MRO, automoción, maquinaria).
- **E-commerce long-tail**: productos de rotación lenta.
- **Logística**: planificación de aprovisionamiento con demanda irregular.

## ¿Cómo usar?

1. Ejecuta el notebook en Google Colab o Jupyter.  
2. Sustituye los datos simulados por tu histórico de ventas por SKU.  
3. Ajusta parámetros: lead time, nivel de servicio, costes.  
4. Exporta los resultados para integrarlos en tu ERP o dashboard.

## Valor añadido

- **Modelos específicos** para un problema donde los modelos estándar fallan.  
- **Optimización de inventario** reduciendo faltantes y exceso de stock.  
- **Decisiones basadas en datos** con indicadores claros para reabastecimiento.

