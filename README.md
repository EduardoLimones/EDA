# 📊 Análisis de la "Guerra de Consolas": Sony vs. Nintendo

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.5-blue.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-blue.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-blue.svg)
![SciPy](https://img.shields.io/badge/SciPy-1.10-blue.svg)

### 📖 Contexto del Proyecto

¿Sabías que la PlayStation nació de una colaboración fallida entre Sony y Nintendo? Este proyecto es un **Análisis Exploratorio de Datos (EDA)** que se sumerge en la histórica rivalidad de estos dos gigantes japoneses para responder a la pregunta: **¿quién ha dominado realmente el mercado de los videojuegos?**

Para ello, se analizan y comparan las ventas históricas de hardware y software, culminando en una prueba de hipótesis para validar estadísticamente los hallazgos.

---

### 🗂️ Índice

1.  [Objetivos y Preguntas](#-objetivos-y-preguntas-analizadas)
2.  [Metodología](#-metodología)
3.  [Conclusiones Principales](#-conclusiones-principales)
4.  [Visualizaciones Destacadas](#-visualizaciones-destacadas)
5.  [Instalación y Uso](#-instalación-y-uso)
6.  [Tecnologías Utilizadas](#-tecnologías-utilizadas)
7.  [Dataset](#-dataset)
8.  [Autor](#️-autor)

---

### 🎯 Objetivos y Preguntas Analizadas

El análisis se centra en responder a las siguientes preguntas:

* **¿Qué plataformas han dominado el mercado?** Se analiza el total de ventas acumuladas por consola.
* **¿Cuáles son los juegos y géneros más exitosos?** Se identifican los títulos y categorías con mayor volumen de ventas.
* **¿Cómo ha sido la competencia histórica entre marcas?** Se realiza un análisis temporal de la rivalidad entre Sony y Nintendo para observar sus ciclos de éxito.
* **¿Son las diferencias entre marcas estadísticamente significativas?** Se utiliza la prueba U de Mann-Whitney para validar si la diferencia en las distribuciones de ventas es real o producto del azar.

---

### 🔬 Metodología

El proyecto sigue un flujo de trabajo de análisis de datos de principio a fin:

1.  **Obtención de Datos**: Se extrajeron datos de ventas de videojuegos de **vgchartz.com** mediante técnicas de **Web Scraping** con Pandas.
2.  **Limpieza y Preprocesamiento**: Se realizó una limpieza exhaustiva de los datos, manejando valores nulos, convirtiendo tipos de datos (ej. "31.37m" a numérico) y estandarizando la información.
3.  **Ingeniería de Características (Feature Engineering)**: Se creó la columna `Marca` para agrupar las consolas por compañía (Sony/Nintendo) y facilitar la comparación directa.
4.  **Análisis y Visualización**: Se utilizaron **Seaborn** y **Matplotlib** para crear visualizaciones comparativas (barras, cajas, violín, líneas, etc.) que respondieran a las preguntas del análisis.
5.  **Validación Estadística**: Se aplicó la prueba de hipótesis no paramétrica **U de Mann-Whitney** con **SciPy** para dar rigor estadístico a las conclusiones.

---

### 💡 Conclusiones Principales

1.  🏆 **Dominio en "Grandes Éxitos" para Nintendo:** El top 10 de juegos más vendidos de la historia está dominado casi en su totalidad por títulos de Nintendo (ej. *Wii Sports*, *Pokémon*, *Mario*).
2.  📈 **Liderazgo en Volumen para Sony:** En las consolas de sobremesa, Sony consistentemente ha vendido un mayor volumen de software acumulado, destacando el éxito arrollador de la PlayStation 2.
3.  🎮 **Nintendo, Rey de las Portátiles:** En el mercado portátil, el dominio de Nintendo es absoluto, con la DS y 3DS superando ampliamente a la PSP y PS Vita.
4.  📊 **Diferencia Estadística Validada:** La prueba U de Mann-Whitney confirmó con un **p-valor < 0.05** que existe una diferencia estadísticamente significativa entre las distribuciones de ventas de Sony y Nintendo.

---

### 📊 Visualizaciones Destacadas

A continuación se muestran algunos de los gráficos generados durante el análisis.

| Evolución Anual: Sony vs. Nintendo | Ventas Totales por Plataforma |
| :---: | :---: |
| ![Gráfico de Líneas de Ventas Anuales](https://raw.githubusercontent.com/EduardoLimones/EDA/main/EDA/src/graficos/Graficolineal.png) | ![Gráfico de Lollipop](https://raw.githubusercontent.com/EduardoLimones/EDA/main/EDA/src/graficos/ventaconsolaslollipop.png) |
| **Comparativa Generación: PS2 vs. GC** | **Distribución de Géneros** |
| ![Comparativa PS2 vs GC](https://raw.githubusercontent.com/EduardoLimones/EDA/main/EDA/src/graficos/GCvsPS2.png) | ![Gráfico de Géneros](https://raw.githubusercontent.com/EduardoLimones/EDA/main/EDA/src/graficos/generos.png) |

---

### 🚀 Instalación y Uso

Para ejecutar este análisis en tu entorno local, sigue estos pasos:

1.  **Clona el repositorio:**
    ```bash
    git clone [https://github.com/EduardoLimones/EDA.git](https://github.com/EduardoLimones/EDA.git)
    cd EDA
    ```

2.  **Instala las dependencias:**
    ```bash
    pip install pandas matplotlib seaborn scipy jupyter
    ```

3.  **Ejecuta el Notebook:**
    Abre el archivo `memoria.ipynb` con Jupyter Notebook para ver y ejecutar el análisis completo.
    ```bash
    jupyter notebook memoria.ipynb
    ```

---

### 🛠️ Tecnologías Utilizadas

* **Lenguaje**: Python 3.10
* **Librerías de Análisis**: Pandas, NumPy
* **Librerías de Visualización**: Matplotlib, Seaborn
* **Librerías de Estadística**: SciPy
* **Entorno de Trabajo**: Jupyter Notebook

---

### 💾 Dataset

El conjunto de datos principal fue construido mediante Web Scraping y contiene información sobre las ventas de videojuegos con las siguientes columnas clave:
`Nombre`, `Plataforma`, `Fecha Salida`, `Género`, `Ventas Norte América`, `Ventas Europa`, `Ventas Japón`, `Ventas Otros` y `Ventas Totales`.

---

### ✍️ Autor

* **Eduardo José Limones Contreras**
* **LinkedIn**: [Eduardo José Limones Contreras](https://www.linkedin.com/in/eduardo-jos%C3%A9-limones-contreras-b1348677/)
* **GitHub**: [@EduardoLimones](https://github.com/EduardoLimones)
