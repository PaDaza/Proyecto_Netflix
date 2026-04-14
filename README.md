# Proyecto Integrado de Ciencia de Datos
## Análisis de comportamiento de usuarios de Netflix

### Integrantes
- Johann carrasco
- Pablo Daza
- Ricardo Ruiz

### Asignatura
Programación para la Ciencia de Datos (SCY1101)

---

## Descripción del proyecto
Este proyecto fue desarrollado para la Evaluación Parcial N°1 de la asignatura **Programación para la Ciencia de Datos**.

El objetivo fue trabajar un flujo completo de ciencia de datos sobre un dataset de comportamiento de usuarios de Netflix, aplicando exploración, limpieza, transformación, visualización y documentación del proceso.

---

## Origen del dataset
El dataset utilizado corresponde a un archivo de comportamiento de usuarios de Netflix.

Archivos principales del proyecto:
- `data/raw/netflix_user_behavior_dataset(4).csv`
- `data/processed/netflix_processed.csv`
- `notebook_netflix_.ipynb`

Para fines académicos, se trabajó con una versión ensuciada del dataset, con el fin de aplicar de manera más clara las etapas de limpieza solicitadas en la evaluación.

---

## Objetivo del análisis
Preparar el dataset para futuros análisis, aplicando técnicas básicas de limpieza y transformación de datos de forma ordenada, documentada y reproducible.

---

## Etapas desarrolladas

### 1. Exploración inicial
Se revisó la estructura general del dataset mediante:
- dimensiones
- tipos de datos
- estadísticas descriptivas
- valores nulos
- filas duplicadas

### 2. Limpieza de datos
En esta fase se trabajó con:
- revisión de valores nulos
- revisión y eliminación de duplicados
- revisión de posibles outliers
- eliminación de la columna `user_id`

Además, se dejó un dataset procesado y más ordenado para continuar con la transformación.

### 3. Transformación de datos
Se aplicaron técnicas de transformación avanzada, entre ellas:
- creación de la variable `nivel_actividad`
- escalamiento de variables numéricas con `StandardScaler`
- codificación de variables categóricas con `OneHotEncoder`

### 4. Pipeline
Se utilizó `ColumnTransformer` junto con `Pipeline` para automatizar el preprocesamiento de los datos y mejorar la reproducibilidad del flujo.

### 5. Visualización final
Se generó una visualización final para resumir la relación entre el nivel de actividad del usuario y la variable `churned`.

---

## Estructura del repositorio
```text
Proyecto_Netflix/
│
├── data/
│   ├── raw/
│   │   └── netflix_user_behavior_dataset(4).csv
│   └── processed/
│       └── netflix_processed.csv
│
├── notebook_netflix_.ipynb
├── README.md
```

---

## Justificación del entorno de trabajo
Se decidió utilizar **Google Colab** para desarrollar el notebook, ya que permite trabajar de forma simple con archivos `.ipynb`, ejecutar el código por bloques y visualizar resultados rápidamente.

Además, GitHub fue utilizado para almacenar el proyecto, mantener el versionado y facilitar el trabajo colaborativo, tal como se solicita en la pauta.

---

## Reproducibilidad
El proyecto fue organizado para que cualquier persona pueda ejecutar el notebook desde el inicio hasta el final, siempre que tenga disponibles las librerías necesarias y los archivos del dataset en la estructura correspondiente del repositorio.

---

## Librerías utilizadas
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

## Reflexión grupal
Este proyecto permitió aplicar un flujo completo de trabajo en ciencia de datos, desde la carga del dataset hasta su transformación final.

Como grupo, fue importante documentar cada etapa y mantener un orden claro en el notebook, ya que esto facilita la reproducibilidad y el trabajo colaborativo. Además, el uso de GitHub permitió registrar avances, organizar versiones y compartir el proyecto de manera más profesional.

---

## Conclusión
Este trabajo permitió aplicar de forma práctica las etapas principales del preprocesamiento de datos. A través de la exploración, limpieza, transformación y documentación del flujo, se logró preparar un dataset de manera más clara, ordenada y reproducible.
