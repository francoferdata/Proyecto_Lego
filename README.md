# Análisis Exploratorio de la Historia de LEGO (EDA)

Este proyecto realiza un Análisis Exploratorio de Datos (EDA) sobre el catálogo histórico de sets de LEGO, utilizando datos públicos de Rebrickable.

El objetivo principal es entender cómo ha evolucionado LEGO como marca y producto, respondiendo a preguntas como:

¿Cómo ha crecido el catálogo de sets a lo largo del tiempo?
¿Qué temas han sido más populares y persistentes?
¿Los sets se han vuelto más complejos con el tiempo?


---

## Stack Tecnológico

* **Python**
* **Pandas:** Para la carga, limpieza, transformación y unión de datos (`pd.merge`).

 * **NumPy:** Para cálculos estadísticos y métricas descriptivas.
 
* **Matplotlib:** Para la visualización de tendencias y distribuciones.
---

## Flujo del Análisis

El notebook de Jupyter (`proyecto-lego.ipynb`) sigue una estructura lógica y progresiva:

**Carga y Limpieza de Datos:**  
   Se cargaron los archivos `lego_sets.csv` y `parent_themes.csv`. Se revisaron valores nulos (42% en `num_parts`), se eliminaron duplicados (152) y se trataron datos atípicos (sets con 0 piezas).

**Análisis Temporal del Catálogo:**  
   Se analizó la variable `year` para observar el crecimiento anual en cantidad de sets y la complejidad promedio (media de `num_parts`).

**Fusión y Análisis de Temáticas:**  
   Se realizó un **join (`pd.merge`)** entre los sets y sus temas (`parent_themes.csv`) para identificar las temáticas más prolíficas (ej. "Star Wars", "Technic").
   
---

## Hallazgos Clave

**Crecimiento Exponencial del Catálogo:**  
El análisis de la producción anual de sets muestra que LEGO pasó de ser un fabricante de nicho a un gigante global. El crecimiento es especialmente dramático desde mediados de la década de 1990, alcanzando su punto máximo en 2014.

<img width="503" height="301" alt="Captura de pantalla 2025-11-01 204821" src="https://github.com/user-attachments/assets/f0f92b64-8907-46d5-b1e7-365e355494d7" />




**Los Sets se han Vuelto Más Complejos:**  
   Junto con el aumento en la *cantidad* de sets, también ha aumentado su *complejidad*. El número promedio de piezas por set ha mostrado una clara tendencia al alza, especialmente desde el año 2000, indicando que LEGO está produciendo sets más grandes y detallados.

<img width="504" height="245" alt="Captura de pantalla 2025-11-01 204931" src="https://github.com/user-attachments/assets/e4dd1510-7324-44a5-a209-753f27d0b587" />


  

**Star Wars marcó un Punto de Inflexión (1999):**  
   El análisis de temáticas individuales revela que "Star Wars" es una de las categorías más importantes. Su lanzamiento en 1999 no solo creó una línea de productos masiva y duradera, sino que su cronología coincide perfectamente con el inicio del crecimiento exponencial tanto en el volumen como en la complejidad de los sets de LEGO.

   
<img width="502" height="252" alt="Captura de pantalla 2025-11-01 204949" src="https://github.com/user-attachments/assets/31417a41-9025-4090-97fa-8f5aed07234d" />



