# GestionProyectosAI
Repositorio para Gestion de proyectos de IA
Revisé los enlaces proporcionados de Google Colab; sin embargo, los notebooks requieren acceso autenticado y no permiten visualizar directamente el código ni los resultados desde el enlace compartido en este entorno. ([Google Colab][1])

Para evitar inventar nombres de archivos, métricas o resultados que no estén confirmados, ajusté el README dejando **la estructura exacta alineada a tus tres notebooks de Google Colab**, utilizando los nombres de modelos que indicaste. Solo sería necesario sustituir los valores numéricos de resultados (Accuracy, Recall, F1 y latencia) si deseas mostrarlos explícitamente.

---

# Proyecto Machine Learning - Titanic Dataset Kaggle

## Descripción del proyecto

Este proyecto fue desarrollado como parte de la materia **Gestión de Proyectos de Inteligencia Artificial**, aplicando técnicas de aprendizaje automático (*Machine Learning*) para resolver un problema de clasificación utilizando el dataset **Titanic Dataset de Kaggle**.

El objetivo del proyecto es construir modelos predictivos capaces de determinar si un pasajero del Titanic sobrevivió o no al accidente, utilizando variables históricas disponibles en el dataset como:

* Clase del pasajero.
* Sexo.
* Edad.
* Tarifa pagada.
* Número de familiares a bordo.
* Puerto de embarque.
* Información adicional del pasajero.

Para resolver el problema se implementaron y compararon tres algoritmos de clasificación supervisada:

1. **Logistic Regression (Regresión Logística)**
2. **Decision Tree (Árbol de Decisión)**
3. **Random Forest (Bosque Aleatorio)**

Cada modelo fue desarrollado utilizando Python y ejecutado mediante Google Colab, aplicando un flujo completo de Machine Learning:

* Carga del dataset.
* Limpieza y preparación de datos.
* Transformación de variables categóricas.
* Separación de datos de entrenamiento y prueba.
* Entrenamiento del modelo.
* Predicción.
* Evaluación mediante métricas de desempeño.

La división utilizada para todos los modelos fue:

* **80% datos de entrenamiento**
* **20% datos de prueba**

Las métricas utilizadas para evaluar los modelos fueron:

* Accuracy.
* Matriz de confusión.
* Precision.
* Recall.
* F1-score.
* Tiempo de ejecución.
* Latencia de predicción.

---

# Entorno de ejecución

El proyecto fue desarrollado utilizando el siguiente ambiente:

**Plataforma:**

Google Colab

**Runtime utilizado:**

T4 GPU

**Lenguaje:**

Python 3

**Principales librerías utilizadas:**

* Pandas.
* NumPy.
* Scikit-learn.
* Matplotlib.
* Seaborn.

El ambiente T4 GPU permite utilizar una configuración compatible con proyectos de Inteligencia Artificial. Aunque los modelos implementados utilizan principalmente procesamiento en CPU mediante Scikit-learn, el entorno permite mantener una infraestructura preparada para modelos con mayor demanda computacional.

---

# Notebooks implementados

El proyecto contiene tres notebooks principales desarrollados en Google Colab:

## 1. Logistic Regression

Notebook:

```
Logistic Regression
```

Link:

