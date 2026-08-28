# Modelo de Clasificación Binaria para la Predicción de Bancarrota Empresarial a partir de Estados Financieros: Dataset Taiwan Economic Journal

***Análisis de Solvencia Corporativa y Riesgo Financiero con Machine Learning*** 

**Laura Rivera · Natalý Cárdenas** Departamento de Matemáticas, Física y Ciencia de Datos, Universidad del Norte, Barranquilla, Colombia
`sriveral@uninorte.edu.co` · `nizaquita@uninorte.edu.co`

::::{grid} 1 1 3 3
:gutter: 2

:::{grid-item-card} Asignatura
:class-card: meta-card
Visualización de Datos
:::

:::{grid-item-card} Autoras
:class-card: meta-card
Laura Rivera & Natalý Cárdenas

*Departamento de Matemáticas, Física y Ciencia de Datos*
*Universidad del Norte*
:::

:::{grid-item-card} Metodología
:class-card: meta-card
EDA · Feature Engineering · Modelos de Clasificación
:::

::::

## Resumen del Proyecto
Este proyecto desarrolla un análisis integral del riesgo de insolvencia empresarial a partir de indicadores financieros corporativos. En primer lugar, se realiza un análisis exploratorio de datos (EDA) para comprender la estructura del conjunto de datos, estudiar la distribución de las variables, identificar valores faltantes, detectar posibles sesgos y examinar las relaciones entre los indicadores de solvencia y la quiebra empresarial.

Posteriormente, se prepara la información para el modelado mediante la eliminación de la variable constante `Net Income Flag` y la estandarización de las variables numéricas. Debido al desequilibrio entre las empresas solventes y las empresas en quiebra, se emplea `class_weight='balanced'`, con el objetivo de otorgar mayor importancia a la clase minoritaria y reducir el riesgo de pasar por alto casos de insolvencia.

Finalmente, se entrena un modelo de clasificación y se evalúa utilizando métricas adecuadas para problemas desbalanceados, especialmente *Recall* y ROC-AUC. El propósito es identificar las variables financieras más relacionadas con el riesgo y construir una herramienta predictiva que permita detectar oportunamente empresas con mayor probabilidad de quiebra.


## Estructura del Análisis

::::{grid} 1 1 2 2
:gutter: 2

:::{grid-item-card} 1. Análisis Exploratorio (EDA)
:class-card: step-card
Evaluación de distribuciones, tratamiento de valores faltantes, detección de sesgo y análisis de correlación entre variables financieras.
:::

:::{grid-item-card} 2. Modelado y Predicción
:class-card: step-card
Entrenamiento de algoritmos supervisados, optimización de hiperparámetros y evaluación de métricas orientadas a la detección de riesgo (Recall / ROC-AUC).
:::

::::



:::{seealso} Enlaces de interés
**Conjunto de datos**
- [UCI Machine Learning Repository — Taiwanese Bankruptcy Prediction](https://archive.ics.uci.edu/dataset/572/taiwanese+bankruptcy+prediction)
- [Kaggle — Company Bankruptcy Prediction](https://www.kaggle.com/datasets/fedesoriano/company-bankruptcy-prediction)

**Repositorio del proyecto**
- [GitHub](https://github.com/lauraformore/BancarrotaEmpresarial_VIZ)
:::