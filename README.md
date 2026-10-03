# ICU Mortality and Length of Stay Prediction Using EHR Data

A machine learning project using **MIMIC-IV clinical data** to predict ICU mortality and length of stay using patient information from the **first 24 hours of ICU admission**.

## Project Overview

The project investigates two prediction tasks:

- **ICU Mortality Prediction:** Predict in-hospital mortality using early ICU clinical information.
- **Length of Stay Prediction:** Among survivors, predict whether the ICU stay is **≤7 days** and estimate length of stay.

## Data & Preprocessing

The project uses credentialed-access **MIMIC-IV** data from PhysioNet. Clinical, demographic, and diagnostic information was processed and combined using patient and admission identifiers.

Key preprocessing steps included:

- Processing large clinical event tables in chunks
- Handling missing values through imputation
- Feature engineering and encoding
- Filtering clinically implausible values
- Removing readmissions and very short ICU stays
- Preparing separate datasets for mortality classification and LOS prediction

## Machine Learning Models

### Mortality Prediction

- Logistic Regression
- Random Forest
- XGBoost
- Multi-Layer Perceptron (MLP)

### Length of Stay Prediction

- Elastic Net
- K-Nearest Neighbors
- Random Forest
- XGBoost

## Results

For mortality prediction, **XGBoost achieved an ROC-AUC of 0.90**.

For length-of-stay prediction, the models achieved MAE values between **0.94 and 0.96 days**.

Important predictors identified across the tasks included **GCS measurements, respiratory failure, sepsis, urea nitrogen, age, heart rate, and hematocrit**.

## Tech Stack

**Python · Pandas · NumPy · Scikit-learn · XGBoost · Matplotlib · Seaborn · Jupyter · Google Colab**

**Dataset:** MIMIC-IV

## Project Report

The complete methodology, analysis, model comparison, and results are documented in the project report.

[Read the Full Project Report →](https://github.com/SushmithaSudharsan/icu-mortality-prediction-using-ehr-data/blob/main/Final_Project%20Report.pdf)

[View Repository →](https://github.com/SushmithaSudharsan/icu-mortality-prediction-using-ehr-data)
