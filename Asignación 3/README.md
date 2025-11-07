# 📊 Análisis de Datos: Patrones de Sueño y Estilos de Vida

## Introducción
Este proyecto realiza un Análisis Exploratorio de Datos (EDA) exhaustivo sobre el *Sleep Health and Lifestyle Dataset* de Kaggle. El objetivo principal fue preprocesar y explorar la relación entre diversos factores de salud/estilo de vida y el nivel de estrés, preparando un conjunto de datos limpio y filtrado para un futuro modelo de clasificación de Machine Learning.

---

## 🛠️ Metodología y Preprocesamiento

1.  **Limpieza y Transformación:**
    * Se identificaron y eliminaron filas duplicadas.
    * La columna `Blood Pressure` fue descompuesta en dos variables numéricas: **`Systolic_BP`** y **`Diastolic_BP`**.
    * Se unificaron etiquetas en `BMI Category` (`Normal Weight` unificado a `Normal`).
2.  **Filtrado de Outliers:** Se aplicó el método del **Rango Intercuartílico (IQR)** en las variables numéricas para eliminar valores extremos, lo que mejora la robustez del modelo de clasificación.
3.  **Creación de Variable Objetivo:** La variable `Stress Level` (1-10) se transformó en la variable binaria **`Nivel_Estres_Binario`**:
    * **ESTRESADO:** Nivel de Estrés ≥ 7
    * **ESTRES MODERADO:** Nivel de Estrés entre 3 y 6
4.  **Selección de Variables (Correlación):**
    * La variable original `Stress Level` fue eliminada.
    * La columna **`Sleep Duration`** fue eliminada debido a su altísima correlación (0.89) con `Quality of Sleep` (multicolinealidad). Se mantuvo `Quality of Sleep` por considerarse una métrica más completa del bienestar percibido.

---

## 📈 Conclusiones Clave del Análisis (EDA)

* **Relación Inversa Fuerte:** Se confirmó una **fuerte relación inversa** entre la **Calidad del Sueño** y el **Nivel de Estrés**. Las personas clasificadas como 'ESTRESADO' reportan consistentemente una calidad de sueño más baja.
* **Factores Laborales:** Las ocupaciones como **`Sales Representative`** y **`Software Engineer`** mostraron la mayor proporción de individuos en la categoría **ESTRESADO**.
* **Preparación Final:** El *dataset* final (con variables categóricas codificadas) fue dividido en **`train.csv`** y **`test.csv`** (80/20), aplicando **estratificación** sobre la variable objetivo para asegurar que la proporción de estrés se mantenga en ambos conjuntos.

---

## 📁 Archivos de Datos Generados

El repositorio contiene los siguientes archivos listos para la fase de modelado de clasificación:
* `Sleep_health_and_lifestyle_dataset.csv`: Datos originales.
* `analisis_sueno.ipynb`: Código Python completo del análisis.
* **`train.csv`**: Conjunto de datos de entrenamiento limpio y estratificado.
* **`test.csv`**: Conjunto de datos de prueba limpio y estratificado.
