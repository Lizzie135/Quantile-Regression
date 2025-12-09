# Quantile Regression & ML: SAT Performance Analysis

**Author:**  Elizabeth-Lynda Nartey  

## Description
Analyzes the impact of parental income on SAT performance using quantile regression and machine learning. Captures effects across the performance distribution, predicts SAT outcomes, and identifies key factors like school tier and public/private status to understand educational inequality.

---

## Dataset
- **Source:** [Kaggle: Elite College Admissions](https://www.kaggle.com/datasets/mexwell/elite-college-admissions)  
- **Size:** 1,946 rows, 81 columns  
- **Key Features:**  
  - `income` — parental household income percentile  
  - `tier` — school selectivity  
  - `public` — public/private school indicator  
- **Target Variable:** `sat` — SAT attendance rate (scaled, proxy for SAT scores)  

---

## Methods

### Data Cleaning & Preprocessing
- Selected relevant features and dropped missing values  
- Standardized and encoded categorical features  

### Exploratory Data Analysis (EDA)
- Scatterplots and jitter plots for SAT vs. income  
- Visualized school tier and public/private effects  

### Quantile Regression
- Estimated SAT performance at **10th and 90th percentiles**  
- Revealed that parental income has a stronger effect on high-performing students  

### Machine Learning Models
- Linear Regression (baseline)  
- Random Forest Regressor  
- Gradient Boosting Regressor (optional: XGBoost/LightGBM)  
- Evaluated using RMSE, MAE, R²  

### Visualization of Predictions
- Predicted SAT scores vs. actual scores  
- Feature importance for tree-based models  

---

## Key Insights
- Quantile regression shows income effects are **not uniform**: higher-income families disproportionately boost top-performing students.  
- ML regressors can accurately predict SAT attendance, enabling targeted academic support.  
- School tier and public/private status significantly influence SAT outcomes.  

---

## Tools & Libraries
- **Python:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `seaborn`  
- **R:** `quantreg`, `broom`, `tidyverse`  
- **Environment:** Jupyter Notebook, RStudio  

---

## Future Work
- Incorporate additional student and school features  
- Hyperparameter tuning for ML models  
- Combine ML predictions with quantile regression insights for actionable interventions  

---

## How to Run
1. Clone this repo:
```bash
git clone <your-repo-url>

