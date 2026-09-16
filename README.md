# car-price-prediction
End-to-end car price analysis: Python cleaning, Excel dashboard, and ML prediction (93% R²)
# 🚗 Car Price Prediction — End-to-End Data Project

An end-to-end data project on a used-car dataset (8,000 records): from raw messy data cleaned in **Python**, to an interactive **Excel dashboard**, to a **Machine Learning** model that predicts car prices with **93% accuracy (R²)**.

## 📌 Project Overview

This project covers the full data analytics pipeline:

1. **Data Cleaning & Preprocessing** (Python / Pandas)
2. **Data Modeling & Dashboard** (Excel / Power Pivot / DAX)
3. **Machine Learning** (Regression)

---

## 🐍 1. Data Cleaning (Python)

- Removed duplicate records
- Handled missing values using **median** and **mode** (based on each column's nature)
- Extracted numeric values from messy text columns (e.g. `1248 CC` → `1248`)
- Used **Regex** to parse a complex `torque` column
- Standardized inconsistent text categories

## 📊 2. Dashboard (Excel — Power Pivot & DAX)

- Built a **Star Schema**: a Fact table (Cars) linked to 3 Dimension tables (Brands, Fuel, Transmission) via One-to-Many relationships
- Created **DAX measures** (Average Price, Total Cars, Max/Min Price)
- Designed an interactive dashboard with 6 visuals, dynamic KPI cards, and slicers

![Dashboard](Cars_Dashboard%20-%20Copy.png)

## 🤖 3. Machine Learning (Price Prediction)

- Encoded categorical features (One-Hot Encoding)
- Split data into training (80%) and testing (20%)
- Compared 3 models: **Linear Regression**, **Random Forest**, **XGBoost**
- **Best model: Random Forest** — R² = **0.928**, MAE ≈ 100,665

### Key Insight
The most important factors in a car's price are **engine power (max_power)** and **vehicle age**.

---

## 🛠️ Tools & Libraries
`Python` · `Pandas` · `Scikit-learn` · `XGBoost` · `Matplotlib` · `Excel` · `Power Pivot` · `DAX`

## 📂 Files
- `cardekho_dataset.ipynb` — Full Python code (cleaning + ML)
- `cars_cleaned.csv` — Cleaned dataset
- `Cars_Dashboard.png` — Excel dashboard
