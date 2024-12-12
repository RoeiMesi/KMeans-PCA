# K-Means and PCA

This project focuses on implementing the K-Means clustering algorithm and Principal Component Analysis (PCA) from scratch using NumPy. It provides hands-on experience with unsupervised learning techniques and dimensionality reduction.

## Overview

### Part 1: K-Means
1. **Objective**:
   - Implement and understand the K-Means clustering algorithm.
   - Visualize clustering results and analyze the cost function.

2. **Steps**:
   - Generate a 2D dataset with predefined clusters.
   - Implement K-Means clustering with custom initialization, iterative centroid updates, and cost calculation.
   - Analyze the convergence by plotting costs across iterations.
   - Test the algorithm with different numbers of clusters and plot the results for each iteration.

### Part 2: PCA
1. **Objective**:
   - Implement the PCA algorithm for dimensionality reduction.
   - Apply PCA to the MNIST dataset and visualize data in the reduced space.

2. **Steps**:
   - Implement PCA by calculating eigenvalues and eigenvectors of the covariance matrix.
   - Reduce the data to 2 dimensions and visualize in principal component space.
   - Compare projection matrices and understand their properties.
   - Reconstruct images from reduced dimensions and analyze reconstruction fidelity.

## Environment

- **Programming Language**: Python 3.x
- **Libraries**:
  - NumPy
  - Matplotlib
  - sklearn.datasets (for MNIST)
- **System Requirements**: Any standard Python environment.

## Instructions

### Part 1: K-Means

1. **Data Generation**:
   - Generate a synthetic 2D dataset with four clusters.
   - Shuffle the data to ensure randomness.

2. **Algorithm Implementation**:
   - Implement the `KMeans` class with methods for centroid initialization, label assignment, and centroid updates.
   - Include cost calculation to monitor convergence.

3. **Visualization**:
   - Plot data points and centroids at each iteration.
   - Visualize costs as a function of iterations to ensure the algorithm converges.

4. **Experiments**:
   - Run the algorithm with different numbers of clusters (2, 3, 4, 6, 8, 10, 20) and record final costs.

5. **Results**:
   - Plot clusters and centroid locations for each iteration.
   - Compare clustering results visually.

### Part 2: PCA

1. **Data Preparation**:
   - Load the MNIST dataset and preprocess it by centering the data.

2. **Algorithm Implementation**:
   - Implement the `PCA` class to calculate eigenvalues and eigenvectors of the covariance matrix.
   - Project the data onto the top principal components.

3. **Visualization**:
   - Reduce data to 2 dimensions and plot using scatter plots.
   - Compare matrices \( V^T V \) and \( V V^T \) and explain their properties.

4. **Reconstruction**:
   - Implement a function to reconstruct data from reduced dimensions.
   - Test reconstruction with varying dimensions (3, 10, 100) and visualize results.
   - Evaluate whether reconstructed images match the original images.

## Results

### K-Means
- **Final Costs for Different Cluster Numbers**:
  - 2 clusters: 16252.94
  - 3 clusters: 9610.87
  - 4 clusters: 3843.71
  - 6 clusters: 3274.15
  - 8 clusters: 2605.75
  - 10 clusters: 2211.16
  - 20 clusters: 1101.99

- **Visualization**:
  - Costs vs. Iterations: Convergence graph demonstrates decreasing cost.
  - Clusters and Centroids: Visual inspection shows meaningful separation.

### PCA
- **Data Visualization**:
  - MNIST data projected onto the top 2 principal components.
  - Clusters are visually distinct based on digit labels.

- **Matrix Comparison**:
  - \( V^T V \): Identity matrix due to orthonormal eigenvectors.
  - \( V V^T \): Projection matrix representing reduced subspace.

- **Reconstruction**:
  - Images reconstructed from 3, 10, and 100 principal components.
  - Higher dimensions result in more accurate reconstructions, but none are identical to the original image.

## Notes

- Ensure randomness by seeding the random number generator where necessary.
- Test the implementation thoroughly for edge cases.
- Interpret and explain results in the context of unsupervised learning and dimensionality reduction.
