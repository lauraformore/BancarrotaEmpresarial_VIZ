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

## Introducción 

Predecir con anticipación el riesgo de bancarrota de una empresa es un problema de alto impacto: permite a inversionistas, entidades financieras y a la propia gerencia tomar decisiones oportunas para prevenir o mitigar pérdidas, en lugar de reaccionar cuando la quiebra ya es inminente. Contar con un modelo que identifique señales tempranas de riesgo financiero, a partir de indicadores contables que las empresas ya reportan, aporta valor tanto para el análisis de crédito como para la supervisión financiera.

Para este proyecto se utiliza el dataset del **Taiwan Economic Journal**, que reúne información financiera de **6.819 empresas** que cotizaron en la Bolsa de Taiwán entre 1999 y 2009. Cada empresa está descrita por **95 ratios financieros** (rentabilidad, liquidez, endeudamiento, eficiencia operativa, entre otros) y por una variable objetivo binaria que indica si la empresa terminó en bancarrota o no.


## Marco Teórico

**Riesgo de insolvencia / quiebra empresarial:** es la probabilidad de que una empresa no pueda cumplir con sus obligaciones financieras (pago de deudas, proveedores, nómina, etc.) y, como consecuencia, entre en un proceso legal de bancarrota. Este riesgo suele acumularse de forma progresiva y deja huellas medibles en los estados financieros de la empresa mucho antes de que la quiebra sea formal.

**Ratios financieros:** son relaciones entre dos cifras del estado financiero de una empresa (por ejemplo, utilidad neta entre activos totales) que permiten comparar el desempeño de empresas de tamaños distintos en una misma escala, y que resumen aspectos como rentabilidad, liquidez, endeudamiento y eficiencia.

**Modelos de clasificación:** dado que el problema consiste en distinguir entre dos categorías (empresa que quiebra vs. empresa que no quiebra) a partir de los ratios financieros, es natural abordarlo como un problema de **clasificación binaria supervisada**. Un modelo de este tipo aprende, a partir de datos históricos etiquetados, los patrones en los ratios que están asociados con la quiebra, para luego poder estimar el riesgo de empresas nuevas.

## Objetivos

### Objetivo general
Desarrollar un dashboard con un modelo predictivo de riesgo de bancarrota empresarial, que permita explorar los datos financieros de las empresas y estimar su nivel de riesgo.

### Objetivos específicos
- Realizar un análisis exploratorio de datos (EDA) que permita entender la calidad, distribución y relaciones entre los ratios financieros del dataset.
- Tratar el desbalance de clases presente en la variable objetivo antes de entrenar los modelos.
- Entrenar y comparar distintos modelos de clasificación para identificar el que mejor predice el riesgo de bancarrota.
- Construir un dashboard interactivo que integre el EDA y, en etapas posteriores, el modelo predictivo.

## Metodología

El proyecto sigue un flujo de trabajo secuencial: primero un **análisis exploratorio de datos (EDA)**, que permite entender la estructura, calidad y relaciones entre las variables; luego un **preprocesamiento**, donde se tratan los problemas identificados en el EDA (variables redundantes, desbalance de clases, escalas distintas, entre otros); después el **modelado**, en el que se entrenan y comparan distintos algoritmos de clasificación; y finalmente la construcción del **dashboard**, que integra los resultados de las etapas anteriores en una herramienta interactiva.


## Resumen del Proyecto
Este proyecto desarrolla un análisis integral del riesgo de insolvencia empresarial a partir de indicadores financieros corporativos. En primer lugar, se realiza un análisis exploratorio de datos (EDA) para comprender la estructura del conjunto de datos, estudiar la distribución de las variables, identificar valores faltantes, detectar posibles sesgos y examinar las relaciones entre los indicadores de solvencia y la quiebra empresarial.


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