# Graduate Admission Prediction — Ensemble Classification

## Objective

Build and compare classification models for the binary target `Chance of Admit` using applicant academic and profile features.

## Dataset

The notebook's recorded data preview contains **400 observations**. Predictors include GRE Score, TOEFL Score, University Rating, SOP, LOR, CGPA and Research. The target is `Chance of Admit` (binary).

The input file expected by the notebook is `Uad.xls`. The dataset is not included in this repository; place the authorized source file in this folder before running the notebook.

## Workflow

1. Inspect the dataset dimensions, variable types and missing values.
2. Remove the serial-number field and encode the `Research` feature.
3. Split the data into training and testing sets.
4. Train and tune Random Forest, AdaBoost, Gradient Boosting and XGBoost classifiers.
5. Evaluate classification performance using classification reports, confusion matrices, sensitivity/specificity and ROC-AUC.
6. Use cross-validation and `GridSearchCV` to compare model configurations.

## Methods and tools

**Python:** pandas, NumPy, Matplotlib, Seaborn and scikit-learn; XGBoost.

**Methods:** Random Forest, AdaBoost, Gradient Boosting, XGBoost, one-hot encoding, train/test split, cross-validation, grid search, confusion matrix and ROC analysis.

## Files

- `Graduate_Admission_Prediction.ipynb` — notebook containing the model development and evaluation.
- `Uad.xls` — required local input file; not included.

## Reproducibility note

The notebook expects `Uad.xls` in its working directory. Confirm the dataset's file format and source before rerunning; adjust the data-loading function if necessary. Re-run the notebook before quoting model metrics because results depend on the chosen split, estimator and evaluation method.
