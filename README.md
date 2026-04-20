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
After loading the data we need start cleaning the dataset:
- Check and remove columns with high missing values.
- Handled missing data using mean for numeric columns.
- Encoded categorical variables using Label Encoding. 
-Dividing the dataset into Feature columns and Output columns.

  Dividing the large dataset to training dataset and testing dataset. Now we can apply ML Models to it.

## Models Used

###  1. Random Forest Classifier
Used to predict whether a loan will default.

Reasons to choose this model: 
- Handles non-linear relationships well.
- Works effectively with tabular data.
- Robust to noise and overfitting.

Output:
- Predicted class (0 or 1)
- Probability of default (P(Default))

### 2. Ridge Regression 
Used to estimate the potential loss amount associated with a default.

Reasons to choose this model: 
- Handles multicollinearity in financial features.
- Provides stable predictions with regularization.
- Easy to interpret.

# Evaluation Metrics

# Classification Metrics:
1. Accuracy → Overall correctness
2. Precision → Correctness of positive predictions
3. Recall → Ability to detect defaulters
4. F1 Score → Balance between precision and recall
5. Confusion Matrix → Detailed prediction breakdown
6. ROC-AUC Score → Model’s ability to distinguish classes

# Regression Metrics
1. R² Score → Model fit quality
2. Mean Squared Error (MSE) → Prediction error

By seeing the Evaluation Metrics we can understand that models i.e the Random Forest give the maximum accuracy and precision thus is the best to be used for default probability prediction.
