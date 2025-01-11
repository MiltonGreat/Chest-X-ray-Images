# Chest X-Ray Image Classification: Detecting Pneumonia with Deep Learning

## Overview

Chest X-rays are a critical tool for diagnosing respiratory conditions such as pneumonia. However, the manual interpretation of X-rays is time-intensive and subject to variability among radiologists. This project leverages deep learning techniques to classify chest X-rays into categories such as normal, bacterial pneumonia, and viral pneumonia, achieving a high accuracy of 94%. The resulting model provides a powerful assistive tool for radiologists, enabling faster and more consistent diagnosis.

### Problem Statement

Pneumonia, a leading cause of morbidity and mortality globally, requires timely diagnosis for effective treatment. Detecting abnormalities in chest X-rays can be challenging due to image complexity and subtle differences among disease categories. This project addresses these challenges using a Convolutional Neural Network (CNN) to automate the classification of chest X-ray images.

### Dataset

- Source: Labeled Chest X-Ray Images Dataset.
- Total images: 5,856 validated chest X-rays.
- Categories: Normal, Bacterial Pneumonia, Viral Pneumonia.
- Split: Training and testing sets based on independent patients.

### Solution Approach:

1. Data Preprocessing
- Image Resizing: Standardized all images to a fixed size for uniform model input.
- Normalization: Scaled pixel values to improve model convergence.
- Augmentation: Applied techniques like flipping, rotation, and zooming to address class imbalance and improve generalization.

2. Model Development
- Convolutional Neural Network (CNN): Built and trained a deep learning model for image classification.
- Transfer Learning: Fine-tuned a pre-trained model (e.g., ResNet or VGG) to leverage feature extraction capabilities.

3. Model Evaluation
- Metrics: Accuracy, precision, recall, F1-score.
- Classification Report: Detailed analysis for each class (normal, bacterial pneumonia, viral pneumonia).

### Key Findings:

Model Performance:
- Accuracy: 94%, indicating robust overall performance.
- Precision and Recall: High scores for normal and pneumonia classes ensure reliable predictions across categories.
- F1-Score: Balanced performance between precision and recall across all classes.

Clinical Insights:
- The model effectively distinguished between bacterial and viral pneumonia, aiding in differential diagnosis.
- Normal cases were accurately identified, reducing the risk of false positives and unnecessary follow-ups.

Example Prediction:
- Input: Chest X-ray labeled as “disease:BACTERIA”.
- Prediction: Correctly classified as bacterial pneumonia with high confidence.

### Challenges

- Class Imbalance: Addressed using extensive data augmentation techniques.
- Computational Resources: Required efficient GPU use for training deep learning models.

### Future Directions

- Broader Disease Coverage: Extend the model to identify other respiratory conditions like tuberculosis or COVID-19.
- Explainability: Incorporate tools like Grad-CAM to visualize the areas of the X-rays contributing to predictions.
- Deployment: Develop a user-friendly application or API for real-world clinical use.
- Integration with Patient Data: Combine X-ray analysis with clinical features for improved diagnosis accuracy.

### Key Skills

Deep learning, image preprocessing, CNNs, Python.


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
