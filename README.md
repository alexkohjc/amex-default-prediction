# amex-default-prediction

This notebook will focus on optimizing the worst performing algorithm (Support Vectors) to showcase improvement in metrics after hyperparams optimization
I'll only be using 5K records for faster run-times

After hyperparams optimization:
- f1-score: 0.80 -> 0.89
- recall: 0.68 -> 0.74 (focusing on recall to reduce false negatives to catch more defaults; but if biz objective is to increase # of clients who can get loans, we could focus on precision instead)

## Skillsets used
- EDA
  - drop highly-correlated variables
- data cleaning/transformation
  - handle missing values
  - variable scaling
  - variable encoding
- Dimension Redux using PCA to reduce collinearity
  - scree plot to choose # of components
- ML models
  - Support Vectors
  - Random Forest
  - XGBoost
- model eval
  - confusion matrix
- model optimization
  - k-fold cross-validation
  - hyperopt as opposed to gridsearchCV
    - optimize the 'C', 'kernel' and 'gamma' of Support Vectors algo
- model interpretation
  - xgboost feature importance
  - xgboost shapley values
- others
  - sample code for Siamese Neural Networks with Triplet Loss
