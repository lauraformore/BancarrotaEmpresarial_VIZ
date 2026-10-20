# Bancarrota empresarial · Jupyter Book

Laura Rivera · Natalý Cárdenas.

Fuentes: `index.md` (presentación y marco teórico), `EDA.ipynb` (análisis) y `style/custom.css` (presentación).

```sh
pip install -r requirements.txt
jupyter-book build . --warningiserror --keep-going
```

El resultado se encuentra en `_build/html/index.html`. La compilación usa las salidas guardadas del notebook (`execute_notebooks: off`) y no vuelve a ejecutar el análisis. El flujo de GitHub Actions compila y publica al subir cambios a `main`.

Las tablas ETL y las vistas univariadas se consultan mediante desplegables cerrados inicialmente. Cada variable numérica contiene su tabla y figura. Los boxplots usan el rango completo de observaciones; los cálculos y modelos se conservan.
