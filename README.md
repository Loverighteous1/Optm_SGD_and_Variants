
# LAB: Stochastic Gradient Descent
The objective of this lab session is to implement and test:
- Stochastic gradient descent with constant stepsizes
- Stochastic gradient descent with shrinking stepsizes
- Stochastic gradient descent with sampling with/without replacement
- Stochastic gradient descent with averaging
- Stochastic gradient descent with momentum

and compare your implementation with gradient descent.


# Stochastic Gradient Descent (SGD) Analysis
This repository contains a Jupyter notebook that performs a detailed analysis of Stochastic Gradient Descent (SGD) and its various variants, including:
- SGD with constant stepsizes
- SGD with shrinking stepsizes
- SGD with averaging
- SGD with momentum (SGDm)
- Gradient Descent (GD)

## Overview

The notebook provides a comprehensive comparison of these optimization methods through convergence plots, highlighting their performance in terms of error reduction and computational efficiency.

## Convergence Plots Analysis

1. **SGD with constant stepsizes vs. SGD with shrinking stepsizes**:
    - Constant stepsizes show erratic behavior and do not converge well.
    - Shrinking stepsizes provide a steady reduction in error, achieving a lower final error.

2. **SGD with averaging**:
    - Averaging reduces variance in the updates, leading to significant drops in error, especially when averaging is applied in the later stages of training.

3. **SGDm (SGD with momentum)**:
    - Momentum accelerates convergence and smooths out oscillations, showing stable and consistent improvement.

4. **Gradient Descent (GD)**:
    - GD converges the fastest and achieves the lowest error due to full dataset gradient computations.

5. **Effect of Sampling without Replacement**:
    - Sampling without replacement helps in faster convergence within a single data pass, avoiding redundant updates.

## Computational Cost Comparison

- **GD** has a higher per-step computational cost but converges faster overall.
- **SGD** variants have lower per-step costs but require more steps to achieve similar convergence.

## Practical Recommendations

Combining the best practices from these methods, such as using SGD with momentum and averaging, can yield robust and efficient optimization performance.

## Usage
To run the notebook, ensure you have the necessary Python libraries installed.

## License

This project is licensed under the MIT License.
