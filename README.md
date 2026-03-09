# Telecom X - Predicción de Cancelación de Clientes (Churn)

## Descripción del proyecto

En este proyecto se desarrolla un modelo de **Machine Learning** para predecir la cancelación de clientes (*Churn*) en la empresa Telecom X.

La cancelación de clientes representa un problema importante para las empresas de telecomunicaciones, ya que adquirir nuevos clientes suele ser más costoso que retener a los existentes. Por esta razón, identificar con anticipación qué clientes tienen mayor probabilidad de cancelar el servicio permite implementar estrategias de retención más efectivas.

Este proyecto forma parte del desafío **Telecom X – Parte 2**, enfocado en la construcción y evaluación de modelos predictivos.

---

## Objetivos

- Preparar los datos para el modelado de Machine Learning.
- Analizar las relaciones entre variables y la cancelación de clientes.
- Entrenar diferentes modelos de clasificación.
- Evaluar el desempeño de los modelos mediante métricas.
- Identificar los factores que influyen en la cancelación.
- Proponer estrategias de retención basadas en los resultados.

---

## Dataset

El dataset utilizado corresponde a clientes de una empresa de telecomunicaciones e incluye información como:

- Datos demográficos de los clientes
- Tipo de contrato
- Servicios contratados
- Métodos de pago
- Cargos mensuales y totales
- Tiempo de permanencia en la empresa
- Estado de cancelación (*Churn*)

La variable objetivo del modelo es **Churn**, que indica si un cliente canceló o no el servicio.

---

## Proceso de análisis

El flujo de trabajo del proyecto incluye las siguientes etapas:

### 1. Preprocesamiento de datos

- Eliminación de columnas irrelevantes
- Codificación de variables categóricas mediante **One-Hot Encoding**
- Análisis del balance de clases
- Estandarización de variables para modelos sensibles a la escala

### 2. Análisis exploratorio

Se analizaron las relaciones entre las variables y la cancelación de clientes mediante:

- Matriz de correlación
- Visualización de variables clave
- Comparación de comportamientos entre clientes activos y cancelados

---

## Modelos de Machine Learning

Se entrenaron dos modelos de clasificación:

### Regresión Logística

Modelo lineal utilizado para estimar la probabilidad de cancelación de los clientes.

Ventajas:
- Fácil interpretación
- Permite analizar la influencia de cada variable

### Random Forest

Modelo basado en múltiples árboles de decisión que mejora la capacidad de capturar relaciones complejas entre variables.

Ventajas:
- Buen desempeño en problemas de clasificación
- Permite calcular la importancia de las variables

---

## Evaluación de modelos

Los modelos fueron evaluados utilizando las siguientes métricas:

- Accuracy
- Precision
- Recall
- F1-score
- Matriz de confusión

Estas métricas permiten medir la capacidad del modelo para identificar correctamente a los clientes que tienen mayor riesgo de cancelar el servicio.

---

## Resultados principales

El análisis permitió identificar varios factores asociados a la cancelación de clientes.

Entre los más relevantes se encuentran:

- **Tenure (antigüedad del cliente)**: los clientes con menor tiempo en la empresa presentan mayor probabilidad de cancelar.
- **Tipo de contrato**: los contratos mensuales tienen mayor tasa de cancelación que los contratos de largo plazo.
- **MonthlyCharges**: cargos mensuales más altos están asociados con mayor churn.
- **InternetService (Fiber optic)**: algunos clientes con este servicio presentan mayor tasa de cancelación.
- **PaymentMethod (Electronic check)**: método de pago asociado con mayores niveles de churn.

---

## Estrategias de retención sugeridas

A partir de los resultados obtenidos, se proponen algunas acciones para reducir la cancelación de clientes:

- Ofrecer incentivos para migrar a **contratos de mayor duración**.
- Implementar **programas de fidelización para nuevos clientes**.
- Revisar la estructura de precios para clientes con **cargos mensuales elevados**.
- Promover servicios adicionales como **soporte técnico y seguridad en línea**.
- Analizar la experiencia de los clientes con **servicios de fibra óptica**.

---

## Tecnologías utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Estructura del proyecto

```
TelecomX-Churn-Prediction
│
├── TelecomX_LATAM_Challenge2.ipynb
├── README.md
└── telecom_churn_limpio.csv
```

---

## Conclusión

El uso de modelos de Machine Learning permite anticipar la cancelación de clientes y comprender los factores que influyen en esta decisión. Esto facilita el desarrollo de estrategias de retención más efectivas y contribuye a mejorar la satisfacción y fidelidad de los clientes.

El análisis demuestra que variables como la antigüedad del cliente, el tipo de contrato y los cargos mensuales son determinantes en la predicción del churn.
