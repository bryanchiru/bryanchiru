# 📊 Análisis de Datos y Modelo de Clasificación: Patrones de Sueño y Estilos de Vida

## Introducción
Este proyecto realiza un Análisis Exploratorio de Datos (EDA) exhaustivo sobre el *Sleep Health and Lifestyle Dataset* de Kaggle, seguido por la implementación de un modelo de Machine Learning para predecir el nivel de estrés.

---

## 🛠️ Metodología y Preprocesamiento (Fase 1)

1.  **Limpieza y Transformación:** Se eliminaron duplicados y se separó `Blood Pressure` en `Systolic_BP` y `Diastolic_BP`.
2.  **Filtrado de Outliers:** Se aplicó el método del **Rango Intercuartílico (IQR)** para aumentar la robustez de los datos.
3.  **Creación de Variable Objetivo:** Se creó la variable binaria **`Nivel_Estres_Binario`** (ESTRESADO vs. ESTRES MODERADO).
4.  **Selección de Variables:** Se eliminó la columna **`Sleep Duration`** debido a su altísima multicolinealidad con `Quality of Sleep` (Correlación: 0.89).

### Conclusiones Clave del EDA

* Existe una **fuerte correlación negativa** entre el nivel de estrés y la **Calidad del Sueño**.
* Ocupaciones como **`Sales Representative`** y **`Software Engineer`** mostraron una mayor proporción de individuos en la categoría **ESTRESADO**.

---

## 🚀 Resultados del Modelo de Clasificación (Fase 2)

Se implementó un modelo **Random Forest Classifier** para predecir el `Nivel_Estres_Binario` a partir de las variables de estilo de vida.

### Rendimiento General

| Métrica | Valor | Interpretación |
| :--- | :--- | :--- |
| **Precisión General (Accuracy)** | **0.97** | El modelo clasifica correctamente el 97% de los casos en el conjunto de prueba. |
| **Recall (Clase 'ESTRESADO')** | **1.00** | El modelo detectó el 100% de los casos reales de estrés alto, demostrando gran fiabilidad. |
| **F1-Score (Promedio Ponderado)** | **0.97** | Rendimiento excelente y equilibrado en ambas clases. |

### Conclusión Final del Proyecto

El modelo valida la hipótesis del análisis: la variable **`Quality of Sleep`** (Calidad del Sueño) resultó ser el **predictor más importante** para la clasificación del nivel de estrés, seguido por indicadores fisiológicos como la Frecuencia Cardíaca. El *dataset* preprocesado fue altamente efectivo para la predicción.
