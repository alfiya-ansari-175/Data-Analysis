# 🏡 Ames Housing Data Analysis

This project explores the Ames Housing dataset, performing data cleaning, visualization, and statistical modeling to uncover insights related to home sale prices.

The analysis is conducted in a Jupyter Notebook: `Analysis.ipynb`.

---

## 🧾 Overview

The main goal is to analyze various factors affecting home sale prices using data preprocessing, visualization, and statistical modeling techniques. It includes:

- Data loading and inspection
- Handling missing values
- Exploratory Data Analysis (EDA)
- Feature encoding and transformation
- Statistical hypothesis testing

---

## 📊 Sample Dataset Preview

The dataset includes 81 features such as zoning, lot size, building type, overall quality, and more. A snippet of the data:


---

## 🔍 Key Insights

📌 **Missing Data**  
Some columns have a large amount of missing values:

- `PoolQC`: 1453 missing
- `MiscFeature`: 1406 missing
- `Alley`: 1369 missing
- `Fence`: 1179 missing

These are handled via imputation or dropped depending on relevance.

📌 **SalePrice Distribution**  
Sale prices are right-skewed. A log transformation is suggested to normalize the distribution.

📌 **Correlation with SalePrice**  
Highly correlated variables with `SalePrice`:

- `OverallQual` (Overall Material and Finish Quality)
- `GrLivArea` (Above grade living area)
- `GarageCars`, `GarageArea`
- `TotalBsmtSF`

📌 **LotShape vs. SalePrice**  
Homes with regular lot shapes tend to have higher sale prices.

📌 **Zoning & Neighborhood Analysis**  
The `MSZoning` and `Neighborhood` features show clear segmentation in sale prices. `RL` zoning generally has higher prices than others.

📌 **ANOVA and Regression**  
OLS regression and ANOVA tests were used to evaluate statistical significance of categorical predictors like `MSZoning`.

---

## 🛠️ Tools & Libraries

- `pandas`, `numpy` – data manipulation
- `matplotlib`, `seaborn` – data visualization
- `scikit-learn` – preprocessing
- `statsmodels`, `scipy` – statistical modeling and tests

---


