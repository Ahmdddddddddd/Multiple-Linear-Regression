# House Price Prediction — Azerbaijan

Predicting real estate prices across Azerbaijan using Multiple Linear Regression on 200K+ property listings.

## What It Does

Takes a property's city, area, and room count — predicts its market price in AZN.

## Pipeline

1. **Cleaning** — Removed nulls, duplicates, encoded city names
2. **EDA** — Correlation heatmap, scatter plots, histograms, box plots
3. **Statistical Tests** — Skewness analysis, Box-Cox / Yeo-Johnson transformation, normality tests
4. **Feature Selection** — VIF analysis to remove multicollinearity, selected 3 features
5. **Modeling** — Compared Linear, Ridge, Lasso, ElasticNet with 5-fold Cross Validation
6. **Evaluation** — OLS summary, residual analysis, Durbin-Watson test

## Results

| Metric | Value |
|--------|-------|
| R² | 0.856 |
| Adj. R² | 0.856 |
| Durbin-Watson | 1.998 |
| All feature p-values | < 0.001 |

Picked Linear Regression — same performance as regularized models, simpler.

Quick Start

pip install -r requirements.txt
jupyter notebook linearregression.ipynb


**Elton Valiyev** — [LinkedIn](https://www.linkedin.com/in/eltonvaliyev/)
