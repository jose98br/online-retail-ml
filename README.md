# Predicción de Recompra de Clientes — Online Retail II

Proyecto de Machine Learning para identificar clientes con alta probabilidad de volver a comprar en una empresa de retail online del Reino Unido.

## Objetivo

Construir un modelo de clasificación que prediga si un cliente realizará una nueva compra, permitiendo aplicar acciones de fidelización o retención según el resultado.

## Dataset

**Online Retail II** — 1,067,371 transacciones entre diciembre 2009 y diciembre 2011.

> El archivo de datos (`online_retail_II.xlsx`) no está incluido en el repositorio por su tamaño. Puede descargarse desde [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii).

## Estructura del proyecto

```
├── online_retail_II_EDA-basic.ipynb   # EDA y modelo ML completo
└── README.md
```

## Metodología

1. **EDA** — Exploración y calidad de datos
2. **Limpieza** — Cancelaciones, nulos y outliers
3. **Feature Engineering** — Variables RFM (Recency, Frequency, Monetary) por cliente
4. **Modelado** — Regresión logística (baseline) + XGBoost
5. **Evaluación** — AUC + feature importance (SHAP)

## Resultados

*(Se completará al finalizar el modelo)*

## Tecnologías

- Python 3.12
- pandas, numpy, scikit-learn, xgboost, lightgbm, shap, matplotlib, seaborn
