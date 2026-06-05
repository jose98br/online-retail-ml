# Predicción de Recompra de Clientes — Online Retail II

Proyecto de Machine Learning para identificar qué clientes de una tienda online del Reino Unido van a volver a comprar, permitiendo aplicar acciones de fidelización o retención personalizadas.

## Resultado

**AUC = 0.81** con Gradient Boosting optimizado mediante RandomizedSearchCV.

## Dataset

**Online Retail II** — 1,067,371 transacciones entre diciembre 2009 y diciembre 2011.

> El archivo de datos (`online_retail_II.xlsx`) no está incluido por su tamaño. Puede descargarse desde [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii).

## Estructura del proyecto

```
├── online_retail_II_EDA-basic.ipynb   # Notebook completo: EDA, limpieza, modelo
├── presentacion.html                  # Presentación interactiva (abrir en navegador)
└── README.md
```

## Metodología

1. **EDA** — Análisis exploratorio: estacionalidad, Pareto, distribuciones
2. **Limpieza** — Cancelaciones, registros sin cliente, precios/cantidades negativos
3. **Feature Engineering** — Variables RFM por cliente con fecha de corte
4. **Modelado** — Comparativa de 8 algoritmos evaluados por AUC
5. **Optimización** — RandomizedSearchCV sobre Gradient Boosting
6. **Explicabilidad** — Feature importance: días sin comprar (57%), nº compras (18%), gasto total (14%)

## Variables más importantes

| Variable | Importancia |
|---|---|
| Días sin comprar (Recency) | 57% |
| Nº de compras (Frequency) | 18% |
| Gasto total (Monetary) | 14% |
| Variedad de productos | 6% |

## Tecnologías

Python 3.12 · pandas · scikit-learn · xgboost · lightgbm · matplotlib · seaborn
