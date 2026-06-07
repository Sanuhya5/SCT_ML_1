# 🏠 House Price Prediction using Linear Regression

> **SkillCraft Technology — Machine Learning Internship | Task 1**

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://python.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.3%2B-orange?logo=scikit-learn)](https://scikit-learn.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 📋 Project Overview

This project implements a **Linear Regression model** to predict house prices based on three features:

| Feature | Description |
|---|---|
| `SquareFootage` | Above-ground living area (sq ft) |
| `Bedrooms` | Number of bedrooms |
| `Bathrooms` | Number of full bathrooms |

The **target variable** is `HousePrice` (sale price in USD).

---

## 📁 Project Structure

```
skillcraft_task1/
│
├── house_price_prediction.ipynb   # Main Jupyter Notebook (all steps)
├── README.md                      # Project documentation (this file)
├── requirements.txt               # Python dependencies
├── train.csv                      # Dataset (optional — see note below)
│
└── outputs/                       # Auto-generated during notebook run
    ├── missing_values.png
    ├── price_distribution.png
    ├── pairplot.png
    ├── correlation_heatmap.png
    ├── price_by_category.png
    ├── scatter_features.png
    ├── coefficients.png
    ├── metrics.png
    ├── viz_actual_vs_predicted.png
    ├── viz_residuals.png
    └── dashboard.png
```

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/<your-username>/skillcraft-task1-house-price-prediction.git
cd skillcraft-task1-house-price-prediction
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv

# Windows
venv\Scripts\activate

# macOS / Linux
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. (Optional) Add Real Dataset

Download **train.csv** from [Kaggle — House Prices: Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data) and place it in the project root.

> **If `train.csv` is not found**, the notebook automatically generates a realistic synthetic dataset (1,460 rows) that mirrors the Kaggle distribution — so you can run the notebook **without any dataset download**.

### 5. Launch Jupyter Notebook

```bash
jupyter notebook house_price_prediction.ipynb
```

Then select **Kernel → Restart & Run All** to execute all cells.

---

## 📊 Methodology

```
Data Loading
     │
     ▼
Data Cleaning & Missing Value Analysis
     │
     ▼
Exploratory Data Analysis (EDA)
     │
     ▼
Feature Selection (SquareFootage, Bedrooms, Bathrooms)
     │
     ▼
Train-Test Split (80% / 20%)
     │
     ▼
Linear Regression Model Training
     │
     ▼
Predictions on Test Set
     │
     ▼
Evaluation (MAE, MSE, RMSE, R²)
     │
     ▼
Visualizations + Dashboard
```

---

## 📈 Model Performance

| Metric | Value |
|---|---|
| **MAE** | ~$26,000 |
| **MSE** | ~$1.05 × 10⁹ |
| **RMSE** | ~$32,000 |
| **R² Score** | ~0.72 |

> Exact values depend on the dataset used (synthetic vs. real Kaggle data).

---

## 📊 Visualizations Generated

| Visualization | Description |
|---|---|
| Missing Values Chart | Bar chart showing % of missing values per column |
| Price Distribution | Histogram + KDE + Box Plot of house prices |
| Pairplot | All feature-vs-feature scatter plots |
| Correlation Heatmap | Linear correlation between all numerical features |
| Box Plots | Price distribution grouped by Bedrooms & Bathrooms |
| Scatter Plots | Feature vs Price with trend lines |
| Coefficient Chart | Learned regression weights per feature |
| Actual vs Predicted | Scatter plot with perfect prediction diagonal |
| Residual Plot | Residuals vs Predicted + Residual Distribution |
| Summary Dashboard | All key plots in a single 2×3 grid |

---

## 🛠️ Technologies Used

- **Python 3.8+**
- **NumPy** — Numerical operations
- **Pandas** — Data manipulation
- **Matplotlib** — Base plotting
- **Seaborn** — Statistical visualizations
- **Scikit-learn** — Machine learning model and metrics

---

## 🎓 Key Concepts Covered

- Simple and Multiple Linear Regression
- Ordinary Least Squares (OLS)
- Missing value imputation (median strategy)
- Outlier detection and capping (IQR method)
- Exploratory Data Analysis (EDA)
- Model evaluation metrics (MAE, MSE, RMSE, R²)
- Residual analysis
- Overfitting vs. underfitting check

---

## 💼 About This Project

This notebook was developed as **Task 1** of the **SkillCraft Technology Machine Learning Internship**. It demonstrates end-to-end implementation of a Linear Regression pipeline — from raw data to a fully evaluated, production-style model with professional visualizations and documentation.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🤝 Connect

If you found this helpful, feel free to ⭐ the repo and connect on [LinkedIn](https://linkedin.com/in/your-profile).

---

*Built with ❤️ during the SkillCraft Technology ML Internship*
