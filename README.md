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
+ [See graphical Representation, Click to View](https://ibb.co/5KJJ7Vm)
  
#### Explanation:
> + It captures the overall variability in the dataset.
> + Larger TSS means more variability in the dependent variable.

#### Key Notes:
> + It doesn't consider the regression model, just the data.
> + It serves as the baseline for comparison.

### 2. Residual Sum of Squares (RSS)
> RSS measures the error in the regression model. It is the sum of the squared differences between the actual values (𝑦i) and the predicted values ($𝑦^𝑖$) from the regression model.
> + [See formula for RSS, click to view](https://ibb.co/mNhzP5f)
> + [See graphical Representation, Click to View](https://ibb.co/5KJJ7Vm)

#### Explanation:
> + Smaller RSS indicates a better fit because the predicted values are closer to the actual values.
> + It measures the "unexplained variance" in the model.

#### Key Notes:
> + RSS will be zero for a perfect fit (rare in real-world scenarios).
> + Overfitting may lead to a very low RSS but poor generalization.

## Basic Rule to Note:
### If Your R-Square is: 
+ 1.0 = Perfect fit (Suspicious)
+ 0.9 is Very Good
+ less than 0.7 Not Great
+ Less than 0.4 is terrible model
+ less than 0 maans model makes no sense for the data

## Adjusted R-Squared
> Adjusted R-Squared is a modified version of 𝑅2 that adjusts for the number of predictors (independent variables) in the model. It accounts for the fact that adding more predictors can artificially inflate 𝑅2.
> + [See Formula for Adjusted Squared, Click to View](https://ibb.co/M54WcqD)
>   
>   Where:
> + 𝑅2 : Coefficient of determination.
> + 𝑛: Number of data points (observations).
> + 𝑘: Number of predictors (independent variables).
