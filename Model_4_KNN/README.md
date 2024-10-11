# KNN - K-Nearest Neighbors Algorithm

![K-Nearest Neighbors Visualization](https://datascientest.com/en/files/2023/09/Illu-2-KNN.jpg)

> *An illustration of KNN algorithm classifying a new data point based on its k nearest neighbors*

## Overview

This folder contains an implementation of the K-Nearest Neighbors (KNN) algorithm. KNN is a simple, non-parametric, and lazy learning algorithm used for classification and regression. It works by finding the `k` closest data points (neighbors) to a given input and making predictions based on their labels.

## Folder Structure

- `knn_model.py`: Python script that implements the KNN algorithm from scratch.
- `datasets/`: A folder containing datasets for training and testing the KNN model.
- `README.md`: Documentation for understanding and using the KNN implementation.
  
## Features

- Implements K-Nearest Neighbors for classification.
- Supports Euclidean and Manhattan distance metrics.
- Configurable number of neighbors (`k`).
- Handles multi-class classification problems.
- Evaluation metrics like accuracy, confusion matrix, and classification report.

## Getting Started

### Prerequisites

Ensure the following Python libraries are installed:

```bash
pip install numpy pandas scikit-learn matplotlib

