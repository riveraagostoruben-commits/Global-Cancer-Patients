# Global Cancer Patient Severity Classification

Project Summary

This project leverages a decade of global cancer patient data (2015–2024) to build a predictive system for classifying patient severity. The goal is to provide a machine learning framework that can assist in clinical decision-making by identifying high-risk cases based on patient demographics and clinical data.

 Technical Workflow
 
- Data Ingestion: Automated dataset retrieval using `kagglehub`.
- Feature Engineering: Implemented a custom `ColumnTransformer` pipeline to handle automated One-Hot Encoding for categorical variables.
- Problem Transformation: Converted a regression-based target into a multi-class classification problem via custom binning logic.

 Machine Learning Models
 
I evaluated five different classification architectures to identify the most robust performer:
- Random Forest Classifier
- XGBoost (Extreme Gradient Boosting)
- Gradient Boosting Machine
- Logistic Regression
- Support Vector Classification 

Evaluation & Results

Each model was evaluated using:
1. Accuracy: To measure overall correctness.
2. Confusion Matrices: To visualize True Positives vs. False Positives across severity classes.
3. F1-Score/Recall: Critical in healthcare contexts to ensure high-severity cases are not missed (minimizing false negatives).

Technologies 
- Python
- Scikit-Learn
- XGBoost
- Matplotlib & Seaborn
