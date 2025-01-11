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

#### Source

https://www.kaggle.com/datasets/tolgadincer/labeled-chest-xray-images
