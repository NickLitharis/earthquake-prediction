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

| Model | MAE | MSE | R² |
|---|---|---|---|
| Random Forest | — | — | — |
| Decision Tree | — | — | — |
| **Gradient Boosting** | **0.32** | **0.18** | **0.86** |

Gradient Boosting achieved the best performance with an R² of 0.86.

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
