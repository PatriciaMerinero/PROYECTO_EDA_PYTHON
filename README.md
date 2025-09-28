<img width="449" height="315" alt="image" src="https://github.com/user-attachments/assets/f8f0aae5-6b6e-4d02-b64f-6eb3f76d528f" />

# 🐍Data Analytics. Módulo 7. Python for data. Eda con Python.

* Análisis Exploratorio de Datos (EDA) de una campaña de marketing de un banco portugués, usando **Python** y **Jupyter/VS Code**.  
* Se parte de dos fuentes (campaña y clientes), se limpian y transforman, y se genera un dataset combinado para el EDA.


# 📝Descripción

* Comprender el comportamiento de los clientes y la respuesta a la campaña.
* Documentar calidad de datos, transformaciones realizadas y hallazgos principales.
* El fin es identificar los factores que influyen en la suscripción de depósitos a plazo y obtener insights que permitan optimizar futuras estrategias de marketing.


# 📂 Estructura 
```
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
```


# ⚙️Instalación y requisitos

* Requisitos previos

  *Tener instalado Python 3.8+ (o la versión que uses).

  *Tener git instalado.
  
  * Recomendable usar un entorno virtual (venv, conda, etc.) para aislar dependencias.

  ### Pasos de instalación

#### 1. Clona tu repositorio
git clone https://github.com/PatriciaMerinero/PROYECTO_EDA_PYTHON.git

#### 2. Entra al directorio del proyecto
cd PROYECTO_EDA_PYTHON

#### 3. Crea y activa un entorno virtual (ej. venv)
python -m venv .venv
  * En Windows:
.venv\Scripts\activate
  * En macOS / Linux:
source .venv/bin/activate

#### 4. Instala las dependencias
pip install -r requirements.txt


  

**Recomendable usar un entorno virtual (venv, conda, etc.) para aislar dependencias.**
## Entorno (Windows + venv)
```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m ipykernel install --user --name eda-venv --display-name "Python (eda-venv)"
```
 
 

 ## Requisitos / dependencias

El archivo requirements.txt contiene las versiones específicas de las librerías usadas, por ejemplo:

```
pandas
numpy
seaborn
matplotlib
openpyxl
pycountry
reverse_geocoder
scipy
ipykernel
jupyter
```
Estas versiones garantizan que los notebooks funcionen igual que en tu máquina.

## Cómo ejecutar los notebooks

* Después de instalar todo, lanza Jupyter.

* Abre los notebooks en este orden:

* 01-analisis_preliminar_limpieza_transformacion.ipynb

* 02_EDA.ipynb

* 03_Informe.ipynb

**El notebook 01 genera los archivos customer_clean.csv y bank_clean.csv en Data/Output/.
Luego el notebook 02 genera full_clean.csv en la misma carpeta.**

En 03_Informe.ipynb esta explicado todo el EDA


# 📈Resultado y conclusiones


Los resultados muestran que la efectividad de las campañas depende de una combinación de factores:


* A nivel individual, la edad, la duración de la llamada y la existencia de contactos previos son claves para el éxito.
* A nivel de campaña, es más eficiente centrarse en pocos intentos de calidad que en la insistencia repetitiva.
* A nivel macroeconómico, el contexto de bajos tipos de interés y menor empleo favorece la contratación de depósitos.
* El dataset presenta un claro desbalance en la variable objetivo: solo un 11,25% de los clientes contrató el depósito, mientras que el 88,75% rechazó.
* La edad muestra cierta señal: los clientes que aceptan tienden a ser ligeramente mayores.
* Los ingresos no discriminan significativamente entre aceptación y rechazo.
* Las condiciones macroeconómicas son relevantes: mayor aceptación cuando el euribor3m es bajo y el número de empleados (nr.employed) es reducido.


# 🚀Próximos pasos.

* Revisar mejor algunas variables que no se han explorado en detalle.

* Probar más gráficos para entender mejor los datos (ej. histogramas, gráficos de dispersión).

* Hacer un resumen más visual de los hallazgos principales.

* Empezar a probar algún modelo sencillo de predicción (ej. regresión logística).

* Documentar mejor cada paso en los notebooks.
  


# 🤝 Autora, contribuciones y agradecimientos


Este proyecto ha sido realizado por **Patricia Merinero** como parte de su aprendizaje en
**análisis exploratorio de datos (EDA) con Python**.

Durante el desarrollo se contó con apoyo y guía en:
- Limpieza y transformación de datos.
- Interpretación de resultados y visualizaciones.
- Redacción del informe paso a paso.

👉 Si alguien quiere contribuir, puede:

* Probar nuevas visualizaciones.

* Añadir ejemplos de modelado predictivo.

* Mejorar la documentación del proyecto.

  ### 💡 Cómo contribuir
¡Se aceptan _issues_ y _pull requests_!
- Propón nuevas visualizaciones o mejoras de EDA.
- Sugiere refactors de notebooks/código o mejoras de documentación.
- Abre un **Issue** describiendo el cambio antes de enviar el PR.

  ### 🙏 Agradecimientos
- A los/las tutores/as que revisaron el trabajo y dieron feedback.
- A las comunidades de **pandas**, **matplotlib** y **seaborn**.
- A la fuente de datos de la campaña bancaria y al conjunto de clientes usados en el proyecto.

### ✉️ Contacto
Si tienes dudas o sugerencias: patriciamerinero@yahoo.es






