# 🌫️ PM2.5 and PM10 Air Quality Analysis — NY-NJ Metropolitan Area (2020–2026)

A data analysis project exploring particulate matter air quality trends in the New York–Newark–Jersey City metropolitan area, using daily EPA monitoring data from 2020 to 2026.

---

## 📌 Project Overview

This project analyses the evolution of two atmospheric pollutants regulated by the U.S. Environmental Protection Agency (EPA):

- **PM2.5** — Fine particulate matter (≤ 2.5 µm). Can penetrate deep into the lungs and enter the bloodstream. EPA 24-hour limit: 35 µg/m³.
- **PM10** — Coarser particles (≤ 10 µm). Irritate the upper respiratory tract. EPA 24-hour limit: 150 µg/m³.

### Research Questions
1. How have PM2.5 and PM10 levels changed over time?
2. Are there consistent seasonal patterns in pollutant concentrations?
3. Can episodes of high pollution be identified and characterised?
4. What is the relationship between PM2.5 and PM10?

---

## 📊 Key Findings

- **Clear seasonal pattern**: PM2.5 peaks in winter (Dec–Jan) driven by heating emissions and atmospheric conditions that trap pollutants near ground level.
- **2023 anomaly**: A major pollution spike occurred on **7 June 2023**, reaching a city-wide PM2.5 daily mean of ~100 µg/m³ — 10 times the annual average — caused by wildfire smoke from Quebec, Canada transported by wind patterns from a low-pressure system over the Gulf of Maine.
- **Overall good air quality**: Only 5 days across the entire 2020–2026 period exceeded the EPA PM2.5 threshold, all concentrated in 2021 and 2023.
- **Moderate PM2.5–PM10 correlation**: They share common sources but react differently to episodic events like wildfires.

---

## 🗂️ Repository Structure

```
air-quality-nyc/
├── air_quality_nyc.ipynb      # Main analysis notebook
├── README.md                  # This file
├── environment.yml            # Conda environment for reproducibility
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

> **Note:** PM2.5 data covers 2020–April 2026. PM10 data covers 2020–2025 (2026 data not yet available from EPA at the time of this analysis).

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python 3.11 | Core language |
| pandas | Data loading, cleaning and aggregation |
| numpy | Numerical operations and linear regression |
| matplotlib | Static time series and scatter charts |
| seaborn | Heatmap and styled visualisations |
| bokeh | Interactive charts with hover and zoom |
| pathlib | File path handling |

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/YOUR_USERNAME/air-quality-nyc.git
cd air-quality-nyc
```

### 2. Create and activate the conda environment
```bash
conda env create -f environment.yml
conda activate air_quality
```

### 3. Launch Jupyter
```bash
jupyter notebook air_quality_nyc.ipynb
```

### 4. Run all cells
In Jupyter: **Kernel > Restart & Run All**

---

## 📁 Data Source

All data was downloaded from the **U.S. EPA Air Quality System (AQS) Data Mart**:
- 🔗 https://www.epa.gov/outdoor-air-quality-data

Data is publicly available and free to use.

---

## 📚 References

- Chen et al. (2023). *Canadian Wildfire Smoke and Asthma Syndrome Emergency Department Visits in New York City*. JAMA, 330(14), 1385–1387. https://pmc.ncbi.nlm.nih.gov/articles/PMC10514869/
- Communications Earth & Environment (2025). *Radiative cooling in New York/New Jersey metropolitan areas by wildfire particulate matter from the 2023 Canadian wildfires*. https://www.nature.com/articles/s43247-025-02214-3
- NYC Community Air Survey (2023). https://a816-dohbesp.nyc.gov/IndicatorPublic/data-features/nyccas/

---

## 👩‍💻 Author

**Sheila Alonso** — Junior Data Analyst  
📧 sheila.alonso7@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/sheila-alonso-rodriguez)
