# House Price Prediction — Regression & Regularization

## Objective

Explore regression-based approaches for predicting the target variable `PRICE` from housing and neighbourhood attributes.

## Dataset

The notebook's recorded data preview contains **506 observations**, 12 explanatory variables and the target `PRICE`. The input file expected by the notebook is `Median_Prices.xls`.

The dataset file is not included in this repository. Place the authorized source file in this folder before running the notebook.

## Workflow

1. Inspect data types, summary statistics and missing values.
2. Handle missing numeric values and encode the binary `RIVER` feature.
3. Fit an Ordinary Least Squares (OLS) model and a multiple linear regression model.
4. Assess model fit with R-squared, Mean Squared Error and 10-fold cross-validation.
5. Standardize predictors for gradient-based estimation and regularized regression.
6. Explore `SGDRegressor`, Ridge, LASSO and Elastic Net, including hyperparameter search with `GridSearchCV`.
7. Compare coefficient behaviour and prediction errors.

## Methods and tools

**Python:** pandas, NumPy, Matplotlib, Seaborn, statsmodels and scikit-learn.

**Methods:** OLS, multiple linear regression, stochastic gradient descent, Ridge (L2), LASSO (L1), Elastic Net, standardization, cross-validation and grid search.

## Files

- `House_Price_Prediction.ipynb` — notebook containing the analysis and model comparisons.
- `Median_Prices.xls` — required local input file; not included.

## Reproducibility note

The notebook reads `Median_Prices.xls` from its working directory. The file name is retained from the original practical. Confirm the dataset's file format and source before rerunning; adjust the data-loading function if the source file is an Excel workbook rather than CSV-formatted text. Re-run the notebook to regenerate metrics before quoting any scores.


## Validation consideration

For the SGD and regularized-regression workflows, standardization is fitted on the training split and then applied to the held-out test split. The practical's earlier missing-value imputation is still performed before the split; for a fully leakage-safe evaluation, move imputation into a scikit-learn pipeline and fit it only within each training fold.
