# Customer Loyalty Prediction with Logistic Regression

This project predicts customer loyalty using demographic and loyalty data. The logistic regression model achieves an accuracy score of **0.8054**.

## Workflow

1. **Data Preprocessing**
   - Unnecessary columns like `ID` are dropped.
   - Missing values in categorical features are filled with the mode.
   - Label encoding is applied to categorical columns (`DemClusterGroup`, `DemGender`, `DemReg`, `DemTVReg`, `LoyalClass`).
   
2. **Multicollinearity Check**
   - The `Variance Inflation Factor (VIF)` is calculated to check for multicollinearity in predictor variables.

3. **Model Training and Testing**
   - A logistic regression model is used to classify customer loyalty.
   - The dataset is split into training and test sets (`80-20` ratio).
   - Model training is performed on the training set, and predictions are made on the test set.
   - The model's accuracy on the test set is **0.8054**.

4. **Results and Export**
   - Confusion matrix and accuracy score are displayed.
   - Prediction probabilities for each class are saved to `Final_test_dataset.xlsx` along with actual test outcomes and test features.


## Technologies

- `pandas`, `numpy`, `scikit-learn`, `statsmodels`, `joblib`.
