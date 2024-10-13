# Chest-X-ray-Images

### Summary and Recommendations

#### 1. Overview

This project is designed to predict mortality outcomes based on patient data using various machine learning models, including Logistic Regression, Random Forest, Gradient Boosting, and XGBoost. The process involves data preprocessing, model training, evaluation, and interpretation using SHAP (SHapley Additive exPlanations) for feature importance analysis. The ultimate goal is to identify which patients are more likely to experience mortality during their hospital stay, based on available clinical data.

#### 2. Data

This dataset contains 5,856 validated Chest X-Ray images. The images are split into a training set and a testing set of independent patients. Images are labeled as (disease:NORMAL/BACTERIA/VIRUS)-(randomized patient ID)-(image number of a patient). For details of the data collection and description.

#### 3. Data Analysis Steps

1. Data Loading
2. Feature Engineering
3. Train-Test Split
4. Handling Class Imbalance
5. Model Training and Evaluation:
  - Logistic Regression
  - Random Forest
  - Gradient Boosting
  - XGBoost
6. Hyperparameter Tuning
7. Model Interpretation Using SHAP

#### 4. Key Findings
      
Classification Report:

- For the classes normal and opacity, the model achieves a high level of performance.
- The precision, recall, and F1-score for both classes are quite strong, indicating that the model can accurately predict both normal and opacity cases.
- Accuracy is 94%, which is a robust indicator of the model’s overall performance.

#### 5. Source

https://www.kaggle.com/datasets/tolgadincer/labeled-chest-xray-images
