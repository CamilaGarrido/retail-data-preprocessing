# RetailData Analytics: Preprocesamiento y Escalamiento

Esta actividad consiste en el preprocesamiento y escalamiento de un dataset de **RetailData Analytics** para identificar clientes recurrentes. Las tareas incluyen limpiar valores nulos, codificar variables categóricas y normalizar escalas numéricas. El fin es garantizar datos aptos para el modelado predictivo de Machine Learning.

---

##  Tecnologías Utilizadas
* **Lenguaje:** Python 3.13.5
* **Librerías:** Pandas, NumPy, Scikit-Learn
* **Entorno:** VS Code con Entorno Virtual (venv)
* **Control de Versiones:** Git & GitHub

---

## Proceso Realizado

### 1. Limpieza e Imputación
Se identificaron valores faltantes (`NaN`) en la columna **Ingresos**, los cuales fueron tratados mediante **SimpleImputer** utilizando la estrategia de la **media**.

### 2. Codificación Categórica
La variable **Ciudad** fue transformada para ser compatible con algoritmos matemáticos mediante:
* **Label Encoding:** Asignación de identificadores numéricos.
* **One-Hot Encoding / Variables Dummy:** Creación de columnas binarias para evitar jerarquías inexistentes.

### 3. Escalamiento de Datos
Para homogeneizar las variables **Edad** e **Ingresos**, se aplicaron:
* **Normalización Min-Max:** Ajuste al rango [0, 1].
* **Estandarización Z-Score:** Ajuste con media 0 y desviación estándar 1.

---

##  Estructura del Repositorio
* `preprocesamiento_retail.ipynb`: Notebook principal con el código y análisis detallado.
* `RetailData_Final.csv`: Conjunto de datos procesado y listo para el modelado.
* `Informe_RetailData.pdf`: Informe ejecutivo de una página con reflexiones técnicas.
* `requirements.txt`: Lista de dependencias para replicar el entorno.

---

##  Instalación y Uso
1. Clona el repositorio.
2. Crea tu entorno virtual: `python -m venv venv`.
3. Actívalo e instala las librerías: `pip install -r requirements.txt`.
4. Ejecuta el notebook en VS Code.
