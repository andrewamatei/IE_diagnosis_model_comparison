# Machine Learning for Infective Endocarditis Detection

This project compares five machine learning models for detecting infective endocarditis, IE, using clinical data from the Medical Information Mart for Intensive Care II, MIMIC-II, database.

The goal was to evaluate how well different models can identify IE cases and support early clinical risk detection. The project compares Decision Tree, Random Forest, Logistic Regression, Extreme Gradient Boosting, XGBoost, and CatBoost using a consistent evaluation framework based on 5-fold cross-validation.

## Project Overview

Infective endocarditis is a serious condition that can be difficult to diagnose early because symptoms may overlap with other diseases. This project applies machine learning techniques to clinical data to compare model performance and identify which methods show the strongest potential for supporting diagnosis.

The analysis focuses on model discrimination and classification quality using:

- Area Under the Curve, AUC
- Sensitivity
- Specificity
- Positive Predictive Value, PPV
- Negative Predictive Value, NPV
- 95% confidence intervals for AUC

The project also includes feature importance analysis to help explain which variables had the greatest influence on model predictions. :contentReference[oaicite:2]{index=2} :contentReference[oaicite:3]{index=3}

## Models Evaluated

The following models were compared:

- Decision Tree
- Random Forest
- Logistic Regression
- XGBoost
- CatBoost

Each model was assessed using the same evaluation structure to support fair comparison across methods. :contentReference[oaicite:4]{index=4}

## Methods

The project used clinical records from the MIMIC-II dataset and applied supervised machine learning methods for binary classification of infective endocarditis cases.

### Evaluation approach

- Data prepared for classification modeling
- Models trained and tested using 5-fold cross-validation
- Performance summarized using AUC, sensitivity, specificity, PPV, and NPV
- Confidence intervals used to assess stability of model performance
- Feature importance reviewed for interpretability in selected models

This approach helped reduce reliance on a single train-test split and gave a more stable estimate of model performance across folds. :contentReference[oaicite:5]{index=5} :contentReference[oaicite:6]{index=6}

## Key Findings

The analysis showed meaningful differences across the five models.

- Random Forest and Logistic Regression were among the strongest overall performers
- XGBoost also showed strong predictive ability with higher specificity than some competing models
- Decision Tree had the weakest overall performance among the compared models
- CatBoost showed promising classification performance and balanced precision and recall
- Feature importance analysis helped identify influential predictors linked to infective endocarditis risk

One reported result in the project showed XGBoost with an AUC of 0.88, sensitivity of 0.80, and specificity of 0.82, while Random Forest and Logistic Regression each reached an AUC of 0.89 in the comparative evaluation summary. The project also reports CatBoost accuracy of 84 percent on the held-out test data. :contentReference[oaicite:7]{index=7}

## Why this project matters

This project shows how machine learning can be used to support healthcare analytics and clinical decision support. It also demonstrates a full comparison workflow rather than relying on a single model.

From a technical point of view, the project shows experience in:

- Healthcare data analysis
- Predictive modeling
- Model evaluation
- Cross-validation
- Feature importance analysis
- Clinical interpretation of machine learning outputs

## Tools and Technologies

- Python
- Scikit-learn
- XGBoost
- CatBoost
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

## Repository Structure

```text
project-folder/
│
├── data/                  # Input data files, if shareable
├── notebooks/             # Jupyter notebooks for analysis and modeling
├── outputs/               # Charts, evaluation results, and exported visuals
├── images/                # Figures for README or portfolio use
├── README.md
└── requirements.txt
