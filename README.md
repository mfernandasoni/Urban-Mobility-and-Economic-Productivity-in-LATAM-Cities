# Urban Mobility and Economic Productivity in LATAM Cities

🌐 [English](#english) | [Español](#español)

---

<a name="english"></a>
## 🇬🇧 English

An analysis of the relationship between traffic congestion and economic performance across Latin American cities.

### 1. Context / Problem
This was an individual project developed as part of the **TripleTen Data Analyst certificate program**. The project combined two data sources:

- `tomtom_traffic.csv`: real-time vehicular congestion and traffic condition data for cities around the world, monitored by TomTom, a global geolocation company. Each record corresponds to a specific update of a city's traffic status.
- `oecd_city_economy.csv`: annual indicators of urban economy, employment, pollution, and population compiled by the OECD (Organisation for Economic Cooperation and Development). Each record represents a city in a specific year.

The objective was to combine both datasets to understand how urban traffic efficiency relates to economic performance in Latin American cities, and to identify which cities represent priority cases for investment or further attention. The analysis was scoped to 2024 and covered 15 cities across Brazil, Colombia, Argentina, Peru, Mexico, Uruguay, and Chile.

### 2. My Contribution
I was responsible for the full analysis: data cleaning and transformation, exploratory analysis, trend visualization, and interpretation of results.

### 3. Process and Decisions
- **Dataset exploration:** I started by exploring both datasets independently to understand their structure, since they came from different sources (TomTom and OECD) with different granularities and formats.
- **Data cleaning and preparation:** I cleaned and standardized both datasets so they could be reliably combined and compared.
- **Year extraction and filtering:** Since the traffic dataset contains real-time updates and the OECD dataset is annual, I extracted the year from the traffic data and applied filters to align both sources on a comparable time basis.
- **Mobility data analysis and summarization:** I analyzed and summarized the traffic/congestion data at the city level before merging it with the economic data, to avoid distortions from mixing raw, high-frequency records with annual indicators.
- **Data merging:** I merged both datasets by city (and year) to build a single dataset that allowed traffic and economic indicators to be compared side by side.
- **Relationship analysis and visualization:** I focused the analysis on identifying whether a relationship existed between GDP per capita and traffic congestion, rather than assuming one — the data showed this relationship is not linear, which shaped how I framed the findings (highlighting specific city cases instead of a general trend).
- **Executive summary:** I closed the analysis with an executive summary highlighting the most actionable findings for decision-makers, rather than a full walkthrough of every metric.

### 4. Outcome / Learning
- Found that there is **no linear correlation** between GDP per capita and traffic congestion across the cities analyzed.
- Identified extreme cases that illustrate this lack of a simple relationship:
  - **Montevideo:** high GDP (~$18,000) with low congestion.
  - **Mexico City:** high GDP (~$15,000) with extreme congestion (2,833 min).
  - **Bogotá:** moderate GDP (~$11,000) with high congestion (1,141 min).
- Identified **Bogotá** as a priority city for transportation infrastructure investment, based on the combination of high traffic congestion, moderate economic productivity, and a significant potential population impact (11.3M inhabitants).

### 5. Tools Used
- Python (pandas, NumPy, Seaborn, Matplotlib)
- Jupyter Notebook

### 6. Evidence
- 📓 Analysis notebook: see repository
- 📊 Chart/visualization image: see repository
- 🗂️ Cleaned dataset: see repository

---
# Movilidad Urbana y Productividad Económica en Ciudades de América Latina

<a name="español"></a>
## 🇪🇸 Español

Un análisis de la relación entre la congestión de tráfico y el desempeño económico en ciudades de América Latina.

### 1. Contexto / Problema
Este fue un proyecto individual desarrollado como parte del **certificado de Data Analyst de TripleTen**. El proyecto combinó dos fuentes de datos:

- `tomtom_traffic.csv`: datos de congestión vehicular y condiciones de tráfico en tiempo real en distintas ciudades, monitoreadas por TomTom, empresa global de geolocalización. Cada registro corresponde a una actualización específica del estado del tráfico en una ciudad.
- `oecd_city_economy.csv`: indicadores anuales de economía urbana, empleo, contaminación y población, compilados por la OCDE (Organización para la Cooperación y el Desarrollo Económicos). Cada registro representa una ciudad en un año específico.

El objetivo fue combinar ambos datasets para entender cómo se relaciona la eficiencia del tráfico urbano con el desempeño económico en ciudades latinoamericanas, e identificar qué ciudades representan casos prioritarios para inversión o atención adicional. El análisis se limitó al año 2024 y abarcó 15 ciudades de Brasil, Colombia, Argentina, Perú, México, Uruguay y Chile.

### 2. Mi Contribución
Este fue un **proyecto individual**. Fui responsable de todo el análisis: limpieza y transformación de datos, análisis exploratorio, visualización de tendencias e interpretación de resultados.

### 3. Proceso y Decisiones
- **Exploración de datasets:** Comencé explorando ambos datasets de forma independiente para entender su estructura, ya que provenían de fuentes distintas (TomTom y OCDE) con diferentes granularidades y formatos.
- **Limpieza y preparación de datos:** Limpié y estandaricé ambos datasets para poder combinarlos y compararlos de forma confiable.
- **Extracción de año y filtros:** Dado que el dataset de tráfico contiene actualizaciones en tiempo real y el de la OCDE es anual, extraje el año de los datos de tráfico y apliqué filtros para alinear ambas fuentes en una base temporal comparable.
- **Análisis y resumen de datos de movilidad:** Analicé y resumí los datos de tráfico/congestión a nivel ciudad antes de combinarlos con los datos económicos, para evitar distorsiones al mezclar registros crudos y de alta frecuencia con indicadores anuales.
- **Combinación de datos (merge):** Combiné ambos datasets por ciudad (y año) para construir un único dataset que permitiera comparar indicadores de tráfico y económicos lado a lado.
- **Análisis de relación y visualización:** Enfoqué el análisis en identificar si existía una relación entre el PIB per cápita y la congestión de tráfico, en lugar de asumirla de antemano; los datos mostraron que esta relación no es lineal, lo cual definió cómo enmarqué los hallazgos (destacando casos específicos de ciudades en vez de una tendencia general).
- **Resumen ejecutivo:** Cerré el análisis con un resumen ejecutivo que destaca los hallazgos más accionables para la toma de decisiones, en lugar de un recorrido completo por cada métrica.

### 4. Resultado / Aprendizaje
- Se encontró que **no existe una correlación lineal** entre el PIB per cápita y la congestión de tráfico en las ciudades analizadas.
- Se identificaron casos extremos que ilustran esta falta de relación simple:
  - **Montevideo:** PIB alto (~$18,000) con baja congestión.
  - **Ciudad de México:** PIB alto (~$15,000) con congestión extrema (2,833 min).
  - **Bogotá:** PIB moderado (~$11,000) con alta congestión (1,141 min).
- Se identificó a **Bogotá** como ciudad prioritaria para inversión en infraestructura de transporte, con base en la combinación de alta congestión de tráfico, productividad económica moderada y un impacto poblacional potencial significativo (11.3M de habitantes).

### 5. Herramientas Utilizadas
- Python (pandas, NumPy, Seaborn, Matplotlib)
- Jupyter Notebook

### 6. Evidencias
- 📓 Notebook de análisis: ver repositorio
- 📊 Imagen de gráfica/visualización: ver repositorio
- 🗂️ Base de datos limpia: ver repositorio
