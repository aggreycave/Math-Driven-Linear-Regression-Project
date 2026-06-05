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

## Repository Structure

```text
math-driven-linear-regression/
├── README.md
├── requirements.txt
├── .gitignore
├── notebooks/
│   ├── Math_Driven_Linear_Regression_Portfolio.ipynb
│   └── original_Math_Driven_Project.ipynb
├── src/
│   ├── __init__.py
│   └── linear_regression_from_scratch.py
├── tests/
│   └── test_linear_regression.py
└── docs/
    └── AI_Engineer_Portfolio_Summary.md
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/math-driven-linear-regression.git
cd math-driven-linear-regression
```

### 2. Create a virtual environment

```bash
python -m venv .venv
source .venv/bin/activate   # macOS/Linux
# .venv\Scripts\activate    # Windows
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the notebook

```bash
jupyter notebook notebooks/Math_Driven_Linear_Regression_Portfolio.ipynb
```

### 5. Run tests

```bash
pytest
```

## Example Results

Using synthetic data generated from approximately:

$$y = 4 + 3x + \epsilon$$

The model learns parameters close to:

- Intercept: approximately 4
- Slope: approximately 3

The final notebook shows the learned line, residual behavior, and loss convergence.

## AI Engineering Relevance

This project demonstrates skills that are important for AI Engineering roles:

- Mathematical understanding of machine learning algorithms
- Python and NumPy programming
- Model training and evaluation
- Reusable code design
- Testing and documentation
- Ability to explain AI systems clearly to technical and non-technical audiences

## Suggested CV Bullet

**Math-Driven Linear Regression from Scratch** — Built a NumPy-based linear regression model from first principles, implementing prediction, gradient descent optimization, loss tracking, MSE/RMSE/R² evaluation, residual analysis, and normal equation comparison; packaged the project with tests and GitHub-ready documentation to demonstrate mathematical ML foundations and clean Python engineering practice.

## Next Improvements

- Add support for multiple features
- Add feature scaling
- Add polynomial regression
- Compare results against scikit-learn
- Deploy as a small Streamlit demo
- Add CI testing with GitHub Actions
