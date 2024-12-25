# ML_Heart_Disease_Pred


Project Overview

This project focuses on analyzing patient health data to predict the potential presence of heart disease using machine learning techniques. 
The project is structured to provide actionable insights to hospitals, enabling early diagnosis and prevention of life-threatening conditions.
The project consists of three key tasks:

1.	Preparing a complete data analysis report.
   
2.	Building and evaluating machine learning models to predict heart disease.
   
3.	Providing recommendations to hospitals based on the predictions.
________________________________________

Dataset Description

The dataset contains 14 columns, including one unique identifier (patient_id) and 13 features related to patient health metrics and diagnostics:

•	slope_of_peak_exercise_st_segment (int): Slope of the peak exercise ST segment.

•	thal (categorical): Results of the thallium stress test (normal, fixed_defect, reversible_defect).

•	resting_blood_pressure (int): Resting blood pressure (mmHg).

•	chest_pain_type (int): Types of chest pain (4 categories).

•	num_major_vessels (int): Number of major vessels colored by fluoroscopy (0–3).

•	fasting_blood_sugar_gt_120_mg_per_dl (binary): Fasting blood sugar > 120 mg/dl (0: False, 1: True).

•	resting_ekg_results (int): Resting electrocardiographic results (0, 1, 2).

•	serum_cholesterol_mg_per_dl (int): Serum cholesterol (mg/dl).

•	oldpeak_eq_st_depression (float): ST depression induced by exercise relative to rest.

•	sex (binary): Gender (0: female, 1: male).

•	age (int): Patient's age (years).

•	max_heart_rate_achieved (int): Maximum heart rate achieved (bpm).

•	exercise_induced_angina (binary): Exercise-induced chest pain (0: No, 1: Yes).

________________________________________

Project Tasks

Task 1: Data Analysis

•	Performed exploratory data analysis (EDA) to understand the dataset, visualize relationships, and detect outliers or missing data.

•	Key observations:

o	Identified correlations between features such as age, maximum heart rate, and cholesterol levels with heart disease.

o	Detected and treated missing or inconsistent data.

o	Visualized distributions and feature relationships using plots and heatmaps.

Task 2: Predictive Modeling

•	Built and evaluated several machine learning models for predicting heart disease:

o	Logistic Regression

o	Decision Tree Classifier

o	Random Forest Classifier

o	Support Vector Machine (SVM)

o	XGBoost

•	Evaluation Metrics: Accuracy, Precision, Recall, F1-Score, ROC-AUC

•	Best Model: Random Forest Classifier achieved the highest ROC-AUC score and was selected as the recommended model for production.

Task 3: Recommendations to Hospitals

•	Developed actionable insights based on model predictions:

o	Identified high-risk groups based on age, cholesterol levels, and other metrics.

o	Suggested early screening and monitoring strategies for high-risk patients.

o	Highlighted the importance of controlling blood sugar levels and cholesterol to reduce risk factors.

________________________________________

Challenges and Solutions

Challenges Faced

1.	Imbalanced Dataset:
   
o	Problem: Class imbalance in the target variable (heart disease cases vs. non-cases).

o	Solution: Used techniques like SMOTE (Synthetic Minority Oversampling Technique) to balance the dataset.

2.	Missing and Inconsistent Data:
   
o	Problem: Missing values in some features.

o	Solution: Handled missing data using mean/mode imputation for numerical/categorical variables.

3.	Feature Scaling:
   
o	Problem: Variability in feature scales.

o	Solution: Applied standardization using StandardScaler for algorithms sensitive to feature scales (e.g., SVM).

4.	Model Overfitting:
    
o	Problem: Overfitting observed in complex models.

o	Solution: Used cross-validation and regularization techniques to improve generalization.
_______________________________________

Results and Recommendations

Model Comparison


![Screenshot (45)](https://github.com/user-attachments/assets/eb976971-2480-4ebc-9ab6-74c08ae47f3e)

•	Recommended Model: Random Forest Classifier is suggested for deployment due to its high accuracy and robustness.


________________________________________

Tools and Libraries Used

•	Data Analysis and Visualization: pandas, NumPy, Matplotlib, Seaborn

•	Machine Learning: scikit-learn, XGBoost, SMOTE

•	Jupyter Notebook: Used for combining data analysis, modeling, and visualization in a single environment.

