# 📊 Challenge 3 – Telecom X (Predicción de Evasión de Clientes)

## 🎯 Objetivo
Este proyecto corresponde a la **segunda parte del Challenge Telecom X** del programa de Data Science LATAM de Alura.  
El objetivo es construir **modelos predictivos de Machine Learning** que permitan a la empresa **anticipar la evasión de clientes (churn)**, identificar las variables más influyentes y proponer estrategias de retención.

---

## 🛠️ Flujo del proyecto

1. **Carga de datos**
   - Se utilizaron los datos ya tratados en el Challenge 2 (`TelecomX_clean.csv`).

2. **Preparación de datos**
   - Eliminación de columnas irrelevantes (ej. `customerID`).
   - Separación de la variable objetivo `Churn`.
   - División en conjuntos de entrenamiento y prueba (70% / 30%).
   - Transformación de variables:
     - Escalado de variables numéricas.
     - Codificación One-Hot de variables categóricas.
   - Manejo de valores nulos con imputación.

3. **Modelado**
   - **Regresión Logística** como modelo baseline.
   - **Random Forest Classifier** como modelo avanzado.
   - Evaluación mediante:
     - Accuracy
     - Precision
     - Recall
     - F1-score
     - Matriz de confusión
     - ROC AUC

4. **Análisis de importancia de variables**
   - Identificación de las características más relevantes para explicar la evasión.

---

## 📈 Resultados principales

- La **tasa general de churn** en el dataset es de aproximadamente **XX %**.
- El modelo de **Random Forest** obtuvo un desempeño superior con una ROC AUC de **YY %**.
- Principales variables asociadas a la evasión:
  - **Tipo de contrato** (los contratos mensuales muestran mayor riesgo de churn).
  - **Cargos mensuales** (los clientes con cargos más altos tienden a irse).
  - **Tenure (antigüedad)** (los clientes con poca permanencia son más propensos a darse de baja).
  - **Tipo de servicio de internet** (fibra óptica tiene mayor churn que DSL).

---

## 🚀 Instrucciones de ejecución

1. Clonar este repositorio:
   ```bash
   git clone https://github.com/tu-usuario/telecomx-churn-predict.git
   cd telecomx-churn-predict
