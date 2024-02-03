# Concrete Strength Prediction

Predicting the strength of concrete in megapascals (MPa) for use in large-scale construction projects.

## Dataset Analysis Overview

- The dataset consists of 1036 samples with 8 features.
- The data points exhibit wide variations between min and max values.
- More than 55% of tested cement does not contain ash in the mix.
- About 46% of cement does not have slag, while superplastic additive was absent in about 37% of tested cement.
- Approximately 40% of the cement mixes were aged for just about a month.
- Overall, the mix ratios were not uniformly distributed, suggesting no linear relationship between concrete strength and ingredients.
- The dataset has no missing values, and all datapoints are complete.
- The variable 'age' seems to be the only non-floating continuous variable.

## Tools and Libraries Used

- Jupyter Notebook
- Google Colab
- Python Libraries:
  - NumPy
  - Pandas
  - Matplotlib
  - Seaborn
  - Sweetviz
  - XGBoost

## Models Used

- Linear Regression (LR)
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Decision Tree (DT)
- Random Forest (RF)
- Ridge Regressor (RR)
- Gradient Boosting (GB)
- XGBoost (XGB)
- Artificial Neural Network (ANN)

## Evaluation Metrics

We employed the following primary evaluation metrics:

- **Mean Squared Error (MSE):** Measures the average squared difference between actual and predicted values.
- **Mean Absolute Error (MAE):** Measures the average absolute difference between actual and predicted values.
- **Mean Absolute Percentage Error (MAPE):** Measures the percentage difference between actual and predicted values.
- **R-squared (R²):** Measures the proportion of the variance in the dependent variable that is predictable from the independent variables.

## Model Comparison

Observations:

- Random Forest (RF) achieved the lowest MSE, indicating superior performance in minimizing squared differences between predicted and actual values.
- Gradient Boosting (GB) and XGBoost (XGB) showed high R² values, suggesting a good fit to the data.
- Support Vector Machine (SVM) demonstrated competitive performance across multiple metrics.

# Conclusion

In this study, we aimed to predict concrete strength in megapascals (MPa) using various regression models. We considered three models: Linear Regression, Random Forest Regressor, and XGBoost Regressor. The following summarizes our key findings:

1. **Model Performance:**
   - All three models demonstrated reasonable predictive performance, as indicated by evaluation metrics on the test set.
   - The XGBoost Regressor achieved the lowest Mean Squared Error (MSE), suggesting superior accuracy in predicting concrete strength.
   - Random Forest Regressor also performed well, while Linear Regression showed competitive results.

2. **Hyperparameter Tuning:**
   - Hyperparameter tuning was performed to optimize the models further.
   - XGBoost Regressor benefited significantly from tuning, resulting in improved performance.

3. **Model Strengths and Weaknesses:**
   - Linear Regression, despite its simplicity, provided a good baseline performance.
   - Random Forest Regressor demonstrated robustness and resilience to overfitting, producing consistent results.
   - XGBoost Regressor, with careful hyperparameter tuning, outperformed other models, showcasing its ability to capture complex patterns in the data.

4. **Recommendations:**
   - For simplicity and interpretability, Linear Regression may suffice in scenarios where predictive accuracy is not the sole focus.
   - Random Forest Regressor is a reliable choice, offering a good balance between interpretability and performance.
   - XGBoost Regressor, with its powerful modeling capabilities, is recommended when high accuracy is crucial, and the interpretability trade-off is acceptable.
