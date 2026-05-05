# 🌫️ Análisis de Calidad del Aire PM2.5 y PM10 — Área Metropolitana NY-NJ (2020–2026)

Proyecto de análisis de datos sobre la evolución de la calidad del aire en el área metropolitana de Nueva York–Newark–Jersey City, usando datos diarios de monitoreo de la EPA entre 2020 y 2026.

---

## 📌 Descripción del Proyecto

Este proyecto analiza la evolución de dos contaminantes atmosféricos regulados por la Agencia de Protección Ambiental de EE.UU. (EPA):

- **PM2.5** — Partículas finas (≤ 2,5 µm). Pueden penetrar en los pulmones y pasar al torrente sanguíneo. Límite diario EPA: 35 µg/m³.
- **PM10** — Partículas más gruesas (≤ 10 µm). Irritan las vías respiratorias superiores. Límite diario EPA: 150 µg/m³.

### Preguntas de Investigación
1. ¿Cómo han evolucionado los niveles de PM2.5 y PM10 a lo largo del tiempo?
2. ¿Existen patrones estacionales consistentes en las concentraciones?
3. ¿Se pueden identificar y caracterizar episodios de alta contaminación?
4. ¿Qué relación existe entre PM2.5 y PM10?

---

## 📊 Principales Hallazgos

- **Patrón estacional claro**: el PM2.5 alcanza sus picos en invierno (dic–ene) debido a las emisiones de calefacción y a las condiciones atmosféricas que atrapan los contaminantes cerca del suelo.
- **Anomalía de 2023**: el **7 de junio de 2023** se registró un pico de PM2.5 de ~100 µg/m³ en la media diaria de la ciudad — diez veces la media anual — causado por el humo de los incendios forestales de Quebec (Canadá), transportado por los patrones de viento de un sistema de bajas presiones sobre el Golfo de Maine.
- **Buena calidad del aire en general**: solo 5 días en todo el periodo 2020–2026 superaron el umbral de PM2.5 de la EPA, todos concentrados en 2021 y 2023.
- **Correlación moderada PM2.5–PM10**: comparten fuentes comunes pero reaccionan de forma diferente ante eventos episódicos como incendios.

---

## 🗂️ Estructura del Repositorio

```
air-quality-nyc/
├── air_quality_nyc.ipynb      # Notebook principal de análisis
├── README.md                  # Versión en inglés (GitHub)
├── README_ES.md               # Este archivo
├── environment.yml            # Entorno conda para reproducibilidad
└── data/
    ├── pm_2_5_2020_NewYork.csv
    ├── pm_2_5_2021_NewYork.csv
    ├── pm_2_5_2022_NewYork.csv
    ├── pm_2_5_2023_NewYork.csv
    ├── pm_2_5_2024_NewYork.csv
    ├── pm_2_5_2025_NewYork.csv
    ├── pm_2_5_2026_NewYork.csv
    ├── pm_10_2020_NewYork.csv
    ├── pm_10_2021_NewYork.csv
    ├── pm_10_2022_NewYork.csv
    ├── pm_10_2023_NewYork.csv
    ├── pm_10_2024_NewYork.csv
    └── pm_10_2025_NewYork.csv
```

> **Nota:** Los datos de PM2.5 cubren 2020–abril 2026. Los datos de PM10 cubren 2020–2025 (los datos de 2026 aún no estaban disponibles en la EPA en el momento de este análisis).

---

## 🛠️ Herramientas y Librerías

| Herramienta | Uso |
|-------------|-----|
| Python 3.11 | Lenguaje principal |
| pandas | Carga, limpieza y agregación de datos |
| numpy | Operaciones numéricas y regresión lineal |
| matplotlib | Gráficas estáticas de series temporales y scatter |
| seaborn | Heatmap y visualizaciones estilizadas |
| bokeh | Gráficas interactivas con hover y zoom |
| pathlib | Manejo de rutas de archivos |

---

## 🚀 Cómo Ejecutar

### 1. Clonar el repositorio
```bash
git clone https://github.com/TU_USUARIO/air-quality-nyc.git
cd air-quality-nyc
```

### 2. Crear y activar el entorno conda
```bash
conda env create -f environment.yml
conda activate air_quality
```

### 3. Lanzar Jupyter
```bash
jupyter notebook air_quality_nyc.ipynb
```

### 4. Ejecutar todas las celdas
En Jupyter: **Kernel > Restart & Run All**

---

## 📁 Fuente de Datos

Todos los datos se descargaron del **EPA Air Quality System (AQS) Data Mart**:
- 🔗 https://www.epa.gov/outdoor-air-quality-data

Los datos son públicos y de uso libre.

---

## 📚 Referencias

- Chen et al. (2023). *Canadian Wildfire Smoke and Asthma Syndrome Emergency Department Visits in New York City*. JAMA, 330(14), 1385–1387. https://pmc.ncbi.nlm.nih.gov/articles/PMC10514869/
- Communications Earth & Environment (2025). *Radiative cooling in New York/New Jersey metropolitan areas by wildfire particulate matter from the 2023 Canadian wildfires*. https://www.nature.com/articles/s43247-025-02214-3
- NYC Community Air Survey (2023). https://a816-dohbesp.nyc.gov/IndicatorPublic/data-features/nyccas/

---

## 👩‍💻 Autora

**Sheila Alonso** — Junior Data Analyst  
📧 sheila.alonso7@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/sheila-alonso-rodriguez)
