# Heart-Disease-Prediction
## Objective

The goal of this project is to predict the presence of heart disease based on patient medical and clinical records using machine learning models.

## Dataset

Source: UCI Heart Disease Dataset

Target Variable: target

1 → Disease Present

0 → No Disease

The dataset includes features such as:

- Age

- Sex

- Chest Pain Type

- Resting Blood Pressure

- Cholesterol

- Fasting Blood Sugar

- Resting ECG

- Maximum Heart Rate

- Exercise-Induced Angina

- ST Depression (Oldpeak)

- ST Slope

## Project Workflow
1️. Exploratory Data Analysis (EDA)

- Data inspection and cleaning

- Checking missing values

- Correlation heatmaps

- Distribution plots

- Feature relationships with target

2️. Data Preprocessing

- Label Encoding of categorical variables

- Feature Scaling using StandardScaler

- Train-Test Split

3️. Model Training

The following models were implemented and compared:

- Logistic Regression

- Decision Tree

- Random Forest

- Support Vector Machine (SVM)

- Voting Classifier (Ensemble)

## Best Model

Random Forest Classifier

Accuracy: ~87.5%

Balanced performance across precision and recall

Robust against overfitting compared to single decision tree

## Hyperparameter Tuning

GridSearchCV was used to optimize model parameters.

Improved model performance through systematic tuning.

## Model Deployment

The trained model is saved using joblib:

---
import joblib

joblib.dump(model, "heart_disease_model.pkl")
joblib.dump(feature_list, "feature_list.pkl")

---
To load and predict:

---
model = joblib.load("heart_disease_model.pkl")
features = joblib.load("feature_list.pkl")

---
## Tools & Technologies

- Python

- Pandas

- NumPy

- Matplotlib

- Seaborn

- Scikit-learn

- Scikit-learn Models Used:

- Logistic Regression

- Decision Tree

- Random Forest

- SVM

- Voting Classifier

## Key Skills Demonstrated

- Data Cleaning & EDA

- Correlation Heatmaps

- Feature Engineering

- Feature Scaling

- Ensemble Learning

- Hyperparameter Tuning

- Model Evaluation

- Model Persistence

## Future Improvements

Use XGBoost or LightGBM

Deploy using Flask/Streamlit

Add SHAP for model interpretability

Perform advanced feature engineering
