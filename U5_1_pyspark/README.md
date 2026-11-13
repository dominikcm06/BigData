# U5_1 PySpark

Proyecto de la Unidad 5 de Tópicos de Big Data: introducción a PySpark.

## Práctica 5.1 — Preparación de PySpark y exploración de NYC Taxi

Comprobación del entorno de PySpark en VS Code (SparkSession, DataFrames pequeños) y exploración de una muestra de NYC Yellow Taxi de enero de 2025 ([NYC TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)). Ver [`notebooks/U5_1_preparation_pyspark_NYC_taxi.ipynb`](notebooks/U5_1_preparation_pyspark_NYC_taxi.ipynb).

El notebook lee el archivo Parquet por HTTP con PyArrow y no guarda el dataset en disco, por lo que `data/raw/` queda vacío. Spark se ejecuta de forma local, y requiere tener **Java** instalado (el notebook comprueba la versión en la primera celda).

## Estructura del proyecto

```
U5_1_pyspark/
├── .venv/                          ← Entorno virtual local (NO se sube a GitHub)
├── data/
│   ├── raw/                        ← Datos originales
│   └── processed/                  ← Datos transformados
├── notebooks/                      ← Jupyter Notebooks
│   └── U5_1_preparation_pyspark_NYC_taxi.ipynb
├── src/                            ← Código Python reutilizable
├── .gitignore                      ← Archivos/carpetas que Git debe ignorar
├── README.md                       ← Documentación del proyecto
└── requirements.txt                ← Dependencias Python
```

## Configuración del entorno

1. Crear el entorno virtual (o reutilizar el de otra carpeta del curso, ya que `.venv/` no se sube a GitHub):

   ```bash
   python -m venv .venv
   ```

2. Activar el entorno virtual:

   - Windows (PowerShell):
     ```powershell
     .venv\Scripts\Activate.ps1
     ```
   - Windows (cmd):
     ```cmd
     .venv\Scripts\activate.bat
     ```
   - Git Bash / Linux / macOS:
     ```bash
     source .venv/Scripts/activate
     ```

3. Instalar las dependencias:

   ```bash
   pip install -r requirements.txt
   ```

4. Lanzar Jupyter Notebook:

   ```bash
   jupyter notebook notebooks/
   ```
