# Hybrid-Regression-Classification-Model-for-Credit-Default-Risk
This project applies classification and regression models to predict loan defaults and estimate associated risk, enabling better credit risk analysis. 
The classification model predicts whether a customer is likely to default on a loan, while the regression model estimates the potential financial loss. This combined approach provides a more comprehensive understanding of credit risk.
The major objectives of this project is to find the default probability.
I have used Random Forest(Classification) and Ridge Regression(Regression).
NOTE: As the dataset was very large, we can acces it from(https://www.kaggle.com/datasets/wordsforthewise/lending-club)
Main Libraries used for this project:
- **Pandas** → Data manipulation and analysis  
- **NumPy** → Numerical computations  
- **Scikit-learn (sklearn)** → Machine learning models and utilities  
  - `LabelEncoder` → Encoding categorical variables  
  - `StandardScaler` → Feature scaling  
  - `train_test_split` → Splitting data into training and testing sets  
  - `Pipeline` → Building ML pipelines  
  - `RandomForestClassifier` → Classification model  
  - `Ridge` → Regression model  
  - Metrics:
    - `accuracy_score`
    - `precision_score`
    - `recall_score`
    - `f1_score`
    - `confusion_matrix`
    - `roc_auc_score`
    - `r2_score`
    - `mean_squared_error`

---
