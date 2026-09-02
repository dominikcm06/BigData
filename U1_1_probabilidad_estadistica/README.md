# U1_1 Probabilidad y Estadística

Proyecto de la Unidad 1 de Tópicos de Big Data: análisis de probabilidad y estadística.

## Práctica 1.1 — Análisis de la evolución poblacional mundial

Análisis exploratorio y estadística descriptiva sobre datos reales de población mundial (Naciones Unidas, *World Population Prospects 2024*, procesados por [Our World in Data](https://ourworldindata.org/)). Ver [`notebooks/01_evolucion_poblacional.ipynb`](notebooks/01_evolucion_poblacional.ipynb).

## Estructura del proyecto

```
U1_1_probabilidad_estadistica/
├── .venv/                          ← Entorno virtual local (NO se sube a GitHub)
├── data/
│   ├── raw/                        ← Datos originales (proporcionados por la maestra)
│   │   ├── annual-population-growth/
│   │   │   ├── annual-population-growth.csv
│   │   │   ├── annual-population-growth.metadata.json
│   │   │   └── readme.md
│   │   └── births-and-deaths-projected-to-2100/
│   │       ├── births-and-deaths-projected-to-2100.csv
│   │       ├── births-and-deaths-projected-to-2100.metadata.json
│   │       └── readme.md
│   └── processed/                  ← Datos transformados
├── notebooks/                      ← Jupyter Notebooks
│   └── 01_evolucion_poblacional.ipynb
├── src/                            ← Código Python reutilizable
├── .gitignore                      ← Archivos/carpetas que Git debe ignorar
├── README.md                       ← Documentación del proyecto
└── requirements.txt                ← Dependencias Python
```

## Configuración del entorno

1. Crear el entorno virtual:

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
   jupyter notebook notebooks/01_evolucion_poblacional.ipynb
   ```
