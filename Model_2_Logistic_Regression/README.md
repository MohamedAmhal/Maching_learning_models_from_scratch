# Logistic Regression Model

![Logistic Regression](https://www.ejable.com/wp-content/uploads/2023/11/linear-regression-vs-logistic-regression-2.webp)

## Introduction

Logistic regression is a statistical method used for binary classification tasks. It predicts the probability that a given input belongs to one of two possible classes. Unlike linear regression, logistic regression applies a **sigmoid function** to ensure that the output falls between 0 and 1, making it suitable for classification.

The formula for logistic regression is given as:

\[
h_\theta(x) = \frac{1}{1 + e^{-\theta^T x}}
\]

Where:
- \( h_\theta(x) \) is the hypothesis or predicted probability.
- \( \theta \) represents the model parameters.
- \( x \) is the input feature vector.
- \( e \) is the base of the natural logarithm.

## Loss Function

For logistic regression, we use a **log loss** or **binary cross-entropy loss** function to measure how well the model’s predictions match the actual labels.

The cost function for logistic regression is:

\[
J(\theta) = - \frac{1}{m} \sum_{i=1}^{m} \left[ y^{(i)} \log(h_\theta(x^{(i)})) + (1 - y^{(i)}) \log(1 - h_\theta(x^{(i)})) \right]
\]

Where:
- \( J(\theta) \) is the cost function.
- \( y^{(i)} \) is the actual label for the \(i^{th}\) training example.
- \( h_\theta(x^{(i)}) \) is the predicted probability for the \(i^{th}\) training example.
- \( m \) is the number of training examples.

## Gradient Descent Optimization

To minimize the cost function and find the optimal parameters \( \theta \), we use **gradient descent**. Gradient descent adjusts the parameters iteratively in the direction of the steepest decrease in the cost function.

The gradient descent update rule for logistic regression is:

\[
\theta := \theta - \alpha \frac{1}{m} \sum_{i=1}^{m} \left( h_\theta(x^{(i)}) - y^{(i)} \right) x^{(i)}
\]

Where:
- \( \alpha \) is the learning rate.
- \( h_\theta(x^{(i)}) \) is the predicted probability for the \(i^{th}\) training example.
- \( y^{(i)} \) is the actual label for the \(i^{th}\) training example.

## Conclusion

Logistic regression is a powerful and interpretable machine learning model for binary classification tasks. By optimizing the loss function using gradient descent, we can find the best parameters to maximize the accuracy of the model.

