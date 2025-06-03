Churn Prediction: Addressing Class Imbalance and Model Performance
Project Overview
This project focuses on predicting customer churn using machine learning techniques, with special emphasis on addressing the class imbalance problem. Customer churn significantly impacts business revenue and retention, making accurate churn prediction crucial.

Objectives
Train a baseline model without handling class imbalance and evaluate its performance.

Investigate the class imbalance in the dataset and its impact on model predictions.

Implement multiple approaches to handle class imbalance, including class weighting and random oversampling.

Train and compare different machine learning models, tuning hyperparameters for improved performance.

Draw conclusions on the best strategy for churn prediction with imbalanced data.

Dataset
The dataset includes customer demographic details, account information, and the churn status (target variable). Key preprocessing steps include:

Dropping irrelevant columns

Encoding categorical variables

Handling missing and infinite values

Scaling numerical features

Methodology
Baseline Model: Train a Random Forest model without addressing class imbalance and evaluate using F1-score and AUC-ROC metrics.

Class Imbalance Handling:

Calculate and apply class weights in the Random Forest model.

Use random oversampling of the minority class with Logistic Regression to balance the training data.

Hyperparameter Tuning: Perform grid search on the Random Forest model with class weights to find optimal parameters and improve model performance.

Results
The baseline model showed moderate performance.

Applying class weights slightly improved F1-score and AUC-ROC, indicating better minority class prediction.

Random oversampling with Logistic Regression performed worse than Random Forest models in this scenario.

Hyperparameter tuning further improved the Random Forest model’s metrics.

Conclusion
Handling class imbalance is essential to enhance prediction accuracy, especially for minority classes like churned customers. The best results were achieved by tuning a Random Forest model with class weights. Further experiments with additional imbalance techniques and models may yield even better performance.

Notes
This project follows best practices for structuring, documenting, and evaluating machine learning workflows.

Reviewer feedback was incorporated iteratively to improve code structure, modeling approaches, and evaluation rigor.
