# Earthquake Prediction Analysis

Seismic data analysis and magnitude prediction using machine learning. Built as part of the **Big Data** course at Ionian University.

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-1.5%2B-150458?logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit_learn-1.2%2B-F7931E?logo=scikit-learn)

---

## What It Does

- Cleans and preprocesses historical seismic data (coordinates, depth, magnitude, datetime)
- Analyzes temporal trends at yearly and decadal scales
- Identifies high-frequency geographical hotspots using lat/long grouping
- Compares three regression models to predict earthquake magnitude

---

## Models Compared

Three regression models were trained and compared. **Gradient Boosting performed best**: MAE 0.32, MSE 0.18, R² 0.86.

Random Forest and Decision Tree were also evaluated; only the winning model's scores are reported here.

---

## EDA Highlights

- **Temporal trends** — yearly and decadal magnitude averages reveal long-term activity patterns
- **Geographical hotspots** — top seismogenic zones identified by event frequency
- **Magnitude distribution** — breakdown of low vs. high magnitude events across the dataset
- **Extreme events** — top 10 strongest earthquakes ranked by magnitude

---

## Installation

```bash
git clone https://github.com/NickLitharis/earthquake-prediction
cd earthquake-prediction
pip install -r requirements.txt
```

Open `final-earthquake.ipynb` in Jupyter and run all cells.

---

## Dataset

`earthquake_data.csv` — contains fields: `DATETIME`, `LAT`, `LONG`, `DEPTH`, `MAGNITUDE`
