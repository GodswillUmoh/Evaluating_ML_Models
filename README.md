# Evaluating Machine Learning Models
>Evaluating Machine Learning Models refers to the process of assessing the performance of a machine learning algorithm on a given dataset. This involves measuring how well the model makes predictions on unseen data (i.e., generalizes) and determining whether it meets the desired performance metrics.

## Why Evaluate ML Models?
> + Measure Performance: To determine how well the model predicts outcomes.
> + Avoid Overfitting/Underfitting: Ensures the model is neither too complex nor too simple.
> + Model Comparison: Helps in selecting the best model among multiple algorithms.
> + Real-World Impact: Validates that the model performs reliably in practical applications.

## R-Square (Coefficient of Determination)
> R-Square is a statistical measure that indicates how well a regression model explains the variability of the dependent variable (𝑦).
$R 
2
 =1− 
TSS/
RSS
​
$
> Where:
+ 𝑅𝑆𝑆 = Residual Sum of Squares (error in predictions)
+ 𝑇𝑆𝑆 = Total Sum of Squares (total variance in 𝑦)

## Residual Sum of Squares (RSS) and Total Sum of Squares (TSS)
_Both RSS and TSS are key concepts in regression analysis. They measure different aspects of how well a regression model fits the data._

### 1. Total Sum of Squares (TSS)
> TSS represents the total variance in the dependent variable (y) and measures how far the actual values (𝑦𝑖) are from the mean of the dependent variable (𝑦ˉ).
+ [See formula for TSS, Click to View](https://ibb.co/pbZ4vVV)
  
#### Explanation:
> + It captures the overall variability in the dataset.
> + Larger TSS means more variability in the dependent variable.

### 2. Residual Sum of Squares (RSS)
> RSS measures the error in the regression model. It is the sum of the squared differences between the actual values (𝑦i) and the predicted values ($𝑦^𝑖$) from the regression model.
> + [See formula for RSS, click to view](https://ibb.co/mNhzP5f)

