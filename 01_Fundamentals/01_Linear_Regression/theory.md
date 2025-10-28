# 1- Linear Regression

## 1.1- Theory

### What is Linear Regression?
Supervised learning algorithm used to model the relationship between a dependent variable (target) and one or more independent variables (features). Assumes linear relationship between inputs and output.

### Mathematical Foundation

#### Simple Linear Regression:
$$ y = \beta_0 + \beta_1x + \epsilon $$

**Where:**
- $y$ = dependent variable (target)
- $x$ = independent variable (feature)  
- $\beta_0$ = y-intercept (bias term)
- $\beta_1$ = slope coefficient (weight)
- $\epsilon$ = error term (residual)

#### Multiple Linear Regression:
$$ y = \beta_0 + \beta_1x_1 + \beta_2x_2 + \dots + \beta_nx_n + \epsilon $$

### Cost Function: Mean Squared Error (MSE)
$$ MSE = \frac{1}{n} \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 $$

**Purpose:** Measures quality of predictions by calculating average squared differences between actual and predicted values.
  - Goal: Find parameters (β₀, β₁) that minimize MSE
  - Can be optimized using:
    - **Ordinary Least Squares (OLS)** - Analytical solution (closed-form)
    - **Gradient Descent** - Iterative optimization approach

### Optimization Methods
- **Ordinary Least Squares (OLS):** Analytical solution that finds optimal parameters directly
- **Gradient Descent:** Iterative approach suitable for large datasets

**Evaluation Metrics:**
  - R-squared (R²) - Proportion of variance explained
  - Mean Absolute Error (MAE)
  - Root Mean Squared Error (RMSE)