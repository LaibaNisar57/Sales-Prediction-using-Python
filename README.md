# Sales-Prediction-using-Python
## 👤 Author
- **Program:** EXPS Nexus Virtual Internship
- **Role:** Data Science Intern
- **Name:** Laiba Nisar
# Multi-Channel Advertising Sales Prediction & Budget Optimization

An econometric and machine learning study analyzing the relationship between media expenditures (TV, Radio, Newspaper) and product sales to eliminate marketing waste and maximize return on ad spend (ROAS).


## 📌 Project Overview
Marketing teams often misallocate capital across channels due to unmeasured channel cross-effects. This project implements multiple regression and non-linear tree-based models on empirical advertising data to isolate the marginal returns of each medium, forecast sales demand, and recommend a mathematically defensible budget reallocation strategy.


## 📊 Key Findings & Channel Elasticity

- **TV Spend (Volume Anchor):** Displays the strongest overall correlation with product demand ($r \approx 0.90$). High absolute investments drive brand baseline scale.
- **Radio Spend (High-Efficiency Multiplier):** Delivers the highest marginal sales yield per dollar invested, acting as a cost-effective performance accelerator alongside TV.
- **Newspaper Spend (Zero Marginal Return):** Shows near-zero statistical significance ($p > 0.05$, coefficient near zero) when controlling for TV and Radio. Budget spent here acts as friction rather than growth.

## ⚙️ Model Evaluation Benchmark

| Model | Evaluation Role | R² Score | MAE | RMSE |
| :--- | :--- | :--- | :--- | :--- |
| **Linear Regression (OLS)** | Causal inference & marginal elasticity | ~0.899 | ~1.25 | ~1.65 |
| **Ridge Regression** | Multicollinearity control | ~0.899 | ~1.25 | ~1.65 |
| **Random Forest Regressor** | Non-linear feature interactions | **~0.975** | **~0.60** | **~0.85** |

*Random Forest provides the highest predictive accuracy, while Ordinary Least Squares (OLS) delivers interpretable coefficients for executive budget decisions.*

## 💼 Actionable Marketing Strategy
1. **Defund Print Channels:** Reallocate 100% of the active Newspaper budget directly into high-yield Radio and top-of-funnel TV campaigns.
2. **Implement an 80/20 TV-Radio Synergy:** Maintain TV as the primary top-funnel awareness engine while using Radio to capture low-cost frequency.
3. **Diminishing Returns Guardrails:** Cap single-channel TV scaling using marginal response tracking to avoid advertising saturation.

### Requirements
- Python 3.9+
- Jupyter Notebook / Google Colab

### Installation
pip install pandas numpy matplotlib seaborn scikit-learn
