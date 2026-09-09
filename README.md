# Seasonal Agriculture Performance Analysis

**VOIS for Tech (AICTE) — Major Project | Data Visualization Track**

## Overview

Agricultural performance shifts from season to season due to changing environmental
conditions, resource availability, and farming practices — but raw farm data rarely
makes those shifts obvious on its own. This project analyzes a 4,000-record seasonal
agriculture dataset to identify meaningful patterns, trends, and relationships in how
farming performance changes across India's three cropping seasons: **Kharif, Rabi,
and Zaid**.

## Objective

- Explore and clean the dataset
- Compare environmental conditions, resource usage, yield, disease/pest risk, and
  economic performance across seasons
- Test whether observed seasonal differences are statistically significant
- Identify relationships between environmental/resource factors and outcomes
- Translate findings into evidence-based, season-specific recommendations

## Dataset

`seasonal_agriculture_performance_dataset.csv` — 4,000 farm records covering:

- 8 states, 10 districts, 8 crops, 3 seasons, 4 irrigation methods
- Environmental conditions (rainfall, temperature, humidity, sunlight, soil)
- Resource usage (fertilizer, pesticide, water)
- Yield, production, and economic performance (cost, revenue, profit)

## Approach

1. **Data cleaning** — missing-value imputation, outlier capping (IQR method)
2. **Exploratory analysis** — seasonal comparisons via boxplots, bar charts, and heatmaps
3. **Statistical testing** — one-way ANOVA to confirm significance of seasonal yield differences
4. **Correlation analysis** — identifying which factors most influence yield and profitability
5. **Cross-analysis** — crop × season and state × season patterns, to check consistency across regions
6. **Insights & recommendations** — evidence-based, season-specific conclusions

## Tools & Technologies

- Python 3
- Pandas, NumPy — data cleaning and manipulation
- Matplotlib, Seaborn — visualization
- SciPy — statistical testing
- Jupyter Notebook — analysis and documentation

## Repository Contents

| File | Description |
|---|---|
| `Seasonal_Agriculture_Performance_Analysis.ipynb` | Full analysis notebook |
| `seasonal_agriculture_performance_dataset.csv` | Source dataset |
| `README.md` | Project overview (this file) |

## Key Findings

- Yield differs significantly across seasons (one-way ANOVA, p < 0.001)
- Kharif shows the highest rainfall, humidity, and disease/pest risk
- Water-use efficiency and yield are the two variables most strongly correlated with profitability
- Seasonal patterns are not fully uniform across crops and states — some regions/crops
  buck the general seasonal trend
- Several records show costs exceeding revenue, particularly in the Zaid season —
  pointing to an efficiency gap worth further investigation

## How to View

Open `Seasonal_Agriculture_Performance_Analysis.ipynb` directly on GitHub (renders
automatically), or open it in [Google Colab](https://colab.research.google.com) for
an interactive view.

---
**Course:** Data Visualization — VOIS for Tech (AICTE), Batch 2026-2027
