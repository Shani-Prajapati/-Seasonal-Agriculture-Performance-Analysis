# Seasonal Agriculture Performance Analysis

**VOIS AICTE Major Project — Data Analytics Track (Batch 1, 2026-2027)**

Author: Shani Prajapati | Karnavati University

## Overview

This project analyzes 4,000 farm records spanning three Indian cropping seasons —
**Kharif, Rabi, and Zaid** — to understand how agricultural performance (yield, cost,
revenue, profit, resource use, and risk) changes across seasons, and what factors
actually drive that variation.

## Problem Statement

Agricultural activities are influenced by seasonal variations in environmental
conditions, farming practices, resource availability and market conditions. Raw
agricultural data does not by itself explain how performance changes across
seasons. This project investigates seasonal differences in agricultural
performance by identifying meaningful patterns, trends, relationships and
variations in the data.

## Dataset

`seasonal_agriculture_performance_dataset.csv` — 4,000 farm-level records across
8 Indian states, 8 crops, and 3 seasons, with 28 columns covering:

- Environmental conditions (rainfall, temperature, humidity, soil pH/moisture)
- Farming inputs (fertilizer, pesticide, irrigation method, seed quality)
- Outcomes (yield, production, cost, revenue, profit, water efficiency, disease/pest risk)

## Approach

1. **Data cleaning** — handled missing values (season/crop-wise median imputation), checked for duplicates
2. **Feature engineering** — profit margin %, cost per tonne
3. **Exploratory analysis** — seasonal summaries, distributions, correlation analysis
4. **Visualization** — 8 charts covering yield/profit by season, environmental conditions, resource usage, profit distribution & loss rate, correlation heatmap, crop mix, state-wise patterns, and water-yield relationships
5. **Insights & recommendations** — evidence-based takeaways for seasonal agricultural planning

## Key Findings

- **Kharif** is the strongest season on almost every metric (highest rainfall, yield, and profit), but even here **42% of farms operate at a loss**.
- **Zaid** (summer) is structurally loss-making — average profit is negative, and **65% of Zaid farms lose money**.
- **Water access**, not rainfall or fertilizer, is the strongest driver of yield (r=0.39) and profit (r=0.49).
- Fertilizer and pesticide usage stay nearly flat across seasons while yield and profit fall sharply — inputs aren't scaling down with outcomes.
- The Kharif > Rabi > Zaid profit ranking holds in **7 of 8 states**, confirming a genuine seasonal effect rather than a regional one.

Full analysis, charts, and recommendations are documented in
[`Seasonal_Agriculture_Performance_Analysis.ipynb`](./Seasonal_Agriculture_Performance_Analysis.ipynb).

## Tech Stack

- Python (Pandas, NumPy)
- Matplotlib, Seaborn
- Jupyter Notebook

## Repository Contents

```
├── Seasonal_Agriculture_Performance_Analysis.ipynb   # Full documented analysis
├── seasonal_agriculture_performance_dataset.csv       # Raw dataset
└── README.md
```

## How to Run

```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook Seasonal_Agriculture_Performance_Analysis.ipynb
```
