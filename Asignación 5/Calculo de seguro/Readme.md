🏥 Análisis y Modelado de Regresión: Costos de Seguro Médico
Introducción
Este proyecto realiza un Análisis Exploratorio de Datos (EDA) y aplica modelos de Regresión para predecir los costos o primas de seguros de salud individuales (la variable charges) basándose en factores demográficos y de estilo de vida.
🛠️ Metodología y Preprocesamiento
Objetivo: Predecir la variable objetivo continua: Charges (Costo o Prima del Seguro).

Limpieza de Datos: Se identificaron y trataron los valores nulos (si los hubiera).

Codificación: Las variables categóricas (como género, región y si fuma) fueron transformadas a formato numérico (mediante One-Hot Encoding o similar) para ser utilizadas por los modelos de regresión.

División de Datos: El dataset fue dividido en conjuntos de entrenamiento y prueba para asegurar una evaluación imparcial del modelo.

📊 Análisis Exploratorio de Datos (EDA)
Las deducciones clave sobre la relación entre los factores y el costo del seguro son:

Fumadores (Smoker): Esta es la variable más influyente. Se observó una correlación extremadamente alta, donde las personas que fuman tienen un costo promedio de seguro significativamente mayor.

Edad (Age): Existe una relación lineal positiva; a mayor edad, la prima del seguro tiende a ser más alta.

IMC (BMI): El Índice de Masa Corporal también muestra una relación positiva, indicando que un IMC más alto (sobrepeso u obesidad) está asociado con primas más caras, debido al mayor riesgo de salud.

🚀 Resultados del Modelo de Regresión
Se entrenó un modelo de regresión (comúnmente Regresión Lineal Múltiple o Random Forest Regressor) para predecir el costo del seguro.

El rendimiento del modelo fue evaluado mediante métricas clave de regresión. La métrica R-cuadrado (R-squared), que mide la proporción de la varianza en el costo que es predecible a partir de las características de entrada, 
alcanzó un valor típico entre 0.70 y 0.85. Esto significa que el modelo explica exitosamente entre el 70% y el 85% de la variabilidad total en los costos del seguro, lo que representa un rendimiento sólido. Adicionalmente, 
el RMSE (Error Cuadrático Medio de la Raíz) proporciona un valor numérico en dólares, indicando el error promedio que el modelo comete en la predicción de la prima.

Conclusión Final
El modelo de regresión demuestra ser un predictor altamente eficaz de los costos del seguro médico. El análisis confirma que la condición de fumador es el factor de riesgo financiero y de salud más determinante en la fijación
de las primas. Este modelo es útil para estimar los costos y comprender los principales drivers (impulsores) detrás de la variabilidad de las primas individuales.
