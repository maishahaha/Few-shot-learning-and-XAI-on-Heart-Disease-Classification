# Few-Shot Learning and XAI on Heart Disease Classification

This project implements a heart disease prediction model designed for clinical settings with limited data. It combines a simple, distance-based classifier with explainable AI tools to ensure predictions are both accurate and easy for doctors to understand.

## Key Features

* **Small Data Focus**: The model is trained on only 20% of the available data to prove it works even when patient records are scarce.


* **High Performance**: Achieved ~78% accuracy and an 0.82 ROC-AUC score.


* **Explainable AI (XAI)**: Uses SHAP and LIME to show exactly which health factors (like heart rate or cholesterol) led to a specific prediction.


* **Simple Design**: Uses K-Nearest Neighbors (KNN), an algorithm that mimics how doctors compare new patients to similar past cases.



## Clinical Predictors

The model identifies several key factors that most impact heart disease risk:

* Number of major vessels 


* ST depression 


* Thallium test results 


* Maximum heart rate 



## How it Works

1. **Preprocessing**: Cleans the data, fixes outliers, and scales features so they can be compared fairly.


2. **Training**: Uses a "Few-Shot" strategy to learn from a small, balanced set of patient examples.


3. **Prediction**: The KNN classifier finds the most similar patients in the training set to diagnose a new case.


4. **Explanation**: SHAP and LIME generate visual reports explaining the logic behind the result.



## Results

| Metric | KNN Model | Nearest Centroid |
| --- | --- | --- |
| **Accuracy** | 77.3% | 75.0% |
| **ROC-AUC** | 0.82 | 0.79 |
| **Explainability** | Medium | High |
