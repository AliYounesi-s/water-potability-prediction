# Water Potability Prediction

## Objective
To predict whether water is potable based on physicochemical properties using supervised machine learning models, with emphasis on evaluation metrics suitable for imbalanced data.

## Dataset
Public water quality dataset containing 3,276 samples and 9 numeric physicochemical features, including pH, sulfate concentration, chloramines, and turbidity.  
The target variable (potability) is moderately imbalanced (~61% non-potable, ~39% potable).

## Methods
- Data cleaning and median imputation for missing values
- Stratified train/test split (80/20)
- Feature scaling for linear models
- Classification models:
  - Logistic Regression (baseline)
  - Random Forest
- Hyperparameter tuning using GridSearchCV optimized for F1-score
- Model evaluation using precision, recall, confusion matrix, and F1-score

## Key Results
- Logistic Regression showed limited performance due to linear decision boundaries and class overlap
- Random Forest improved precision by capturing non-linear relationships
- F1-optimized Random Forest achieved a better balance between precision and recall, though performance remained constrained by overlapping feature distributions

## Interpretation
This dataset illustrates the importance of metric selection in health and safety-related classification problems.  
Depending on the application context, precision or recall may be prioritized to balance false positives and false negatives.

## Tools
Python, Pandas, NumPy, scikit-learn, Matplotlib

## Notes
This project focuses on analytical reasoning, model evaluation, and interpretation rather than maximizing predictive performance.
