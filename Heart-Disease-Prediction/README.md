#  Heart Disease Prediction

## Problem Statement
Predict whether a patient has heart disease based on medical attributes.

## Dataset
- Source: Heart Disease UCI (Kaggle)
- Rows: 303 | Columns: 14

## Steps Performed
- Exploratory Data Analysis + Correlation Heatmap
- Missing value check
- Feature Engineering
- Train/Test Split + StandardScaler

## Models Used
| Model | Test Accuracy |
|---|---|
| Logistic Regression | 85.25% |
| Random Forest | 88.52% |
| XGBoost | 85.25% |

## Best Model: Random Forest
- Precision: 85%
- Recall: 91%
- F1 Score: 88%
- Tuned with GridSearchCV + max_depth=4

## Libraries Used
pandas, numpy, scikit-learn, xgboost, matplotlib, seaborn, joblib
