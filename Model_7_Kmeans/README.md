# K-Means Clustering Algorithm

![K-Means Clustering](https://miro.medium.com/v2/resize:fit:1080/0*KfNpMUTtyCNQwYnp.png)

## Overview

K-Means is an unsupervised machine learning algorithm that is used to partition a dataset into **K distinct clusters**. The algorithm classifies data points into clusters in such a way that each data point belongs to the cluster with the nearest mean, serving as a prototype for the cluster.

## How K-Means Works

1. **Initialization**: The algorithm begins by selecting **K initial centroids** randomly or using some heuristic.
2. **Assignment Step**: Each data point is assigned to the nearest centroid, based on a distance metric (commonly Euclidean distance). This creates K clusters.
3. **Update Step**: For each cluster, the centroid is recalculated by averaging the data points assigned to the cluster.
4. **Repeat**: Steps 2 and 3 are repeated until the centroids no longer change significantly, or a predefined number of iterations is reached.

### Objective Function

The goal of K-Means is to minimize the sum of squared distances (variance) between each data point and the centroid of its cluster. This is defined by the following formula:

\[
\text{Objective} = \sum_{i=1}^{K} \sum_{x \in C_i} ||x - \mu_i||^2
\]

Where:
- \( K \) is the number of clusters.
- \( C_i \) is the set of data points assigned to cluster \( i \).
- \( \mu_i \) is the centroid of cluster \( i \).
- \( ||x - \mu_i||^2 \) is the squared Euclidean distance between point \( x \) and the centroid \( \mu_i \).

## Applications

K-Means is commonly used in:
- Image compression
- Customer segmentation
- Anomaly detection
- Document clustering

## Pros and Cons

### Pros:
- Simple and easy to understand.
- Fast and efficient for large datasets.
- Scales well to high-dimensional data.

### Cons:
- Requires the number of clusters \( K \) to be specified in advance.
- Sensitive to initial centroids and outliers.
- May converge to local minima.

## Example

```python
from sklearn.cluster import KMeans
import numpy as np

# Create sample data
X = np.array([[1, 2], [1, 4], [1, 0],
              [10, 2], [10, 4], [10, 0]])

# Create KMeans instance
kmeans = KMeans(n_clusters=2, random_state=0).fit(X)

# Predict the cluster for each point
print(kmeans.labels_)

