# Diabetes-Prediction-using-K-Nearest-Neighbors-KNN-

📘 Project Overview

This project focuses on building a K-Nearest Neighbors (KNN) classification model to predict whether a person is diabetic or not based on key health indicators. The goal is to use data-driven insights to support early diagnosis and prevention of diabetes — one of the most common global health challenges.

🎯 Objective

To develop and evaluate a KNN classification model that accurately predicts the likelihood of diabetes, achieving a strong balance between precision, recall, and F1-score across training and testing datasets.

🧩 Dataset Description

The dataset includes various medical and physiological parameters related to diabetes diagnosis.

Features Used:

Pregnancies – Number of times pregnant

Glucose – Plasma glucose concentration

BloodPressure – Diastolic blood pressure (mm Hg)

SkinThickness – Triceps skin fold thickness (mm)

Insulin – Serum insulin (mu U/ml)

BMI – Body mass index (weight/height²)

DiabetesPedigreeFunction – Family history measure

Age – Age in years

Target Variable:

Outcome: 1 → Diabetic, 0 → Non-Diabetic

⚙️ Technologies Used

Language: Python 🐍

Libraries:

pandas – Data manipulation and cleaning

numpy – Numerical computation

matplotlib / seaborn – Data visualization

scikit-learn – Model building and evaluation

🧮 Model Development Process

Data Preprocessing

Handled missing and invalid values (e.g., zero glucose or insulin)

Normalized data using StandardScaler

Split the dataset into training and testing sets

Model Building

Implemented K-Nearest Neighbors (KNN) from sklearn.neighbors

Tuned the optimal value of K using cross-validation and the elbow method

Model Evaluation

Measured performance using Precision, Recall, and F1-score

Analyzed confusion matrix for misclassification insights

📊 Model Performance
Dataset	Precision	Recall	F1-Score
Train	  0.82	    0.89	  0.85
Test	  0.74	    0.62	  0.67

✅ The model performs consistently with strong recall on training data, indicating high sensitivity to detecting diabetic patients. Although the test scores are slightly lower, the results demonstrate reasonable generalization.

🔍 Insights

Glucose, BMI, and Age have the strongest correlation with diabetes outcome.

Proper data scaling significantly impacts KNN accuracy.

A higher K value can improve model stability but may reduce sensitivity.

Healthcare ML models should prioritize recall to minimize missed positive cases.

📈 Visualizations

Correlation Heatmap – Shows relationships among features

Confusion Matrix – Displays true vs. predicted classifications

Elbow Plot – Helps find the optimal K value

ROC Curve – Evaluates classification performance
