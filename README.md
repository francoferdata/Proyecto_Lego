# Análisis del Catálogo Histórico de LEGO

## Introducción
Este proyecto presenta un **análisis exploratorio de datos (EDA)** sobre un dataset histórico de sets de LEGO.  
El objetivo principal es identificar **tendencias en la evolución del catálogo**, con foco en el impacto de las **temáticas licenciadas** como *Star Wars*.  

### Datasets utilizados
- **lego_sets.csv** → Información de cada set (número, nombre, año, piezas, temática).  
- **parent_themes.csv** → Describe las temáticas principales e indica si son licenciadas.  

---

## Stack Tecnológico
- **Lenguaje:** Python  
- **Librerías:** Pandas, Matplotlib, Seaborn  
- **Entorno:** Jupyter Notebook  

---

## Fases del Análisis
1. **Calidad y Limpieza de Datos** → Detección y manejo de nulos, duplicados y outliers.  
2. **Análisis Temporal** → Evolución del número y tamaño de sets por año.  
3. **Temática Star Wars** → Estudio de su representatividad y evolución histórica.  
4. **Sets Licenciados vs. No Licenciados** → Comparación de impacto en el catálogo.  

---

## Preguntas y Hallazgos Clave

### 1️⃣ Calidad de Datos
- **¿Existen valores nulos o duplicados?**  
  > La columna `num_parts` tiene un **42 % de nulos**. Se eliminaron **153 duplicados** en `set_num`.  

- **¿Hay valores atípicos?**  
  > Distribución sesgada: la mayoría de los sets tiene **< 200 piezas**, pero existen outliers con más de **5000 piezas** (ejemplo: *Taj Mahal – 5922 piezas*).  

---

### 2️⃣ Análisis Temporal
- **¿Cómo ha evolucionado el número de sets por año?**  
  > Crecimiento **exponencial desde 1990**, con un máximo en **2014 (732 sets)**.  

- **¿Ha cambiado el tamaño promedio?**  
  > Sí, los sets modernos son **más grandes y complejos** desde el año 2000.  

---

### 3️⃣ Star Wars
- **¿Qué proporción del catálogo representa?**  
  > Aproximadamente el **5.1 % del total**, siendo la licencia más importante.  

- **¿Cómo evolucionó?**  
  > Desde su debut en **1999**, supera los **600 sets**, consolidándose como la colaboración más exitosa.  

---

### 4️⃣ Licenciados vs. No Licenciados
- **¿Qué porcentaje son licenciados?**  
  > Solo el **11.1 % del catálogo**; el resto son creaciones originales.  

- **¿Cómo creció esa proporción?**  
  > A partir de **1999** aumentó sostenidamente, impulsando el éxito comercial de LEGO.  

---

## Conclusión
La introducción de **licencias** (especialmente *Star Wars*) en **1999** fue un **punto de inflexión** que cambió el rumbo de LEGO.  
Aunque los sets originales siguen dominando, los licenciados aportaron **complejidad, variedad y crecimiento sostenido**
