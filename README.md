# ovarian_cancer_prediction_project
Overview

This project focuses on the early detection of ovarian cancer using a multi-modal approach that combines clinical (tabular) data and medical image data.

The system integrates Machine Learning (ML) and Deep Learning (DL) models along with fusion techniques to improve prediction accuracy and reliability.

Objectives
Predict ovarian cancer using clinical and image data.
Improve accuracy using ensemble and fusion techniques.
Perform effective feature selection and preprocessing.
Develop a robust decision-support system for healthcare.

Dataset
1. Tabular Dataset (Clinical Data)
Source: Public datasets (e.g., Kaggle)
Features: Tumor markers, Blood chemistry, CBC parameters
Data Type: Numeric
2. Image Dataset
Classes:
Non-Cancerous
Clear Cell
Endometrioid
Serous
Mucinous

Methodology
 1. Data Preprocessing (Tabular Data)
Checked data shape, types, and null values
Outlier detection using box plots
Outlier treatment:
Log Transformation
IQR Capping
Z-score Capping
Train-test split: 80% training, 20% testing
 2. Machine Learning Models
Random Forest (RF)
Logistic Regression (LR)
Support Vector Machine (SVM)
Multi-Layer Perceptron (MLP)
Best Results:
RF: 90.3% CV Accuracy
LR: 88.8% CV Accuracy
 3. Feature Selection Techniques
SelectKBest
Recursive Feature Elimination (RFE)
Autoencoder-Decoder based feature extraction
Combined top features (union approach) for improved performance
4. Image Data Processing
Image validation (format, size, corrupted files)
Resized to 227 × 227
Data Augmentation:
Rotation
Zoom
Horizontal & Vertical Flip
Brightness Adjustment

Dataset split:
70% Training
15% Validation
15% Testing

 6. Deep Learning Models
VGG16
VGG19
Custom CNN (KKNet)
Configuration:
Optimizer: Adam
Learning Rate: 0.0001
Loss: Categorical Crossentropy

Best Result:
KKNet Accuracy: 93%

 8. Fusion Techniques (Multi-Modal Learning)
To combine predictions from tabular and image models:
Late Fusion
Weighted Fusion
Voting Fusion
Stacking Fusion
Best Performance:
Stacking Fusion (LR as meta-learner)

Evaluation Metrics
Accuracy
Precision
Recall (Sensitivity)
Specificity
F1 Score
Advanced Metrics:
