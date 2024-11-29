# Análisis Exploratorio de Datos (EDA) para el Dataset de Energías Renovables

Este proyecto realiza un análisis exploratorio de datos (EDA) sobre un conjunto de datos relacionado con plantas energéticas y sus características. El objetivo es limpiar, explorar y visualizar el dataset para comprender mejor las tendencias, patrones y relaciones en los datos. Además, se aplican técnicas de imputación de datos faltantes, análisis de valores atípicos, codificación de variables categóricas y reducción de dimensionalidad mediante PCA.

## Requisitos

Este proyecto requiere las siguientes librerías de Python:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`

Instala las librerías necesarias con el siguiente comando:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn


Descripción del Dataset
El dataset contiene información sobre diversas plantas energéticas, con las siguientes características:

Planta Energética: Nombre de la planta.
Tipo de Energía: Tipo de energía generada (eólica, solar, hidráulica, etc.).
Nivel de Democratización Energética: Nivel de accesibilidad de la energía generada.
Región: Localización geográfica de la planta.
Número de Comunidades Energéticas: Cantidad de comunidades que se benefician de la planta.
Número de Proyectos en Marcha: Cantidad de proyectos energéticos en curso.
Capacidad Generada (MW): Potencia generada por la planta.
Reducción de CO2 (toneladas): Estimación de reducción de emisiones de CO2.
Costo de Producción ($/MW): Costo de producción de energía.
Año de Instalación: Año en que la planta fue instalada.
Rentabilidad en 10 años: Indicador de rentabilidad (1 = Rentable, 0 = No rentable).
Pasos Realizados en el Análisis
1. Carga de Datos
Se carga el dataset utilizando pandas.read_csv() y se inspeccionan las primeras filas para comprender su estructura.

2. Exploración Inicial del DataFrame
Se inspeccionan los tipos de datos, valores únicos, y se realiza un análisis básico de estadísticas descriptivas. Además, se identifican las columnas con valores nulos.

3. Identificación y Manejo de Valores Faltantes
Se aplican técnicas de imputación para completar los datos faltantes. Para los datos numéricos se usa la mediana o la media, y para los datos categóricos se usa la moda. También se manejan los valores atípicos utilizando gráficos de cajas (boxplots).

4. Estadísticas Descriptivas
Se calculan estadísticas descriptivas tanto para las variables cuantitativas como cualitativas del dataset. Esto incluye medidas como la mediana, moda, varianza, y la distribución de las variables categóricas.

5. Visualización de Datos
Se realizan diferentes visualizaciones, incluyendo histogramas, gráficos de barras y gráficos de dispersión, para entender mejor la distribución y las relaciones entre las variables del dataset.

6. Codificación de Variables Categóricas
Se aplican técnicas de codificación como One-Hot Encoding, Label Encoding y Ordinal Encoding a las variables categóricas para prepararlas para modelos predictivos.

7. Correlación de Variables
Se calcula y visualiza la matriz de correlación entre las variables del dataset para entender las relaciones lineales entre ellas. Se utiliza un mapa de calor (heatmap) para mostrar las correlaciones de forma visual.

8. Reducción de Dimensionalidad con PCA
Se utiliza el Análisis de Componentes Principales (PCA) para reducir la dimensionalidad de los datos y proyectarlos en dos componentes principales (PC1 y PC2), lo que facilita la visualización y el análisis de patrones.

Resultados
Las visualizaciones y estadísticas descriptivas obtenidas durante el análisis revelan patrones y relaciones clave en los datos, lo que puede ser útil para decisiones sobre proyectos energéticos y la planificación de futuras instalaciones.

Ejemplos de Resultados:
Distribución de los Tipos de Energía: Identificación de los tipos de energía más comunes en el dataset.
Número de Proyectos en Marcha: Distribución de los proyectos y su relación con la rentabilidad.
Correlación entre la Capacidad Generada y la Reducción de CO2: Exploración de la relación entre la capacidad de generación de energía y la cantidad de CO2 reducida.
Conclusiones
El análisis exploratorio de datos proporciona una visión detallada de las características de las plantas energéticas, las relaciones entre variables y los posibles valores atípicos o faltantes. Las técnicas de imputación y la reducción de dimensionalidad con PCA ayudan a mejorar la calidad y la comprensión de los datos, lo que puede ser útil para proyectos futuros de energía renovable.
