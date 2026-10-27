
# 📊 Análisis de Fuga de Clientes | Customer Churn Analysis

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)

## 📌 Descripción del proyecto

Este proyecto desarrolla un análisis exploratorio de datos (*Exploratory Data Analysis — EDA*) enfocado en identificar patrones y asociaciones relacionados con la fuga de clientes  (*Customer Churn*).

Mediante Python, visualizaciones y pruebas estadísticas, se examinan variables demográficas, económicas y de comportamiento para comprender cómo se distribuye el abandono entre distintos segmentos de clientes.

El objetivo es transformar los datos en información útil para apoyar la toma de decisiones, identificar grupos que requieren mayor atención y plantear oportunidades de mejora en las estrategias de retención.

## 🎯 Objetivos del análisis

- Evaluar la calidad e integridad del conjunto de datos.
- Cuantificar la proporción de clientes que abandonaron el banco.
- Analizar la relación entre edad y abandono.
- Comparar las tasas de fuga entre países.
- Examinar la distribución del salario estimado según el estado del cliente.
- Investigar la asociación entre el número de productos contratados y la fuga.
- Explorar diferencias de abandono según la actividad del cliente.
- Aplicar pruebas estadísticas para contrastar hipótesis.

## 💼 Problema de negocio

La fuga de clientes puede afectar la estabilidad de los ingresos, la rentabilidad y el crecimiento de una entidad financiera.

Sin un análisis segmentado, resulta difícil reconocer qué grupos presentan mayores tasas de abandono y cuáles deberían investigarse con mayor profundidad.

Este proyecto propone un enfoque analítico que permite explorar los datos, identificar patrones y generar evidencia para orientar futuras iniciativas de retención.

## 🛠️ Herramientas y tecnologías

| Herramienta | Aplicación |
|---|---|
| Python | Lenguaje principal de análisis |
| Pandas | Limpieza, transformación y análisis de datos |
| NumPy | Operaciones numéricas |
| Matplotlib | Visualización de información |
| Seaborn | Gráficos estadísticos |
| SciPy | Pruebas de hipótesis estadísticas |
| Jupyter Notebook | Desarrollo y documentación del análisis |

## 📂 Estructura del proyecto

```text
Analisis-Fuga-Clientes/
│
├── Analisis_Fuga_Clientes.ipynb
├── db_Fuga_Clientes.csv
└── README.md
```

**Archivos principales:**

- `Analisis_Fuga_Clientes.ipynb`: notebook con el proceso de análisis exploratorio, tablas, visualizaciones y pruebas estadísticas.
- `db_Fuga_Clientes.csv`: conjunto de datos utilizado como fuente para el análisis.
- `README.md`: documentación general del proyecto.

## 🔍 Metodología

### 1. Carga y exploración de datos
Importación del archivo CSV y revisión de las primeras observaciones, dimensiones y estructura del conjunto de datos.

### 2. Auditoría de calidad
Identificación de registros duplicados, valores nulos, tipos de datos y características de las variables.

### 3. Análisis estadístico descriptivo
Cálculo de medidas estadísticas y revisión de la distribución de la variable objetivo `churn`.

### 4. Análisis exploratorio y visualización
Comparación de los grupos de clientes mediante tablas y gráficos para explorar patrones de abandono.

### 5. Contraste estadístico
Aplicación de la prueba U de Mann–Whitney para explorar diferencias en las distribuciones de edad y de la prueba chi-cuadrado para evaluar la asociación entre variables categóricas.

### 6. Interpretación de resultados
Evaluación de los patrones encontrados, considerando la magnitud de las diferencias, el tamaño de los grupos y las limitaciones del análisis.

## 📈 Variables analizadas

| Variable | Descripción |
|---|---|
| `abandono` | Estado de abandono del cliente |
| `edad` | Edad del cliente |
| `pais` | País del cliente |
| `salario` | Salario estimado |
| `producto` | Número de productos contratados |
| `estado` | Indicador de actividad del cliente |

## 📊 Indicadores y análisis

El notebook contempla los siguientes componentes analíticos:

- **Tasa de fuga:** porcentaje de clientes que abandonaron el banco.
- **Distribución demográfica:** comparación de edades según el estado de abandono.
- **Segmentación geográfica:** análisis de la fuga por país.
- **Análisis económico:** comparación de salarios estimados entre grupos.
- **Relación con productos:** tasa de abandono según la cantidad de productos contratados.
- **Actividad del cliente:** exploración del abandono según su estado de actividad.
- **Validación estadística:** pruebas para evaluar si las diferencias observadas cuentan con evidencia estadística.

## 🧪 Pruebas estadísticas

### U de Mann–Whitney

Se utiliza para evaluar si existen diferencias entre las distribuciones de edad de los clientes que abandonaron y los que permanecieron.

### Chi-cuadrado de independencia

Se utiliza para examinar si existe asociación entre el número de productos contratados y el estado de abandono.

Se considera un nivel de significancia de **0,05** como referencia para interpretar los resultados estadísticos.

> La significancia estadística no implica causalidad. Los resultados deben interpretarse considerando los supuestos de cada prueba y las características de los datos.

## 🚀 Cómo ejecutar el proyecto

### Requisitos

- Python 3.10 o superior recomendado.
- Jupyter Notebook o JupyterLab.
- Las bibliotecas utilizadas en el análisis.

### Instalación de dependencias

```bash
pip install pandas numpy matplotlib seaborn scipy jupyter
```

### Ejecución

1. Clona o descarga este repositorio.
2. Guarda `Analisis_Fuga_Clientes.ipynb` y `db_Fuga_Clientes.csv` en la misma carpeta.
3. Abre una terminal en esa carpeta.
4. Ejecuta:

```bash
jupyter notebook
```

5. Abre `Analisis_Fuga_Clientes.ipynb`.
6. Ejecuta las celdas en orden.

## 📌 Hallazgos y resultados

El notebook permite examinar las diferencias entre los grupos de clientes, detectar segmentos con mayores tasas de abandono y evaluar asociaciones estadísticas entre las variables seleccionadas.

Los hallazgos cuantitativos definitivos deben documentarse a partir de los resultados obtenidos al ejecutar el análisis sobre el archivo CSV.

Este enfoque evita publicar cifras no verificadas y facilita la actualización de las conclusiones cuando se utilicen nuevos datos.

## 🔮 Oportunidades de mejora

Como evolución del proyecto, se propone:

- Incorporar un dashboard interactivo en Power BI.
- Desarrollar una segmentación de clientes por riesgo de fuga.
- Evaluar modelos predictivos de clasificación.
- Medir la importancia de las variables mediante técnicas estadísticas y de aprendizaje automático.
- Diseñar indicadores de seguimiento para las estrategias de retención.
- Automatizar la actualización y generación de reportes.

## ⚠️ Limitaciones

- El análisis identifica patrones y asociaciones, pero no demuestra relaciones causales.
- Las conclusiones dependen de la calidad, representatividad y período de los datos.
- Las pruebas estadísticas deben interpretarse considerando sus supuestos.
- No se presenta un modelo predictivo entrenado ni una validación de rendimiento en esta etapa.

## 👨‍💻 Autor

**Milton Vivero** - People And Data Analytics

Analisis diseñado para el área de Suscripción con fines de control, seguimiento y toma de decisiones estratégicas.


🔗 **GitHub:** [github.com/milton-vivero](https://github.com/milton-vivero)

---

⭐ Si este proyecto te resulta útil, puedes explorar el repositorio y seguir su evolución.
