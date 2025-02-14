# Module 20 Challenge: Supervised Machine Learning

## Overview of the Analysis

The purpose of this analysis was to build and evaluate machine learning models to predict loan status (healthy vs. high-risk loans). The dataset contained financial information about borrowers, and the goal was to determine whether a loan was high-risk (1) or healthy (0).

# Data Overview:
-Target Variable: loan_status (0 = Healthy, 1 = High-Risk)
- Machine Learning Stages:
    - Data preprocessing (splitting features and labels)
    - Training and testing machine learning models
    - Evaluating performance metrics (accuracy, precision, recall, F1-score)

# Models Used:
- Logistic Regression was selected as the primary model for this classification task.

## Results
The high recall (0.94) for high-risk loans indicates that the model effectively identifies at-risk borrowers, though its precision (0.86) suggests some false positives (healthy loans flagged incorrectly as high-risk).
 
Logistic Regression Model Performance:
- Accuracy: 99%
- Precision:
    - Healthy Loans (0): 1.00
    - High-Risk Loans (1): 0.86
- Recall:
    - Healthy Loans (0): 0.99
    - High-Risk Loans (1): 0.94
- F1-score:
    - Healthy Loans (0): 1.00
    - High-Risk Loans (1): 0.90

## Summary
# Key Findings:
- The Logistic Regression model performed very well, achieving 99% accuracy
- The model was highly effective at identifying healthy loans (0) with 1.00 precision and 0.99 recall
- For high-risk loans (1), the model correctly identified 94% of actual high-risk cases (high recall), but the precision was 0.86, meaning some healthy loans were misclassified as high-risk

# Recommendation:
- The Logistic Regression model is effective, but misclassifying healthy loans as high-risk could lead to lost lending opportunities
- If correctly identifying high-risk loans is the priority, this model is acceptable as it captures 94% of all actual high-risk loans
- If reducing false positives (misclassifying healthy loans) is crucial, then possible solutions to reduce false positives are:
    - Hyperparameter tuning (e.g., adjusting class weights)
    - Alternative models (e.g., Decision Trees, Random Forest)
    - Balancing techniques (oversampling high-risk loans to improve precision)

Overall, the Logistic Regression model is a strong candidate, but additional fine-tuning might improve precision for high-risk loans.
