# Introduction
Diabetes is one of the fastest-growing health challenges worldwide. Early detection can help reduce risks and improve patient outcomes. In this project, we explore how machine learning models can be applied to predict diabetes using real-world clinical data collected from Iraqi hospitals and medical centers. In the previous article, we used a dataset with most of its features not gotten as a result of laboratory investigation. The dataset can be accessed from here.

## Dataset Overview
The dataset was curated from patient records in Baghdad’s medical institutions. It includes demographic details and medical test results:

* **Demographics:** Age, Gender
* **Medical Tests:** Blood sugar, Creatinine ratio, BMI, Urea, Cholesterol, Lipid profile (LDL, VLDL, HDL), Triglycerides, HbA1C
* **Target Classes:** Diabetic, Non-Diabetic, Predict-Diabetic
This combination of clinical and demographic data provides a comprehensive foundation for prediction.

## Methodology
1. Data Preprocessing
In this project, the dataset was used as-is without applying steps such as handling missing values, categorical encoding, or feature scaling as there was no need for such.

2. Exploratory Data Analysis (EDA)
Basic dataset exploration using .info() and .describe() in Python to understand structure and summary statistics
3. Machine Learning Models
I trained multiple models:

* Random Forest
* XGBoost
* LightGBM
4. Model Tuning & Evaluation
* Hyperparameter optimization with RandomizedSearchCV
* Performance metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix
<img width="821" height="318" alt="image" src="https://github.com/user-attachments/assets/6fd3861d-27d5-4331-9895-90b6c048964b" />

Comparison of model accuracy before and after hyperparameter tuning.

## Key Findings
* The models tested showed varying performances with Random Forest and boosting methods generally giving stronger results than the others.
* Tuned LightGBM model was the best performing model with 100% accuracy score.
* Feature importance analysis revealed that HbA1C, Age and BMI were the most important predictive factors.
## Conclusion
This case study highlights how machine learning can be applied to predict diabetes, offering significant potential for early detection and decision support in healthcare. With further refinement and real-world deployment, such models could play a crucial role in clinical practice.

## Next Steps
Future improvements could include:

Expanding the dataset with more diverse patient samples
Incorporating deep learning models
Building a user-friendly web or mobile app for real-time predictions
