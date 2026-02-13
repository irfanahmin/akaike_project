Heart Disease Diagnostic Tool
This project provides a machine learning pipeline to predict heart disease using the Cleveland Clinic dataset. The solution focuses on delivering high predictive accuracy alongside clinical interpretability.

Key Features
Explainable AI: Utilizes feature importance and model coefficients to provide transparency for clinical decision-making.

Robust Validation: Employs Stratified 5-Fold Cross-Validation to ensure model stability across a small sample size of 297 patients.

Feature Engineering: Includes custom interaction terms, such as Age crossed with Blood Pressure, to capture non-linear risks.

Safety Audit: Analyzes False Negatives to evaluate the model's reliability as a clinical screening tool.

Performance Summary
Logistic Regression (Final Model): Mean F1-Score of 0.8168 and Mean AUC-ROC of 0.9136.

SVM: Mean F1-Score of 0.8163 and Mean AUC-ROC of 0.9542.

Random Forest: Mean F1-Score of 0.7843 and Mean AUC-ROC of 0.9063.

Logistic Regression was selected for final deployment because it provided the most stable performance and highest interpretability for medical use.

Clinical Insights
Risk Drivers: The most significant predictors of heart disease identified by the model are major vessel blockage (ca), asymptomatic chest pain (cp_3), and reversible defect thalassemia (thal_2).

Protective Factors: A higher maximum heart rate (thalach) achieved during testing is the strongest indicator of cardiovascular health.

Tech Stack
Language: Python

Libraries: Scikit-Learn, Pandas, Seaborn, Matplotlib

Repository Structure
notebooks/: Contains the end-to-end Google Colab solution.

data/: The heart disease dataset.

outputs/: Visualizations including the confusion matrix and ROC curves.
