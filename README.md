# Task-4-Classification-with-Logistic-Regression.

Task 4: Logistic Regression Classifier
Objective
Build a binary classifier using Logistic Regression to predict whether a tumor is malignant or benign using diagnostic features. The task includes model training, evaluation, threshold tuning, and visualizing the underlying mechanics.

Project Contents
data.csv — Original dataset ( Breast Cancer Wisconsin ) used for this model
logistic_classifier.py — Python script for all preprocessing + visualizations + Linear Regression
Visual Images — Folder containing all visual plots
README.md — This documentation
Dataset
Dataset: Breast Cancer Wisconsin
Target Column: diagnosis

M → Malignant (1)
B → Benign (0)
Features: 30 numeric columns representing various measurements
Tools Used
Python
pandas, numpy
matplotlib, seaborn
scikit-learn
Workflow
1. Load & Explore the Dataset
Dropped irrelevant columns (id, unnamed)
Converted diagnosis labels: M → 1, B → 0
Verified no missing values
Checked class distribution
Visual 1: Class Distribution Bar Plot
Shows data imbalance between benign and malignant cases

Class Distribution

2. Data Exploration
Analyzed feature relationships using a heatmap
Identified correlation patterns and potential redundancy
Plotted histograms of key features
Visual 2: Correlation Heatmap
Visualizes feature interdependencies

Feature Correlation Matrix

Visual 3: Feature Histograms
Shows distributions of radius_mean, texture_mean, etc.

Feature Distribution

3. Preprocessing
Split data into training (80%) and test (20%) sets
Standardized features with StandardScaler
Why scaling?
It ensures features contribute equally and improves model convergence.

4. Model Training
Trained logistic regression model on scaled features
Used default parameters for interpretability
5. Model Evaluation
Evaluated using confusion matrix, classification report, ROC curve
AUC ≈ 0.99 indicates high separability
Visual 4: ROC Curve with AUC Score
Shows model performance across thresholds

ROC curve

6. Threshold Tuning
Changed classification threshold from 0.5 → 0.6
Reduced false positives, slightly affected recall
Used predict_proba() to manually adjust threshold
7. Sigmoid Function
Plotted sigmoid function to demonstrate probability mapping
Visual 5: Sigmoid Function Plot
Shows how input is transformed into a probability (0–1)

Sigmoid Function

Interview Concepts
Concept	Explanation
Logistic vs Linear	Logistic → classification (probabilities), Linear → continuous output
Sigmoid Function	Maps real input to (0, 1) — used for probability output
Precision vs Recall	Precision = TP / (TP + FP), Recall = TP / (TP + FN)
ROC-AUC	AUC shows overall model performance; closer to 1 is better
Confusion Matrix	Table showing TP, TN, FP, FN
Imbalanced Data	Accuracy may be misleading — prefer AUC, F1-score
Threshold Tuning	Helps balance sensitivity and specificity
Logistic for Multi-Class?	Yes, with One-vs-Rest or Softmax strategies
Insights & Anomalies
Radius and perimeter are highly correlated with malignancy
Dataset is clean and balanced enough for model training
A few outliers seen in area_worst and texture_worst
Conclusion
Successfully implemented a binary classifier using logistic regression
Achieved high performance (AUC ~ 0.99) and demonstrated model interpretability
Explored threshold tuning, feature scaling, and sigmoid behavior
Covered all core interview topics for binary classification tasks
