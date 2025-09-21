# AN-LISIS-Y-MODELO-PREDICTIVO-DE-CANCELACIONES-HOTEL.
Predicción de cancelaciones de reservas de hotel usando Random Forest y XGBoost. Incluye EDA, visualizaciones y generación automática de informe PDF..

# 🏨 Predicción de Cancelaciones en Reservas de Hotel

[![Python](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-ML-orange)](https://scikit-learn.org/stable/)
[![XGBoost](https://img.shields.io/badge/XGBoost-ML-brightgreen)](https://xgboost.readthedocs.io/)
[![ReportLab](https://img.shields.io/badge/reportlab-PDF-red)](https://www.reportlab.com/opensource/)

## 📖 Descripción
Este proyecto analiza un dataset realista de **reservas de hotel**, con información sobre:
- Clientes, fechas, duración de estancia
- Tipo de habitación, plan de comidas, segmento de mercado
- Cancelaciones previas, tiempo de anticipación
- Precio medio por noche y solicitudes especiales

El objetivo es:
1. Explorar y entender los datos (EDA).
2. Detectar patrones de comportamiento (cancelaciones, estacionalidad, clientes recurrentes).
3. Construir modelos predictivos para estimar la probabilidad de **cancelación de una reserva**.
4. Generar un **informe PDF con resultados, métricas y visualizaciones**.

---

## 🛠️ Tecnologías usadas
- **Python 3.9+**  
- `pandas`, `numpy`, `matplotlib`, `seaborn` → EDA y visualización
- `scikit-learn` → Modelado (Random Forest)
- `xgboost` → Modelado avanzado
- `reportlab` → Exportación a PDF
- `jupyter notebook` → Documentación y análisis exploratorio

---

## 📊 Resultados principales

- **EDA**:
  - La mayoría de reservas son hechas online y con habitación estándar.
  - La tasa de cancelación ronda el ~35%.
  - Clientes recurrentes cancelan mucho menos que los nuevos.
  - El *lead_time* (días de antelación) influye fuertemente en las cancelaciones.

- **Modelos**:  
  | Modelo             | Accuracy | Recall | F1-score | ROC-AUC |
  |--------------------|----------|--------|----------|---------|
  | Random Forest      | 0.88     | 0.75   | 0.80     | 0.93    |
  | XGBoost            | 0.89     | 0.80   | 0.83     | 0.95    |

📌 **Conclusión**:  
👉 XGBoost obtiene el mejor desempeño, siendo el modelo recomendado para predecir cancelaciones.
👉 Esto permitiría al hotel **anticipar cancelaciones**, optimizar la gestión de habitaciones y mejorar ingresos.

---



