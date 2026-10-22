# Bancarrota empresarial · Jupyter Book

Laura Rivera · Natalý Cárdenas.

Fuentes: `index.md` (presentación y marco teórico), `EDA.ipynb` (análisis) y `style/custom.css` (presentación).

```sh
pip install -r requirements.txt
jupyter-book build . --warningiserror --keep-going
```

El resultado se encuentra en `_build/html/index.html`. La compilación usa las salidas guardadas del notebook (`execute_notebooks: off`) y no vuelve a ejecutar el análisis. El flujo de GitHub Actions compila y publica al subir cambios a `main`.

Las salidas individuales se muestran directamente, con tablas formateadas y desplazamiento para listados extensos. Los desplegables se reservan para las colecciones de muchas variables: cada variable numérica contiene su tabla, figura e interpretación. Los boxplots usan el rango completo de observaciones; los cálculos y modelos se conservan.
