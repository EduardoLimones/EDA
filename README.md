# 📊 Análisis Exploratorio de Ventas de Videojuegos

Este proyecto es un Análisis Exploratorio de Datos (EDA) sobre un conjunto de datos de ventas de videojuegos. El objetivo es descubrir patrones, comparar el rendimiento de diferentes plataformas y géneros, y visualizar las tendencias del mercado a lo largo del tiempo.

---

## 🎯 Objetivos y Preguntas Analizadas

El análisis se centra en responder a las siguientes preguntas:

* **¿Qué plataformas han dominado el mercado?** Se analiza el total de ventas acumuladas por consola.
* **¿Cómo se distribuyen las ventas de los juegos?** Se investiga si la mayoría de los juegos son éxitos modestos o si el mercado está dominado por unos pocos grandes éxitos (análisis de la "cola larga").
* **¿Cómo ha sido la competencia histórica entre marcas?** Se realiza un análisis temporal de la rivalidad entre Sony y Nintendo para observar sus ciclos de vida y su impacto mutuo.
* **¿Son las diferencias entre marcas estadísticamente significativas?** Se utiliza la prueba U de Mann-Whitney para validar si la diferencia en las distribuciones de ventas es real o producto del azar.

---

## 💡 Conclusiones Principales

1.  **Dominancia de Plataformas Clave:** Consolas como la PlayStation 2, Nintendo DS y Nintendo 3DS muestran una clara dominancia en términos de ventas totales de juegos acumuladas.
2.  **Distribución de Ventas Asimétrica:** El mercado sigue un patrón de "cola larga", donde una gran mayoría de juegos tiene ventas modestas y un pequeño número de títulos de gran éxito (outliers) representa una porción significativa de las ventas totales.
3.  **Fuerte Rivalidad Temporal:** El análisis de series temporales muestra una correlación inversa en los ciclos de éxito entre Sony y Nintendo, sugiriendo una competencia directa por el mercado.
4.  **Diferencia Estadística Validada:** La prueba U de Mann-Whitney confirma que existe una diferencia estadísticamente significativa entre las distribuciones de ventas de los juegos de Sony y Nintendo.

---

## 📊 Visualizaciones Destacadas

A continuación se muestran algunos de los gráficos generados durante el análisis.

**1. Evolución Anual de Ventas: Sony vs. Nintendo**
![Gráfico de Líneas de Ventas Anuales](C:\Users\eduar\Desktop\EDA\src\graficos\Graficolineal.png)

**2. Comparativa de Ventas Totales por Plataforma**
![Gráfico de Barras o Lollipop](C:\Users\eduar\Desktop\EDA\src\graficos\ventaconsolaslollipop.png)

---

## 🛠️ Tecnologías Utilizadas

* **Python 3.10.11**
* **Pandas**: Para la manipulación y limpieza de datos.
* **Matplotlib**: Para la creación de gráficos base.
* **Seaborn**: Para la visualización estadística avanzada.
* **SciPy**: Para la ejecución de pruebas estadísticas (U de Mann-Whitney).
* **Jupyter Notebook**: Como entorno de trabajo para el análisis.

---

## 💾 Dataset

El conjunto de datos utilizado contiene información sobre las ventas de videojuegos, incluyendo las siguientes columnas:
`Nombre`, `Plataforma`, `Año de Lanzamiento`, `Género`, `Ventas Norte América`, `Ventas Europa`, `Ventas Japón`, `Ventas Otros` y `Ventas Globales`.

---

## 🚀 Cómo Empezar

Para ejecutar este análisis en tu propio entorno, sigue estos pasos:

1.  Clona el repositorio:
    ```sh
    git clone [[https://m.youtube.com/watch?v=KrJwqsuhZ8U&pp=0gcJCYUJAYcqIYzv](https://github.com/EduardoLimones/EDA.git)]([https://m.youtube.com/watch?v=KrJwqsuhZ8U&pp=0gcJCYUJAYcqIYzv](https://github.com/EduardoLimones/EDA.git))
    ```
2.  Navega al directorio del proyecto:
    ```sh
    cd [EDA]
    ```
3.  Instala las dependencias necesarias:
    ```sh
    pip install -r requirements.txt
    ```

4.  Abre y ejecuta el notebook `memoria.ipynb`.

---

## ✍️ Autor

* **Eduardo José Limones Contreras**
* **LinkedIn**: [[Enlace a perfil de LinkedIn](https://www.linkedin.com/in/eduardo-jos%C3%A9-limones-contreras-b1348677/)]
* **GitHub**: [[Enlace a  perfil de GitHub](https://github.com/EduardoLimones)]
