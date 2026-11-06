# Análisis de Matrículas de Personas Naturales y Jurídicas en Valledupar

## 1. Descripción del proyecto

Este proyecto desarrolla un análisis exploratorio de datos (EDA) sobre las matrículas mercantiles activas de personas naturales y jurídicas en Valledupar, Cesar, Colombia.

A partir de información suministrada por la Cámara de Comercio de Valledupar para el Valle del Río Cesar, se busca identificar patrones en la estructura empresarial de la región, comprender la distribución de las organizaciones jurídicas, reconocer los sectores económicos predominantes y analizar el comportamiento de las matrículas según su clasificación empresarial.

El proyecto utiliza Python y herramientas estadísticas para transformar datos en información útil para la interpretación de la dinámica empresarial local.

## 2. Objetivos

**Objetivo general**

Aplicar conceptos estadísticos y herramientas de análisis de datos mediante Python para explorar, transformar e interpretar información sobre las matrículas mercantiles de personas naturales y jurídicas en Valledupar.

**Objetivos específicos**

- Examinar la estructura y calidad del conjunto de datos.
- Identificar y tratar posibles inconsistencias en los tipos de variables.
- Analizar la distribución de las empresas según su organización jurídica y clasificación empresarial.
- Identificar las actividades económicas con mayor representación.
- Explorar asociaciones estadísticas entre la organización jurídica y el tamaño empresarial.
- Construir visualizaciones y un dashboard para comunicar los principales resultados.

## 3. Fuente de información

Los datos utilizados fueron suministrados por la **Cámara de Comercio de Valledupar para el Valle del Río Cesar**.

El conjunto de datos corresponde a personas naturales y jurídicas activas matriculadas en su jurisdicción.

**Características iniciales del conjunto de datos:**

| Característica | Descripción |
|---|---|
| Registros | 17.260 |
| Variables iniciales | 8 |
| Total de observaciones | 138.080 valores |
| Tipo de información | Matrículas mercantiles activas |
| Cobertura geográfica | Valledupar, Cesar |
| Fuente | Cámara de Comercio de Valledupar |

## 4. Herramientas y tecnologías

El proyecto fue desarrollado utilizando las siguientes herramientas:

- **Python:** lenguaje de programación para el procesamiento y análisis.
- **Pandas:** manipulación, limpieza y transformación de datos.
- **NumPy:** operaciones numéricas.
- **Matplotlib:** visualización de datos.
- **Seaborn:** análisis gráfico y visualizaciones estadísticas.
- **SciPy:** aplicación de pruebas estadísticas, incluyendo chi-cuadrado.
- **Missingno:** identificación y visualización de valores faltantes.
- **PyJanitor:** herramientas complementarias para limpieza de datos.
- **Empiricaldist:** análisis de distribuciones empíricas.
- **UpSetplot:** exploración de intersecciones y conjuntos.
- **Jupyter Notebook / Google Colab:** entorno de desarrollo.

## 5. Metodología

El análisis se desarrolló en las siguientes etapas:

### 5.1. Preparación y exploración de datos

- Importación del conjunto de datos.
- Inspección de dimensiones y estructura.
- Identificación de tipos de variables.
- Renombramiento de columnas para facilitar su interpretación.
- Conversión de fechas al formato datetime.
- Transformación de variables de renovación.
- Separación de códigos y descripciones de actividades económicas.

### 5.2. Calidad y limpieza de datos

Se evaluó la presencia de valores nulos mediante diferentes procedimientos de Pandas y Missingno.

El resultado inicial fue de cero valores nulos en los 17.260 registros.

También se realizaron transformaciones para facilitar los análisis posteriores.

### 5.3. Análisis exploratorio de datos (EDA)

Se desarrollaron diferentes preguntas de investigación:

- ¿Cuáles son los años con mayor número de matrículas de microempresas?
- ¿Cuántas empresas se registraron según su clasificación empresarial?
- ¿Cuáles son las actividades económicas más representativas?
- ¿Qué tipo de organización jurídica predomina?
- ¿Existe una asociación entre la organización jurídica y la clasificación empresarial?
- ¿Cómo se distribuye la clasificación empresarial por actividad económica?

### 5.4. Análisis estadístico

Se utilizaron tablas de contingencia y la prueba chi-cuadrado de independencia para explorar la asociación entre la organización jurídica y la clasificación empresarial.

También se calculó la correlación entre las variables codificadas, diferenciando la asociación categórica de la relación lineal.

### 5.5. Visualización de datos

Se construyeron gráficos para representar:

