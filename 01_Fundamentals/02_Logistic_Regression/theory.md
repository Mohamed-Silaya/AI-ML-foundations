# Logistic Regression 


## Introduction

**Logistic Regression** is a statistical method and machine learning algorithm used for **binary classification** problems.  
Despite its name containing *“regression”*, it is primarily used for **classification tasks** where the outcome is categorical.

### Key Characteristics
- Supervised learning algorithm  
- Probabilistic output (0 to 1)  
- Linear classification boundary  
- Interpretable results  

---

## Core Concepts

### Sigmoid Function

The sigmoid function maps any real-valued number to a value between 0 and 1:

$$
\sigma(z) = \frac{1}{1 + e^{-z}}
$$

**Properties**
- Range: (0, 1)  
- S-shaped curve (S-curve)  
- Symmetric around zero  
- Derivative:  
  $$
  \sigma'(z) = \sigma(z)(1 - \sigma(z))
  $$

---

### Decision Boundary
- Linear decision boundary in feature space  
- Separates classes based on probability threshold  
- Default threshold: **0.5** (can be tuned)

---

### Probability Interpretation
- Output represents \( P(y=1|x) \)  
- Complementary probability: \( P(y=0|x) = 1 - P(y=1|x) \)

---

## Mathematical Foundation

### Hypothesis Function

$$
h_\theta(x) = \sigma(\theta^T x) = \frac{1}{1 + e^{-\theta^T x}}
$$

Where:  

- \( \theta = [\theta_0, \theta_1, ..., \theta_n] \) (parameters)  
- \( x = [1, x_1, ..., x_n] \) (features)  
- \( \theta^T x = \theta_0 + \theta_1x_1 + ... + \theta_nx_n \)

---

### Cost Function: Binary Cross-Entropy

$$
J(\theta) = -\frac{1}{m} \sum [y^{(i)} \log(h_\theta(x^{(i)})) + (1 - y^{(i)}) \log(1 - h_\theta(x^{(i)}))]
$$

Where:  
- \( y^{(i)} \): Actual label (0 or 1)  
- \( h_\theta(x^{(i)}) \): Predicted probability  
- \( m \): Number of samples  

---
