# K-Means Clustering for Gene Expression Data

This project applies K-Means clustering on gene expression data using both a custom implementation of the K-Means algorithm and the Scipy library's implementation. The goal is to explore and compare clustering results on complex gene expression datasets and gain insights into patterns and groupings within the data.

## Project Overview
This project leverages K-Means clustering to group gene expression data based on similarities. The clustering is performed using both a custom-built K-Means algorithm and the K-Means implementation available in the Scipy library, providing an opportunity to understand the nuances of each approach and their comparative performance.

## Dataset Structure
- Rows: Each row represents a sample, such as a tissue or experimental condition.
- Columns: Each column corresponds to a specific gene's expression level across samples.
- Shape: The dataset comprises 801 rows (samples) and 20,532 columns (genes).
The dataset contains numerical values representing the gene expression levels for each sample.

## Clustering Implementations
## Custom K-Means
The custom implementation of K-Means is built from scratch without relying on external clustering libraries. Key features and steps include:
- Initialization: Random selection of initial cluster centroids.
- Distance Calculation: The algorithm computes the Euclidean distance between data points and centroids.
- Cluster Assignment: Each data point is assigned to the nearest cluster based on calculated distances.
- Centroid Update: The centroids are updated by calculating the mean of data points assigned to each cluster.
- Convergence Criteria: The process iterates until convergence, defined by a threshold or a maximum number of iterations.
This implementation offers flexibility and transparency, providing an educational opportunity to understand the inner workings of K-Means clustering.

## Scipy K-Means
The project also utilizes the K-Means clustering function available in the Scipy library. This implementation offers a faster and optimized version of the algorithm, leveraging built-in capabilities for efficient computation. Key features include:
- Scipy's scipy.cluster.vq.kmeans function: This function provides a straightforward way to apply K-Means clustering with minimal configuration.
- Optimized Initialization and Iteration: The Scipy implementation handles initialization and convergence efficiently, providing high-performance clustering with built-in optimization techniques.
Comparing the results of the custom implementation and Scipy's version allows for a deeper understanding of K-Means clustering and potential differences in output, performance, and convergence behavior.

## Usage Requirements
To run this project, you will need:
Python 3.x,
Jupyter Notebook,
NumPy,
Pandas,
Scipy,
Matplotlib (for visualization)

## Results
The project compares the clustering results from both approaches:
- Custom K-Means: Provides insights into the step-by-step convergence and allows fine-grained control over the algorithm parameters.
- Scipy K-Means: Offers faster execution with optimized performance and reliable clustering results.
The comparison highlights differences in computation time, accuracy, and potential variations in cluster assignments due to different initialization strategies.
