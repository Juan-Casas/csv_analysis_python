# csv_analysis_python
# 📊 Análisis de Datos de Autos Usados

## 🧠 Caso de negocio

Este proyecto tiene como objetivo analizar un conjunto de datos de autos usados para obtener información clave que pueda servir en la toma de decisiones comerciales, como estrategias de precios, oferta por marca/modelo y análisis del estado de los vehículos más vendidos.

## 📦 Dataset utilizado

El dataset contiene registros de autos vendidos en distintos estados de EE.UU., incluyendo detalles como:

- Año, marca y modelo
- Tipo de carrocería y transmisión
- Condición, odómetro, color, vendedor
- Precio de venta (`sellingprice`) y precio estimado (`mmr`)
- Fecha de venta (`saledate`)

## 🔧 Proceso técnico

### 1. Limpieza de datos (`ETL`)
- Eliminación de registros con valores nulos irrelevantes
- Conversión de fechas y estandarización de texto a minúsculas
- Traducción de nombres de columnas al español para mejorar la legibilidad

### 2. Análisis con KPIs
Se calcularon los siguientes indicadores:

- Precio promedio y mediano por marca
- Top 5 marcas y modelos más frecuentes
- Tasa de venta según condición
- Diferencia entre precio estimado y real (`mmr` vs `sellingprice`)
- Distribución del odómetro por año

### 3. Visualizaciones generadas
Se utilizaron `matplotlib` y `seaborn` para los siguientes gráficos:

- Distribución del precio de venta
- Comparación entre `mmr` y `sellingprice`
- Modelos más vendidos
- Condición promedio por marca
- Tendencia de ventas por año de vehículo

### 4. Exportación
El dataset limpio se exportó a un archivo CSV codificado en UTF-8-SIG para garantizar compatibilidad con Excel:
