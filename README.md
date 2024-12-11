Heart Failure Prediction

This repository contains a comprehensive analysis and prediction model for heart failure using machine learning techniques. The project leverages a dataset containing 299 records with 13 features to predict mortality due to heart failure.

Dataset Information:

Source: The dataset is based on research by Davide Chicco and Giuseppe Jurman: Machine learning can predict survival of patients with heart failure from serum creatinine and ejection fraction alone (BMC Medical Informatics and Decision Making 20, 16 (2020)).

Description: Contains 12 features relevant to cardiovascular conditions and a target feature (DEATH_EVENT) indicating survival.

Features: Include attributes such as age, ejection fraction, serum creatinine, platelets, and more.

Goal: Predict patient mortality due to heart failure.

Tasks Performed:
1. Data Cleaning and Preprocessing
Addressed null values and scaled features like platelets and creatinine phosphokinase using a Robust Scaler.
Categorized the age feature into three groups: Young, Middle-Aged, and Old.

2. Data Visualization
Analyzed feature relationships with the target variable (DEATH_EVENT) using visualizations like bar plots, violin plots, and box plots.
Key insights include the impact of ejection fraction, serum creatinine, and blood pressure on survival outcomes.

3. Statistical Hypothesis Testing
Conducted T-tests, chi-squared tests, and Spearman’s correlation to evaluate feature dependencies and their relevance to the target variable.

4. Feature Extraction
Applied Principal Component Analysis (PCA) to reduce the feature set from 12 to 7 components while retaining maximum variance.

5. Model Selection and Prediction
Selected a Random Forest Classifier for its efficiency and superior performance over XGBoost.
Implemented hyperparameter tuning using Randomized Search CV, achieving an accuracy of 76.67%.

Results:

Model Accuracy: 76.67%

Evaluation Metrics: Confusion matrix, precision, recall, and F1-score were computed to assess model performance.

Tools and Libraries used:

Python (pandas, numpy, sklearn)

Visualization: Seaborn, Matplotlib

Statistical Analysis: SciPy
