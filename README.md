**Project Overview**
This project builds a machine learning model to detect fraudulent credit card transactions using anonymized PCA‑transformed features (V1–V28), transaction amount, and class labels.
The goal is to accurately classify transactions as fraud (1) or legitimate (0) using scalable preprocessing, robust model training, and explainable evaluation techniques.

The project uses:

Random Forest Classifier

StandardScaler

Cross‑Validation (F1 scoring)

Feature Importance Analysis

Confusion Matrix & Classification Report

Correlation Heatmap

**Dataset Description**
The dataset contains 568,630 transactions with 31 columns:

Column	Description
id	Unique transaction ID
V1–V28	PCA‑transformed features (anonymized for privacy)
Amount	Transaction amount
Class	Target variable (0 = legitimate, 1 = fraud)

**Data Preprocessing**
1. Remove unnecessary columns
2. Train/Test Split
3. Feature Scaling:Scaling ensures all features contribute equally to the model.
4. Model Training — Random Forest:This configuration balances accuracy and speed for large datasets.Random Forest achieves ~99% accuracy and ~0.98 F1 score.
5. **Cross‑Validation**:
   Cross-Validation F1 Scores: [0.9844 0.9850 0.9847],Cross‑validation confirms strong generalization.
   Mean F1 Score: 0.9847
   This shows excellent generalization performance.
6.**Model Evaluation**
   precision    recall  f1-score   support
0       0.97      1.00      0.99     56750
1       1.00      0.97      0.99     56976
accuracy                           0.99
7.**.Confusion Matrix**
Shows extremely low false positives and false negatives.
8.Feature Importance
These features have the strongest influence on fraud detection.
Feature	Importance
V14	0.211
V10	0.150
V4	0.097
V12	0.095
V11	0.086
V17	0.080
V16	0.078
9**.Correlation Heatmap**
A heatmap was generated to visualize relationships between features.
This helps identify redundant or highly correlated variables.

   
