# Employee Attrition Predictor

A machine learning model that predicts which employees are likely to leave a company and explains why. Built as a baseline for an HR analytics platform.

## Problem

Replacing an employee costs a company far more than retaining one. This project identifies at-risk employees early and highlights the factors driving attrition so HR can act.

## Current Scope (v0.1)

- Exploratory data analysis on HR data
- Preprocessing: encoding, scaling, class imbalance handling (SMOTE)
- Train and compare Logistic Regression and Random Forest
- Evaluate with precision, recall, F1, ROC-AUC
- Feature importance for explainability

## Tech Stack

Python, pandas, scikit-learn, imbalanced-learn, matplotlib, seaborn

## Dataset

- IBM HR Analytics Employee Attrition & Performance (Kaggle)
- 1,470 rows, 35 features (age, job role, overtime, income, satisfaction, tenure, etc.)

## Project Structure

```
attrition-predictor/
├── data/
│   └── hr_attrition.csv
├── notebooks/
│   ├── 01_eda.ipynb
│   └── 02_modeling.ipynb
├── src/
│   ├── preprocess.py
│   └── train.py
├── requirements.txt
└── README.md
```

## Setup

```bash
git clone https://github.com/<your-username>/attrition-predictor.git
cd attrition-predictor
pip install -r requirements.txt
python src/train.py
```

## Results

| Model | Precision | Recall | F1 | ROC-AUC |
|-------|-----------|--------|----|---------|
| Logistic Regression | _tbd_ | _tbd_ | _tbd_ | _tbd_ |
| Random Forest | _tbd_ | _tbd_ | _tbd_ | _tbd_ |

## Roadmap (Future Scope)

- [ ] Gradient boosting (XGBoost / LightGBM) with hyperparameter tuning
- [ ] SHAP explanations for individual employee predictions
- [ ] Cost-sensitive threshold tuning based on retention cost
- [ ] Fairness analysis across gender and age groups
- [ ] Streamlit dashboard for HR teams
- [ ] FastAPI prediction endpoint + Docker deployment
- [ ] MLflow experiment tracking
- [ ] Retention recommendation engine

## License

MIT
