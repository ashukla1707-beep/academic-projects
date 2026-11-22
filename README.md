# Academic Projects

A portfolio of selected Statistics and Machine Learning projects completed as part of my academic practical work.

## Projects

| Project | Area | Notebook |
|---|---|---|
| **House Price Prediction** | Regression, gradient-based estimation and regularization | [Open project](./01_House_Price_Prediction/) |
| **Graduate Admission Prediction** | Binary classification and ensemble learning | [Open project](./02_Graduate_Admission_Prediction/) |

## Technical stack

- **Language:** Python
- **Data handling:** pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Statistical modelling:** statsmodels, scikit-learn
- **Machine learning:** Random Forest, AdaBoost, Gradient Boosting, XGBoost
- **Model assessment:** train/test evaluation, cross-validation, GridSearchCV, confusion matrix and ROC-AUC

## Repository structure

```text
academic-projects/
├── README.md
├── requirements.txt
├── 01_House_Price_Prediction/
│   ├── README.md
│   └── House_Price_Prediction.ipynb
└── 02_Graduate_Admission_Prediction/
    ├── README.md
    └── Graduate_Admission_Prediction.ipynb
```

## Running the notebooks

1. Clone this repository.
2. Install the dependencies: `pip install -r requirements.txt`.
3. Open the required project folder in Jupyter Notebook or JupyterLab.
4. Place the corresponding input data file in the same folder as its notebook before running all cells.

**Data note:** The original practical notebooks expect local input files named `Median_Prices.xls` (House Price Prediction) and `Uad.xls` (Graduate Admission Prediction). These datasets are not included in this repository. Obtain them from the original course/source and confirm that you have permission to use or redistribute them. The notebooks preserve the analysis workflow; performance metrics should be rechecked by rerunning the notebooks with the intended data files before being quoted elsewhere.

---

Created and maintained by **Adarsh Shukla**.