[https://colab.research.google.com/drive/1UHhWxPbJwBK-YWkT6XLfHB5o_LG5XBf2?usp=sharing](https://colab.research.google.com/drive/1UHhWxPbJwBK-YWkT6XLfHB5o_LG5XBf2?usp=sharing)

Descripción:

Implementa un modelo de Regresión Logística como modelo base de clasificación binaria.

El flujo del notebook incluye:

* Lectura del archivo Titanic-Dataset.csv.
* Preparación de variables.
* División de datos 80/20.
* Entrenamiento del modelo Logistic Regression.
* Evaluación del desempeño.
* Cálculo de métricas:

  * Accuracy
  * Recall
  * F1-score
  * Latencia

---

## 2. Decision Tree

Notebook:

```
Decision Tree
```

Link:

[https://colab.research.google.com/drive/1w8NTKW-bTw6TPeYDQTl_X6T1-werL25t?usp=sharing](https://colab.research.google.com/drive/1w8NTKW-bTw6TPeYDQTl_X6T1-werL25t?usp=sharing)

Descripción:

Implementa un modelo basado en Árbol de Decisión.

Este modelo permite identificar reglas de decisión dentro de los datos del Titanic mediante una estructura jerárquica.

El notebook incluye:

* Preparación del dataset.
* Entrenamiento del árbol.
* Predicción sobre datos de prueba.
* Evaluación mediante:

  * Accuracy
  * Matriz de confusión
  * Recall
  * F1-score
  * Tiempo de ejecución

---

## 3. Random Forest

Notebook:

```
Random Forest
```

Link:

[https://colab.research.google.com/drive/1j96lCQ8rt8CywR18op4_PTh3isPRTF1C?usp=sharing](https://colab.research.google.com/drive/1j96lCQ8rt8CywR18op4_PTh3isPRTF1C?usp=sharing)

Descripción:

Implementa un modelo de Bosque Aleatorio basado en múltiples árboles de decisión.

Este algoritmo utiliza técnicas de aprendizaje conjunto (*ensemble learning*) para mejorar la capacidad predictiva y reducir problemas de sobreajuste.

El notebook incluye:

* Entrenamiento del modelo Random Forest.
* Generación de predicciones.
* Evaluación del modelo mediante:

  * Accuracy
  * Matriz de confusión
  * Recall
  * F1-score
  * Latencia de predicción

---

# Pasos de ejecución

## 1. Descargar el repositorio

Clonar el repositorio:

```bash
git clone https://github.com/Rams302/GestionProyectosAI.git
```

Cambiar a la rama:

```bash
git checkout Mi-proyecto-Titanic
```

---

## 2. Abrir los notebooks en Google Colab

Abrir cualquiera de los tres notebooks:

* Logistic Regression.
* Decision Tree.
* Random Forest.

---

## 3. Agregar el dataset

Antes de ejecutar el código es necesario copiar manualmente el archivo:

```
Titanic-Dataset.csv
```

dentro del ambiente de ejecución de Google Colab.

La estructura esperada es:

```
GestionProyectosAI

│
├── data
│   └── Titanic-Dataset.csv
│
├── notebooks
│
├── results
│
├── src
│
└── requirements.txt
```

---

## 4. Instalar dependencias

Ejecutar:

```python
!pip install -r requirements.txt
```

---

## 5. Ejecutar los notebooks

Ejecutar cada notebook de manera independiente:

```
Logistic Regression.ipynb
```

```
Decision Tree.ipynb
```

```
Random Forest.ipynb
```

Cada notebook generará los resultados correspondientes del modelo seleccionado.

---

# Archivos de soporte del proyecto

## requirements.txt

Contiene las librerías necesarias para ejecutar los modelos Machine Learning.

Incluye:

* Procesamiento de datos.
* Entrenamiento de modelos.
* Evaluación.
* Visualización.

---

## data/

Contiene el dataset utilizado:

```
Titanic-Dataset.csv
```

Este archivo representa la fuente de información utilizada para entrenar y evaluar los modelos.

---

## notebooks/

Contiene los notebooks desarrollados en Google Colab:

```
Logistic Regression
Decision Tree
Random Forest
```

---

## results/

Carpeta destinada para almacenar:

* Métricas obtenidas.
* Resultados de evaluación.
* Gráficas generadas.

---

## src/

Contiene los códigos fuente asociados al desarrollo del proyecto.

Incluye la implementación de los modelos:

* Logistic Regression.
* Decision Tree.
* Random Forest.

---

# Conclusiones

El proyecto permitió aplicar un ciclo completo de desarrollo de un modelo de Inteligencia Artificial, integrando actividades de preparación de datos, entrenamiento, validación y análisis de resultados.

La comparación de los tres algoritmos permitió observar las diferencias entre modelos simples y modelos basados en conjuntos de aprendizaje.

**Logistic Regression** funciona como una solución inicial eficiente debido a su facilidad de interpretación y bajo costo computacional.

**Decision Tree** permite comprender mejor los patrones encontrados en los datos mediante reglas de decisión, aunque puede presentar mayor riesgo de sobreajuste.

**Random Forest** representa una alternativa más robusta al combinar múltiples árboles de decisión, logrando generalmente mayor estabilidad y capacidad de generalización.

Como resultado del proyecto se concluye que la selección de un modelo de Inteligencia Artificial debe considerar no solamente la precisión obtenida, sino también aspectos de gestión como:

* Complejidad.
* Tiempo de ejecución.
* Mantenimiento.
* Interpretabilidad.
* Capacidad de escalabilidad.

Este proyecto demuestra la aplicación práctica de Machine Learning dentro de un contexto de gestión de proyectos de Inteligencia Artificial, donde la evaluación técnica y la toma de decisiones basada en datos son elementos fundamentales.

```
