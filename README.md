
# 🌍 World Bank Indicators Analysis (2010–2019)

## 📊 Project Overview

This project is a data analysis exercise using **pandas**, **matplotlib/seaborn**, and **scikit-learn**.

We analyze simulated economic, social, and environmental indicators for 20 countries over the period 2010–2019. The objective is to explore data patterns, visualize key metrics, and attempt a basic prediction model for CO₂ emissions.

---

## 🗂️ Dataset Description

**Columns include:**

- `Country`, `Year`
- `GDP (USD)` – Gross Domestic Product (in billions USD)
- `Population` – in millions
- `Life Expectancy` – average life expectancy in years
- `Unemployment Rate (%)`
- `CO₂ Emissions (metric tons per capita)`
- `Access to Electricity (%)`

[the dataset](https://www.kaggle.com/datasets/bhadramohit/world-bank-dataset/discussion/543598)

---

## 🔍 Analysis Workflow

### 1. Data Cleaning
- Removed duplicates
- Grouped data by `Country` and `Year` and calculated mean values

### 2. Visualizations
- Line plots for **GDP** over time (India, US, Germany)
- GDP comparison
- Life expectancy trends
- CO₂ emissions comparison
- Unemployment Rate (%) comparison
-  Mean Life Expectancy by Country
-  Scatterplot: GDP vs CO2
- **Correlation heatmap** of numerical features

### 3. Machine Learning (Simple Linear Regression)
**Goal:** Predict CO₂ emissions per capita

```python
R² Score: -0.077
MSE: 25.10
```

The model performed poorly, indicating linear regression is not sufficient for this dataset.

---

## 📌 Key Observations

- **Life expectancy** is decreasing in the US, Germany, and India — surprisingly. **Turkey** shows the highest value.
- **GDP** grows in India and the US, but declines in Germany.
- **CO₂ emissions** are notably high in **India** and **South Africa**.
- **No strong correlations** were found between most numeric features (as shown in the heatmap).

---

## 📉 ML Summary

- Linear regression shows **low performance** on this task (R² < 0).
- Indicates a need for better feature engineering and possibly nonlinear models.
- Could improve with scaling, more features, or advanced models like **RandomForest** or **XGBoost**.

---

## 💻 Libraries Used

```python
pandas, matplotlib, seaborn
scikit-learn (train_test_split, LinearRegression, r2_score, mean_squared_error)
```

---

## 📁 Project Structure

```
project/
├── data/
│   └── dataset.csv
├── notebooks/
│   └── analysis.ipynb
├── README.md
```

---

## ✅ Next Steps

- Try additional visualizations (bar plots, box plots, facet grids)
- Add a dashboard  with Power BI 
