# Linear Regression

Linear Regression is one of the simplest and most widely used algorithms in machine learning. It’s often the first algorithm people learn because of its interpretability and foundational concepts.

---

## What is Linear Regression?

Linear regression is a **supervised learning** algorithm used to **predict continuous numeric values** based on the linear relationship between input features and output.

It tries to fit a straight line (or hyperplane in higher dimensions) through the data that best represents the relationship between variables.

### Basic Equation:

For one feature (univariate):
```
y = mx + b
```
For multiple features (multivariate):
```
y = w₁x₁ + w₂x₂ + ... + wₙxₙ + b
```

Where:
- `y`: Predicted value
- `x`: Input feature(s)
- `w`: Weights (coefficients)
- `b`: Bias (intercept)

---

## Visual Example

Imagine a dataset of house prices based on square footage:

| Size (sqft) | Price ($) |
|-------------|-----------|
| 1000        | 150,000   |
| 1500        | 200,000   |
| 2000        | 250,000   |

Linear regression fits a line through these points to predict the price of a house with, say, 1700 sqft.

---

## Goal of Linear Regression

Find the line that **minimizes the difference** between the predicted and actual values.

This difference is measured using a **loss function**, commonly:

### Mean Squared Error (MSE):
```
MSE = (1/n) * Σ(ŷᵢ - yᵢ)²
```
Where:
- `ŷᵢ` is the predicted value
- `yᵢ` is the actual value

---

## Types of Linear Regression

### 1. **Simple Linear Regression**
- One input variable
- Predicts using a single line

### 2. **Multiple Linear Regression**
- More than one input variable
- Uses a hyperplane for prediction

### 3. **Regularized Linear Regression**
Adds a penalty term to avoid overfitting.

- **Ridge Regression** (L2 regularization)
- **Lasso Regression** (L1 regularization)
- **Elastic Net** (Combination of L1 and L2)

---

## Assumptions of Linear Regression

Linear regression makes several key assumptions:

✅ Linearity: Relationship between features and target is linear  
✅ Homoscedasticity: Equal variance of residuals  
✅ Independence: Observations are independent  
✅ Normality: Residuals are normally distributed  
✅ No multicollinearity: Features are not highly correlated with each other

Violating these assumptions may lead to inaccurate models.

---

## How It's Trained

1. **Initialize weights and bias** (often to 0)
2. **Make predictions**: `ŷ = w·x + b`
3. **Calculate loss** using MSE
4. **Update weights** using gradient descent:
   ```
   w = w - α * ∂Loss/∂w
   b = b - α * ∂Loss/∂b
   ```
   Where `α` is the learning rate.

Repeat until the loss converges.

---

## Evaluation Metrics

For regression problems like linear regression, use:

- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **R² Score**: Measures proportion of variance explained by the model

---

## Advantages

✅ Easy to implement and interpret  
✅ Fast and efficient  
✅ Works well with linearly separable data  
✅ Provides insights into feature importance via coefficients

---

## Disadvantages

❌ Assumes a linear relationship  
❌ Sensitive to outliers  
❌ Poor performance on complex nonlinear problems  
❌ Can overfit if many features are used without regularization

---

## Use Cases

- Predicting housing prices  
- Estimating demand or sales  
- Forecasting expenses or revenue  
- Modeling relationships in scientific research

---

## Summary

Linear Regression is a fundamental algorithm that lays the groundwork for understanding more complex models. It’s best suited for:

- Problems where the relationship between variables is approximately linear
- Interpretability and quick baselines

> Tip: Try implementing Linear Regression in Python using libraries like `scikit-learn`, or from scratch using `NumPy` for hands-on understanding.
