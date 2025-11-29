# 🍎 Proyecto Final: Análisis y Predicción de Objetivos Nutricionales
Este repositorio contiene el trabajo final del curso de Data Science. El objetivo principal fue analizar un conjunto de datos médicos y nutricionales para intentar predecir el **Objetivo Nutricional** de los pacientes (Pérdida de peso, Ganancia muscular, Mantenimiento) utilizando algoritmos de Machine Learning.

## 📋 Descripción del Proyecto

El proyecto se divide en varias etapas de análisis de datos, desde la limpieza inicial hasta la implementación de modelos predictivos. Se buscó responder a la pregunta: **¿Es posible determinar el objetivo nutricional de un paciente basándonos en sus datos demográficos y hábitos alimenticios?**

### Estructura del Repositorio
* `ProyectoFinalDSREYNOSO.ipynb`: Notebook principal con el código de entrenamiento, validación y conclusiones.
* `df_datos_medicos_nutricionales.xlsx`: Dataset utilizado (Base de datos).
* `README.md`: Este archivo.

## 🛠️ Tecnologías Utilizadas

El proyecto fue desarrollado en **Python** utilizando las siguientes librerías:

* **Pandas & NumPy:** Manipulación y limpieza de datos.
* **Matplotlib & Seaborn:** Visualización de datos (EDA).
* **Scikit-Learn:**
    * *Preprocessing:* LabelEncoder, StandardScaler, OneHotEncoding.
    * *Feature Selection:* SelectKBest (ANOVA).
    * *Model:* RandomForestClassifier.
    * *Metrics:* Confusion Matrix, Classification Report.

## ⚙️ Metodología

1.  **Preprocesamiento de Datos:**
    * Limpieza de nombres de columnas.
    * Codificación de variables categóricas (Encoding de 'Edad', 'Género', 'Tipo de Alimentación').
    * Escalado de variables numéricas.
2.  **Selección de Características (Feature Selection):**
    * Se utilizó el método `SelectKBest` para identificar las variables con mayor varianza respecto al objetivo.
3.  **Modelado:**
    * Algoritmo seleccionado: **Random Forest Classifier**.
    * División de datos: 80% Entrenamiento / 20% Prueba.
4.  **Validación:**
    * Cálculo de Accuracy y análisis de la Matriz de Confusión.

## 📊 Resultados y Conclusiones

Tras entrenar el modelo, se obtuvieron los siguientes resultados:

* **Accuracy (Exactitud):** ~33.5%
* **Análisis:** Dado que el problema cuenta con 3 clases balanceadas, una exactitud del 33% indica que el modelo está actuando de manera aleatoria (azar).

**Conclusión Final:**
El análisis exploratorio y los resultados del modelo de Machine Learning sugieren fuertemente que el dataset utilizado es **sintético** o carece de patrones biológicos reales. No existe una correlación estadística observable entre la ingesta de macronutrientes/hábitos reportados y el objetivo nutricional en esta base de datos específica.

---
*Proyecto realizado por Christian Reynoso - 2025*
