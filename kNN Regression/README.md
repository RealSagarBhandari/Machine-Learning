# kNN Regression & Cross Validation

## Project Overview
The main goal of this project is to implement a **kNN (k-Nearest Neighbors) Regression** algorithm and rigorously evaluate its performance using **Cross-Validation** techniques. The task is to predict continuous target variables, specifically predicting car prices utilizing the `Car_Price_Prediction.csv` dataset.

**kNN Regression** is a non-parametric supervised learning algorithm. Because it makes no underlying assumptions about the data distribution, it predicts the value of a continuous dependent variable purely based on the local neighborhood of the independent variables within the feature space.

## Cross Validation
Cross-validation is implemented to reliably evaluate the machine learning model. Instead of relying on a single static train-test split, the data is partitioned into multiple folds. This ensures every data point gets a chance to be in the test set exactly once, yielding a more robust and less biased performance estimate on unseen data.

## Evaluation Metrics
The regression model's fidelity is primarily tracked using two key metrics:
- **Mean Absolute Error (MAE):** The average of the absolute differences between the predicted and actual values. This provides a clear interpretation of error in the same units as the target variable without overly penalizing massive outliers.
- **Mean Squared Error (MSE):** The average of the squared differences between the predicted and actual values. This is heavily penalized for large errors, thereby ensuring the model avoids significant individual prediction deviations.

---
**File:** `kNN Regression.ipynb`  
**Dataset:** `Car_Price_Prediction.csv`
