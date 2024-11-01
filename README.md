
# Análisis del Rendimiento de Ventas de SisconPC (2022-2023)

Este repositorio contiene el código y análisis de datos de un trabajo final de grado realizado en la Universidad de las Américas, cuyo objetivo es analizar el rendimiento de ventas de la empresa SisconPC durante el periodo 2022-2023. Utilizando modelos de predicción de ventas, segmentación de clientes y optimización de precios, este proyecto busca maximizar la rentabilidad y mejorar la planificación estratégica de la empresa.

## Contenido

- `TesisHV.ipynb`: Jupyter Notebook que contiene el código de limpieza, análisis y modelado de datos.
- `/data`: Directorio que contiene los datos de ventas utilizados para el análisis (no incluido en el repositorio público).
- `/images`: Gráficos y visualizaciones generados a partir del análisis.

## Estructura del Proyecto

### 1. Recolección y Limpieza de Datos
   - Se recogen los datos históricos de ventas proporcionados por SisconPC.
   - Se realiza una limpieza de duplicados y valores faltantes, además de una normalización básica.

### 2. Identificación y Descripción de Variables
   - Las variables del dataset son descritas y categorizadas para su posterior análisis, incluyendo variables como `PVP`, `Costo Unitario`, `Cantidad` y `Total`.

### 3. Análisis Exploratorio de Datos (EDA)
   - Visualización de patrones y tendencias de las ventas mediante gráficos de línea, dispersión y matrices de correlación.

### 4. Transformación Logarítmica
   - Aplicación de transformaciones logarítmicas en variables para mejorar la estabilidad de los datos y facilitar el modelado.

### 5. Modelado Estadístico
   - **ARIMA y SARIMA**: Implementación de estos modelos para la predicción de ventas, con comparación entre ambos modelos en cuanto a precisión y adecuación.
   - **Segmentación de Clientes con K-Means**: Segmentación basada en ventas totales y frecuencia de compras, evaluando la efectividad con los métodos del codo y silhouette.
   - **Regresión Lineal para Optimización de Precios**: Modelos de regresión que examinan el impacto de factores clave en el precio de venta al público (PVP).

## Requisitos

- Python 3.x
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, `seaborn`, `statsmodels`, `sklearn`, `missingno`

Para instalar las bibliotecas necesarias:

```bash
pip install pandas numpy matplotlib seaborn statsmodels scikit-learn missingno
```

## Ejecución

1. Clona este repositorio:

   ```bash
   git clone https://github.com/usuario/proyecto_sisconpc.git
   cd proyecto_sisconpc
   ```

2. Abre el archivo `TesisHV.ipynb` en Jupyter Notebook o Jupyter Lab y sigue la secuencia de celdas.

## Resultados

El análisis arrojó resultados clave sobre los patrones de venta y la segmentación de clientes en SisconPC. Las recomendaciones estratégicas incluyen ajustar los precios dinámicamente, implementar campañas de marketing específicas para cada segmento y mejorar la planificación de inventarios.

## Contribuciones

Este proyecto fue desarrollado como parte de la tesis de grado en la Universidad de las Américas. Agradecimientos al profesor Ing. Manuel Eugenio Morocho y al equipo de SisconPC por su apoyo en la provisión de datos.

## Licencia

Este proyecto es para fines académicos y no comerciales. Todos los derechos son reservados a sus autores y la Universidad de las Américas.
