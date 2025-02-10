# Proyecto de Análisis de Datos de SpaceX

## 📌 Descripción
Este proyecto analiza los lanzamientos de cohetes de SpaceX para identificar los factores que influyen en el éxito de los aterrizajes de la primera etapa. Incluye recopilación de datos, limpieza, análisis exploratorio, visualización y análisis predictivo para comprender y predecir el éxito de los innovadores métodos de recuperación de cohetes de SpaceX.

<div align="center"> 
  <img src="./Space X.jpg" alt="Space X" width="80%"/> 
</div>


## 📂 Estructura del Repositorio
El repositorio incluye los siguientes archivos y notebooks clave:

1. **01_SpaceX_Data_Collection_API.ipynb**:
   - Recopila datos de lanzamientos de cohetes desde la API REST de SpaceX.
   - Procesa las respuestas JSON y las convierte en DataFrames estructurados.
   - Filtra los datos para incluir solo lanzamientos del Falcon 9.

2. **02_SpaceX_Web_Scraping.ipynb**:
   - Extrae datos adicionales de lanzamientos desde Wikipedia.
   - Analiza tablas HTML usando BeautifulSoup y exporta los datos limpios a CSV.

3. **03_SpaceX_Data_Wrangling.ipynb**:
   - Limpia y preprocesa el conjunto de datos combinado.
   - Maneja valores faltantes, filtra columnas innecesarias y aplica codificación one-hot.

4. **04_SpaceX_EDA_SQL.ipynb**:
   - Realiza análisis exploratorio de datos (EDA) usando consultas SQL.
   - Calcula métricas como masa de carga útil, tasas de éxito y rendimiento de los sitios de lanzamiento.

5. **05_SpaceX_EDA_Data_Visualization.ipynb**:
   - Visualiza datos usando matplotlib y seaborn.
   - Analiza la masa de carga útil, las tasas de éxito por órbita y las tendencias a lo largo del tiempo.

6. **06_SpaceX_Interactive_Visual_Analytics_Folium.ipynb**:
   - Crea mapas interactivos usando Folium.
   - Muestra sitios de lanzamiento, tasas de éxito y distancias a proximidades clave (costas, ferrocarriles, autopistas).

7. **08_SpaceX_Predictive_Analytics.ipynb**:
   - Construye modelos de machine learning (Regresión Logística, SVM, Árbol de Decisión, KNN) para predecir el éxito de aterrizajes.
   - Evalúa los modelos usando métricas como precisión, puntaje F1 y matrices de confusión.

8. **SpaceX.pdf**:
   - Proporciona un informe detallado que resume la metodología, los resultados y las conclusiones del análisis.

## 🛠 Metodologías
1. **Recopilación de Datos**:
   - API REST de SpaceX para datos de lanzamientos.
   - Web scraping para información adicional.
2. **Limpieza de Datos**:
   - Limpieza y preparación del conjunto de datos para el análisis.
3. **EDA**:
   - Técnicas de SQL y visualización para descubrir patrones y tendencias.
4. **Visualizaciones Interactivas**:
   - Folium y Plotly Dash para la exploración interactiva de datos.
5. **Análisis Predictivo**:
   - Modelos de machine learning para predecir los resultados de aterrizaje de la primera etapa.

## 🚀 Instalación
1. Clona el repositorio:
   ```bash
   git clone <repository_url>
   cd <repository_folder>
   ```
2. Instala las dependencias:
   ```bash
   pip install -r requirements.txt
   ```
3. Configura las variables de entorno en un archivo `.env`:
   ```env
   SPACEX_API_URL=tu_url_de_api_de_spacex
   IBM_WATSON_API_KEY=tu_clave_api_de_ibm_watson
   IBM_WATSON_URL=tu_url_de_ibm_watson
   ```

## 📑 Cómo Usar
1. Ejecuta los notebooks en el orden proporcionado, comenzando con **01_SpaceX_Data_Collection_API.ipynb**.
2. Asegúrate de que las claves API estén correctamente configuradas en el archivo `.env`.
3. Visualiza los resultados e interactúa con los dashboards en **06_SpaceX_Interactive_Visual_Analytics_Folium.ipynb**.

## 🎯 Principales Resultados
- Las tasas de éxito han mejorado significativamente con el tiempo.
- KSC LC-39A es el sitio de lanzamiento más exitoso.
- Las cargas útiles pesadas tienden a tener mayores tasas de éxito.
- Los modelos de Árbol de Decisión superan ligeramente a otros modelos de ML para predecir aterrizajes.

## 📜 Licencia
Este proyecto está licenciado bajo la Licencia MIT. Útilízalo libremente para aprendizaje y experimentación.

