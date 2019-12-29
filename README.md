# Predict the Sale Price of House

## Work Flow:
First the presence of Null Values is checked. Since, the features 'Alley', 'PoolQC', 'Fence' and 'MiscFeature' has too many null values, it can be dropped. Also the 'Id' feature is not for required for model created, it is also dropped.
Next Categorical Data is converted to Numerical Data using get_dummies. Null Values are imputed with the Median Values using the Imputer. Skewness has been addressed by Log transformation. Changing the infinity values generating by Log transformation to zero. Since there are too many features which are correlated, Prinicipal Component Analysis has been done. Various Regressors such as Linear, Ridge, Lasso, RandomForest, AdaBoost and Bagging Regressors are applied. Ridge Regressor Model gives Highest Regressor Score, hence it is chosen to predict the Sale Price of House    
