# Actividad5 - Titanic Random Forest

## Descripción
Proyecto de Machine Learning para predecir la supervivencia en el Titanic usando Random Forest.

## Flujo del proyecto
- Carga de dataset desde Kaggle
- Limpieza de datos (valores faltantes y variables irrelevantes)
- Transformación de variables categóricas
- División 80% entrenamiento / 20% prueba
- Entrenamiento del modelo Random Forest
- Evaluación del modelo

## Dataset
Titanic Dataset de Kaggle:
https://www.kaggle.com/competitions/titanic

## Estructura del repositorio
datos/
- datos_ini → dataset original
- datos_limp → dataset procesado

fuentes/
- entrena.ipynb → pipeline completo del modelo

## Métricas evaluadas
- Accuracy
- Recall
- F1-score
- Matriz de confusión
- Latencia de predicción

## Modelo utilizado
Random Forest Classifier (n_estimators=100, random_state=42)
