# CHANGELOG

## Estrategia de versionamiento

El proyecto utilizará una estrategia simple basada en versiones mayores.

Para esta entrega únicamente se contempla una versión inicial:

Formato:

Version X.Y

Donde:

X = cambios importantes del proyecto

Y = ajustes menores o correcciones



# Version 1.0


Fecha:

2026-06-30



## Cambios realizados


### Datos

- Integración Titanic Dataset de Kaggle
- Creación carpeta datos_ini
- Generación dataset limpio en datos_limp


### Preparación de datos

- Eliminación de columnas sin valor predictivo
- Tratamiento de valores faltantes
- Conversión de variables categóricas


### Modelo

- Implementación Random Forest Classifier
- División de datos:
  - 80% entrenamiento
  - 20% prueba


### Evaluación

Se agregaron métricas:

- Accuracy
- Recall
- F1-score
- Latencia de predicción


### MLflow

- Registro de métricas
- Registro del modelo entrenado
