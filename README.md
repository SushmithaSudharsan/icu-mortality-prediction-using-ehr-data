# ICU Mortality and Length of Stay Prediction

A healthcare machine learning project using **MIMIC-IV clinical data** to explore early prediction of ICU mortality and length of stay using information from the **first 24 hours of ICU admission**.

## Objectives

* Predict in-hospital ICU mortality using early clinical data.
* Predict whether survivors have a short ICU stay of **≤7 days**.
* Identify clinical features associated with mortality and length of stay.

## Approach

The project includes data preprocessing, missing-value imputation, feature engineering, classification, and regression models.

**Mortality models:** Logistic Regression · Random Forest · XGBoost · MLP
**LOS models:** Elastic Net · KNN · Random Forest · XGBoost

## Results

For mortality prediction, **XGBoost achieved an ROC-AUC of 0.90**.

For length-of-stay prediction, the models achieved MAE values around **0.94–0.96 days**.

Key predictors included **GCS measurements, respiratory failure, sepsis, urea nitrogen, age, heart rate, and hematocrit**.

## Tech Stack

**Python · Pandas · NumPy · Scikit-learn · XGBoost · Matplotlib · Seaborn · MIMIC-IV(Data Set)**

> This project uses credentialed-access clinical data from PhysioNet.

[View the Repository →](#)
