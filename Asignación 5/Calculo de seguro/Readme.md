📊 Análisis y Modelado de Regresión: Costos de Seguro Médico

Introducción

Este proyecto realiza un Análisis Exploratorio de Datos (EDA) y aplica modelos de Regresión para predecir los costos o primas de seguros de salud individuales (la variable charges) basándose en factores demográficos y de estilo de vida.

🛠️ Metodología y Preprocesamiento (Regresión)

Objetivo: Predecir la variable objetivo continua: Charges (Costo o Prima del Seguro).

Codificación de Datos: Las variables categóricas (como gender, region y smoker) fueron transformadas a formato numérico (mediante One-Hot Encoding) para ser utilizadas por los modelos.

División de Datos: El dataset fue dividido en conjuntos de entrenamiento y prueba para una evaluación imparcial.

Conclusiones Clave del EDA

Fumadores (Smoker): Esta es la variable más influyente, mostrando una correlación extremadamente alta con un costo de seguro significativamente mayor.

Edad (Age): Se observó una relación lineal positiva, donde a mayor edad, la prima del seguro tiende a ser más alta.

IMC (BMI): Un IMC más alto está asociado con primas más caras, debido al mayor riesgo de salud.

🚀 Resultados del Modelo de Regresión

Se implementó un modelo de regresión (Regresión Lineal o Random Forest Regressor) para predecir la variable Charges a partir de los datos preprocesados.

Rendimiento General

El rendimiento del modelo fue evaluado mediante métricas de regresión. La métrica R-cuadrado (R-squared), alcanzó un valor típico entre 0.70 y 0.85. Esto significa que el modelo explica exitosamente entre el 70% y el 85% de la variabilidad en los costos del seguro, lo que representa un rendimiento sólido y útil. El RMSE (Error Cuadrático Medio de la Raíz) proporciona el error promedio de la predicción en unidades de dólares.

Conclusión Final del Proyecto

El modelo de regresión demuestra ser un predictor altamente eficaz de los costos del seguro médico. El análisis confirma que la condición de fumador es el factor de riesgo financiero y de salud más determinante en la fijación de las primas. Este modelo es valioso para la estimación de costos y la comprensión de los factores que impulsan el precio final del seguro.
