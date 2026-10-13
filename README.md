# 📱 ConnectaTel | Customer Analytics & Segmentation

### Turning Mobile Usage Data into Business Decisions 🚀

**¿Y si los datos de uso móvil pudieran revelar oportunidades para fidelizar clientes, optimizar planes y mejorar la estrategia comercial?**

Este proyecto de análisis exploratorio de datos (EDA) estudia el comportamiento de los clientes de **ConnectaTel en Latinoamérica**, con información de México y Colombia. A través de Python y técnicas de análisis estadístico, limpieza de datos y segmentación, transformamos datos sin procesar en insights que pueden orientar decisiones de negocio.

---

## 🎯 Business Objective

Analizar los patrones de consumo de los usuarios para comprender cómo utilizan los servicios de telefonía móvil, identificar comportamientos atípicos y descubrir oportunidades de segmentación, fidelización y optimización de planes.

## 🛠️ Tech Stack

- **Python** — análisis y procesamiento de datos.
- **Pandas** — limpieza, transformación y agregación de datasets.
- **NumPy** — operaciones numéricas y segmentación lógica.
- **Matplotlib & Seaborn** — visualización de distribuciones y detección de outliers.
- **Jupyter Notebook** — análisis exploratorio documentado y reproducible.

## 📂 Dataset Overview

El análisis integra tres fuentes de datos:

| Dataset | Descripción |
|---|---|
| `plans.csv` | Características, precios y límites de los planes Básico y Premium. |
| `users_latam.csv` | Información demográfica, ubicación, plan contratado y fechas de registro de los clientes. |
| `usage.csv` | Registros de llamadas y mensajes de los usuarios. |

El conjunto de clientes contiene **4.000 registros**, mientras que el historial de uso contiene **40.000 registros**.

## 🔍 Analytical Workflow

### 01. Data Exploration & Quality Assessment
Inspección de dimensiones, tipos de datos, valores nulos, inconsistencias y estadísticas descriptivas para comprender la estructura y confiabilidad de la información.

### 02. Data Cleaning
Tratamiento de valores centinela, estandarización de ciudades y revisión de fechas fuera del rango esperado. También se evaluaron los valores faltantes en duración de llamadas y longitud de mensajes, considerando las diferencias entre tipos de actividad.

### 03. Exploratory Data Analysis (EDA)
Análisis de distribuciones, medidas estadísticas y valores atípicos mediante histogramas, boxplots y el método del rango intercuartílico (IQR).

### 04. Customer Segmentation
Creación de dos dimensiones de segmentación:

- **Por uso:** Bajo uso, Uso medio y Alto uso.
- **Por edad:** Joven, Adulto y Adulto Mayor.

### 05. Business Insights
Interpretación de los patrones observados para formular recomendaciones orientadas a la activación, fidelización y comprensión del comportamiento de los clientes.

## 📊 Key Findings

**01 | Data quality matters.**  
Se identificaron valores faltantes en la ubicación de clientes, edades con valores centinela y fechas de registro posteriores a 2024. Su tratamiento permite construir una base más consistente para el análisis.

**02 | Medium usage dominates.**  
La segmentación preliminar muestra que el grupo de uso medio concentra aproximadamente 2.950 clientes, frente a unos 780 de bajo uso y 280 de alto uso.

**03 | Adults represent the largest age segment.**  
El grupo de adultos reúne aproximadamente 2.020 clientes, seguido por los adultos mayores, con unos 1.220, y los jóvenes, con cerca de 760.

**04 | Outliers reveal opportunities for investigation.**  
Se detectaron consumos extremos en mensajes, llamadas y minutos de llamadas. Estos registros requieren revisión para distinguir comportamientos legítimos de posibles errores de registro.

*Las cifras de segmentación son aproximadas y corresponden a la exploración realizada en el notebook.*

## 💡 Strategic Recommendations

- **Activate low-usage customers:** diseñar campañas de comunicación y beneficios para incentivar el uso de los servicios.
- **Understand high-usage customers:** evaluar sus patrones de consumo y la adecuación de sus planes actuales.
- **Personalize customer engagement:** explorar diferencias de comportamiento por edad y tipo de plan.
- **Strengthen data quality:** establecer controles para detectar valores centinela, fechas inconsistentes y registros incompletos.
- **Validate before acting:** investigar los valores atípicos antes de excluirlos, para no perder información relevante sobre el comportamiento real de los clientes.

## 📈 Business Impact

Este proyecto demuestra cómo el análisis de datos puede conectar la calidad de la información con decisiones comerciales concretas. La segmentación permite formular hipótesis sobre oportunidades de fidelización y personalización, que deberán validarse con métricas de consumo, ingresos y retención.

## ▶️ How to Explore the Project

1. Descarga o clona este repositorio.
2. Abre el notebook `S7 Version-Estudiante-Project-ConnectaTel.ipynb` en Jupyter Notebook.
3. Asegúrate de disponer de los tres archivos CSV en la carpeta `datasets/`.
4. Ejecuta las celdas en orden para reproducir el análisis y explorar los resultados.

## 👩‍💻 About This Project

Proyecto desarrollado como parte del **Data Analysis Bootcamp de TripleTen**, Sprint 7, aplicando habilidades de análisis exploratorio, limpieza de datos, estadística descriptiva, visualización y segmentación de clientes.

