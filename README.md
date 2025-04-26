# Fraudulent Insurance Claim Detection

## Project Overview

In this project, I worked on building a machine learning model to help detect fraudulent insurance claims.  
The idea was to spot suspicious claims early and help the business save costs.

We used real-world claim data that included policy details, vehicle information, and incident descriptions.  
Our target was simple: figure out if a claim was fraudulent or not.

---

## Steps I Followed

1. **Data Cleaning**
   - Removed unnecessary columns like IDs, dates, and locations that didn’t help in prediction.
   - Handled missing values to clean up the data properly.

2. **Exploratory Data Analysis (EDA)**
   - Looked at how each feature was distributed.
   - Checked how fraud and non-fraud claims differ.
   - Visualized correlations to find strong and weak features.

3. **Feature Engineering**
   - Handled imbalance using SMOTE (since fraud cases were very few).
   - Created dummy variables for categories.
   - Scaled numerical features to get them on the same scale.

4. **Model Building**
   - Built a Logistic Regression model first — simple and easy to interpret.
   - Also trained a Random Forest model — to capture complex patterns better.
   - Used Recursive Feature Elimination and feature importance to select the best features.

5. **Model Evaluation**
   - Plotted ROC curves.
   - Found the best threshold (cutoff) for Logistic Regression.
   - Compared models based on Accuracy, Precision, Recall, F1-score, and ROC-AUC.

---

## Final Outcome

- **Random Forest** turned out to be the better model.
- It gave better Recall, Precision, and overall AUC compared to Logistic Regression.
- So, I recommend using the Random Forest model with a 0.45 cutoff for predicting frauds.

---

## Tools Used

- Python (Pandas, NumPy)
- Matplotlib, Seaborn (for visualization)
- Scikit-learn (for modeling)
- Imbalanced-learn (for SMOTE)

---
