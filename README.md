<img width="449" height="315" alt="image" src="https://github.com/user-attachments/assets/f8f0aae5-6b6e-4d02-b64f-6eb3f76d528f" />

# 🐍Data Analytics. Módulo 7. Python for data. Eda con Python.

* Análisis Exploratorio de Datos (EDA) de una campaña de marketing de un banco portugués, usando **Python** y **Jupyter/VS Code**.  
* Se parte de dos fuentes (campaña y clientes), se limpian y transforman, y se genera un dataset combinado para el EDA.
* El fin es identificar los factores que influyen en la suscripción de depósitos a plazo y obtener insights que permitan optimizar futuras estrategias de marketing.


# 📝Descripción

* Comprender el comportamiento de los clientes y la respuesta a la campaña.
* Documentar calidad de datos, transformaciones realizadas y hallazgos principales.
* El fin es identificar los factores que influyen en la suscripción de depósitos a plazo y obtener insights que permitan optimizar futuras estrategias de marketing.


# 🗂️Estructura

PROYECTO_EDA_PYTHON/
│── Data/
│ ├── Raw/ # Datos originales
│ │ ├── bank-additional.csv
│ │ └── customer-details.xlsx
│ ├── Output/ # Datos limpios y transformados
│ │ ├── bank_clean.csv
│ │ ├── customer_clean.csv
│ │ └── full_clean.csv
│
│── Notebook/ # Notebooks de trabajo
│ ├── 01_analisis_preliminar_limpieza_transformacion.ipynb
│ ├── 02_EDA.ipynb
│ └── 03_Informe.ipynb
│
│── .gitignore
│── README.md
│── requirements.txt

















## Entorno (Windows + venv)
```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m ipykernel install --user --name eda-venv --display-name "Python (eda-venv)"