- Distribución de las organizaciones jurídicas.
- Actividades económicas predominantes.
- Matrículas por año y clasificación empresarial.
- Distribución de empresas por sector económico.
- Asociación entre organización jurídica y clasificación.

Adicionalmente, se desarrolló un dashboard para facilitar la exploración de los resultados.

## 6. Principales resultados

A partir de los resultados documentados en el proyecto, se identificaron los siguientes hallazgos:

**Predominio de microempresas**

Las microempresas representan el 97,41 % de los registros presentados en el informe técnico, evidenciando su importancia dentro de la estructura empresarial analizada.

**Comportamiento de las matrículas**

Entre 2017 y 2021, los años con mayor número de matrículas de microempresas fueron:

| Año | Matrículas |
|---|---:|
| 2020 | 3.060 |
| 2019 | 2.576 |
| 2021 | 2.062 |
| 2018 | 1.579 |
| 2017 | 1.356 |

**Actividades económicas**

El comercio al por mayor y al por menor se identifica como una de las actividades económicas predominantes en el conjunto de datos.

**Organización jurídica**

Las personas naturales representan la mayor proporción de registros, seguidas por las sociedades por acciones simplificadas (SAS).

**Prueba de chi-cuadrado**

Se obtuvo el siguiente resultado:

- Estadístico chi-cuadrado: 2790,35.
- Valor p: 0,0000 (redondeado a cuatro decimales).

El resultado indica evidencia estadística de asociación entre la organización jurídica y la clasificación empresarial.

Por otra parte, la correlación lineal calculada fue de -0,054, lo que evidencia una relación lineal muy débil entre las variables codificadas.

## 7. Dashboard

El proyecto incorpora un dashboard interactivo para explorar la información empresarial mediante filtros y diferentes indicadores.

Entre sus componentes se encuentran:

- Filtros por año de matrícula.
- Filtros por clasificación empresarial.
- Distribución por organización jurídica.
- Actividad económica predominante.
- Indicadores generales de registros.
- Evolución histórica de las matrículas.

## 8. Estructura del repositorio

```text
Analisis-de-Matriculas-Naturales-y-Juridicas/
│
├── README.md
├── analisis_matriculas_naturales_juridicas.ipynb
│
├── data/
│   └── datos.csv
│
└── requirements.txt
```

*La carpeta data y el archivo requirements.txt representan la estructura recomendada para organizar y reproducir el proyecto.*

## 9. Instalación y ejecución

Para ejecutar el proyecto se requiere Python y las librerías utilizadas en el análisis.

Instalación de dependencias:

```bash
pip install pandas numpy matplotlib seaborn scipy empiricaldist pyjanitor missingno upsetplot
```

Posteriormente:

1. Clonar el repositorio.
2. Instalar las dependencias.
3. Ubicar el conjunto de datos en la carpeta correspondiente.
4. Configurar la ruta de acceso al archivo CSV.
5. Abrir el notebook en Jupyter Notebook, JupyterLab o Google Colab.
6. Ejecutar las celdas en orden.

**Nota:** El notebook original utiliza Google Drive y una extensión personalizada de Pandas (`pandas-missing-extension.ipynb`). Para reproducirlo fuera del entorno original será necesario adaptar esas rutas y disponer de dicha extensión o ajustar las celdas correspondientes.

## 10. Consideraciones y limitaciones

- El conjunto de datos corresponde a matrículas activas y no representa necesariamente la totalidad de empresas creadas históricamente en Valledupar.
- Los resultados dependen de la información disponible y de la fecha de actualización de la fuente.
- La asociación estadística identificada no implica causalidad.
- La correlación entre variables categóricas codificadas debe interpretarse con precaución.
- Los resultados sobre formalización no deben confundirse con una medición directa de la informalidad empresarial.

## 11. Conclusiones

El análisis permite identificar características relevantes del tejido empresarial de Valledupar, destacando la participación de las microempresas, la importancia de las actividades comerciales y la predominancia de las personas naturales dentro de los registros examinados.

La aplicación de herramientas de análisis estadístico y visualización facilita la interpretación de estos patrones y proporciona una base para futuras investigaciones sobre la dinámica empresarial de la región.

Como posibles líneas de desarrollo se plantean la incorporación de información geográfica, el análisis de nuevas series temporales y la construcción de modelos de segmentación empresarial.

## 12. Autor

**Sebastián Santiago Pazo**

Estudiante de Negocios Internacionales | Análisis de Datos

Intereses: Python, análisis exploratorio de datos, estadística, visualización de información y análisis empresarial.

---

*Proyecto académico de análisis de datos desarrollado con Python.*
