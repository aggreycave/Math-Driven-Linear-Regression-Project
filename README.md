# Math-Driven Linear Regression from Scratch

A professional portfolio project that implements **Linear Regression from first principles** using NumPy, with a focus on the mathematics behind machine learning: linear algebra, calculus, statistics, gradient descent, and model evaluation.

This project is designed for entry-level **AI Engineer / Machine Learning Engineer** applications. It demonstrates the ability to connect mathematical theory with production-style Python code, clean documentation, testing, and visual explanation.

## Project Highlights

- Implements linear regression without using scikit-learn's model API
- Builds prediction, cost, gradient descent, and evaluation functions from scratch
- Explains the mathematical foundation behind the model
- Compares gradient descent results with the closed-form normal equation
- Visualizes the dataset, fitted regression line, residuals, and training loss
- Includes a reusable Python module and unit tests
- Structured as a GitHub-ready machine learning portfolio project

## Mathematical Concepts Covered

### Linear Algebra
The linear regression model is represented as:

$$\hat{y} = X\theta$$

where:

- $X$ is the feature matrix with a bias column
- $\theta$ is the parameter vector containing the intercept and feature weights
- $\hat{y}$ is the predicted target vector

### Calculus and Optimization
The model minimizes the mean squared error cost function:

$$J(\theta) = \frac{1}{2m}\sum_{i=1}^{m}(\hat{y}^{(i)} - y^{(i)})^2$$

Gradient descent updates the parameters using:

$$\theta := \theta - \alpha \nabla J(\theta)$$

where:

$$\nabla J(\theta) = \frac{1}{m}X^T(X\theta - y)$$

### Statistics
Model performance is evaluated using:

- Mean Squared Error, which measures average squared prediction error
- Root Mean Squared Error, which gives error in the same unit as the target
- R-squared, which measures explained variance
