# 🧠 Actividad 2.12: Redes Neuronales (MLP) y MLflow

**Asignatura:** IEI097 · Minería de Datos  
**Institución:** Instituto Profesional Santo Tomás - Sede Arica  
**Estudiante:** Benjamín Eduardo Naveas Molina  

## 📋 Descripción del Proyecto
Este repositorio contiene el desarrollo práctico del laboratorio de Redes Neuronales Artificiales. El objetivo principal es implementar y entrenar un **Perceptrón Multicapa (MLP)** para la clasificación de tumores (benigno vs. maligno) utilizando el concepto de observabilidad en Machine Learning.

Para garantizar la reproducibilidad y el seguimiento sistemático de cada entrenamiento, se integró **MLflow** a través de un túnel de `ngrok` directo desde Google Colab. 

### 🔬 Experimentos Realizados
Se registraron múltiples ejecuciones evaluando distintos escenarios:
- Impacto del escalado de variables (`StandardScaler`) en la convergencia del gradiente.
- Variación de arquitecturas (capas ocultas y neuronas).
- Cambio de funciones de activación (`ReLU` vs `Tanh`).
- Pruebas de variabilidad y replicación exacta aislando y fijando la semilla (`random_state`).

### 🗃️ Dataset Utilizado
* **Breast Cancer Wisconsin (Diagnostic) Data Set**
* Obtenido mediante la API de Kaggle (`kagglehub`). Se preprocesaron los datos para evitar fuga de datos (Data Leakage) estratificando la partición de prueba.

## 🛠️ Tecnologías y Herramientas
- **Entorno:** Google Colab (Python 3)
- **Machine Learning:** `scikit-learn` (MLPClassifier, StandardScaler, Pipeline)
- **Tracking & Observabilidad:** `mlflow`, `pyngrok`
- **Manipulación de Datos y Visualización:** `pandas`, `numpy`, `matplotlib`

## 📁 Estructura del Repositorio
- `IEI097_Lab2.12_MLP_MLflow.ipynb`: Cuaderno principal con el código fuente y las justificaciones teóricas.
- `runs.csv`: Exportación de la base de datos de MLflow con el registro de parámetros y métricas de todas las ejecuciones.
- `/evidencias`: Directorio que contiene las capturas de pantalla de la interfaz web de MLflow (Tabla de runs, gráficos de comparación y matriz de confusión).

## 🚀 Ejecución en Colab
Puedes revisar el código completo directamente en Google Colab haciendo clic en el siguiente enlace:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/139meTHiK9bGWyHkl_pTFiElLK9gAx66U?usp=sharing)

---
*Este proyecto fue desarrollado como parte de las evaluaciones formativas de la Unidad II de la asignatura Minería de Datos.*
