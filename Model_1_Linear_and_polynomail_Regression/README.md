# Linear Regression Models from Scratch

![Machine Learning](https://www.stanford.edu/class/stats202/figs/Chapter3/3.1.png)

This folder contains two Jupyter notebooks demonstrating the implementation of **Linear Regression** from scratch using Python. Each notebook covers different aspects of Linear Regression, from simple to multiple variables, providing a solid foundation for understanding how these models work internally without relying on machine learning libraries.

## Files in this Folder

### 1. `Get_started_linear_regression(one_variable)_from_scratch.ipynb`

This notebook introduces **Simple Linear Regression** (with one variable). It covers:

- **Introduction to Linear Regression**: Understanding the basic concepts.
- **Mathematical Derivation**: How the model calculates the line of best fit.
- **Gradient Descent**: Optimization technique to minimize the cost function.
- **Implementation from Scratch**: Building a working model using just Python.
- **Visualization**: Plotting the regression line and data points.

#### Key Concepts:
- Cost function (Mean Squared Error).
- Gradient Descent for one variable.
- Prediction using the linear regression model.

### 2. `Linear_regression(multi_variable)_from_scratch.ipynb`

This notebook extends **Linear Regression** to handle multiple variables (features), known as **Multivariable Linear Regression**. It explains:

- **Mathematical Formulation**: For linear regression with multiple inputs.
- **Gradient Descent**: Applying gradient descent for multiple variables.
- **Feature Scaling**: How to normalize the input data to speed up convergence.
- **From Scratch Implementation**: Building a multivariable linear regression model in Python.
- **Example Dataset**: Working with a dataset that contains multiple features.

#### Key Concepts:
- Multiple features and how they impact the model.
- Vectorized implementation for faster computations.
- Performance evaluation using metrics like Mean Squared Error (MSE).

## How to Use These Files

1. Clone the repository and navigate to this folder.
   
   ```bash
   git clone https://github.com/MohamedAmhal/maching_learning_models_from_scratch.git
   cd ml-models-from-scratch/linear_regression

