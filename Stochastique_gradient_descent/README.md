# Stochastic Gradient Descent (SGD)

## Description

Stochastic Gradient Descent (SGD) is a popular optimization algorithm used to minimize the loss function in machine learning models. Unlike traditional Gradient Descent, which computes the gradient using the entire dataset, SGD updates the model's parameters for each training example. This makes it faster and more efficient, especially for large datasets.

## How It Works

1. **Initialize parameters** randomly.
2. **Iterate over the dataset**: For each data point, compute the gradient of the loss function.
3. **Update parameters**: Adjust the parameters by moving them in the direction of the negative gradient.
4. **Repeat**: Continue updating until convergence or a stopping criterion is met.

### Formula

The general update rule for SGD is:

\[
\theta = \theta - \eta \cdot \nabla_{\theta} J(\theta; x^{(i)}, y^{(i)})
\]

Where:
- \( \theta \) represents the model parameters.
- \( \eta \) is the learning rate (a small positive value).
- \( \nabla_{\theta} J \) is the gradient of the loss function \( J \) with respect to the model parameters for the \( i \)-th data point \( (x^{(i)}, y^{(i)}) \).

## Advantages

- **Efficiency**: Faster updates per iteration, ideal for large datasets.
- **Better generalization**: Randomness in updates introduces noise that can help escape local minima.
- **Memory-efficient**: Requires only a single training example to compute the gradient at each iteration.

## Illustration

Below is an illustration of the **SGD process**, where the model parameters are updated iteratively using random samples from the dataset:

![SGD Process](https://media.geeksforgeeks.org/wp-content/uploads/sgd-1.jpg)

1. **Random Initialization**: Start with initial parameters.
2. **Update**: For each random sample, calculate the gradient and update the parameters.
3. **Convergence**: Parameters converge towards the optimal value with some fluctuations due to randomness.

## When to Use

SGD is especially useful for training models with:
- Large-scale data (millions of samples).
- Models where faster iterations are needed.
- Situations where memory efficiency is critical.
