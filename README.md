# Cryptocurrency Clustering Analysis

## Notebooks

### 1. Main Analysis Notebook

- **File Name**: `Main.ipynb`
- **URL**: [Main.ipynb](https://github.com/jancichocki/Module_10_Challenge/blob/main/Main.ipynb)

**Description**: This notebook encompasses the complete set of analyses and tasks outlined for the Module 10 Challenge. It adheres to the specified calendar requirements, integrating comprehensive data exploration, preprocessing, and modeling techniques aimed at understanding cryptocurrency market dynamics.

### 2. Question and Answer Format Notebook

- **File Name**: `crypto_investments.ipynb`
- **URL**: [crypto_investments.ipynb](https://github.com/jancichocki/Module_10_Challenge/blob/main/crypto_investments.ipynb)

**Description**: This notebook adopts a question-and-answer format, aligning with the Juniper Lab's interactive approach to presenting cryptocurrency investment insights. It facilitates a detailed inquiry into specific facets of the cryptocurrency market, enabling a structured and engaging exploration.

## Overview
This project aims to cluster cryptocurrencies based on their market performance using both original and PCA-transformed data. The goal is to find the optimal number of clusters (k) and visualize the clustering to understand the underlying patterns in cryptocurrency market behavior.

## Steps Overview
1. **Import and Prepare Data**
2. **Determine the Best Value for k Using Original Data**
3. **Cluster Cryptocurrencies Using Original Data**
4. **Optimize Clusters with PCA**
5. **Determine the Best Value for k Using PCA Data**
6. **Cluster Cryptocurrencies Using PCA Data**
7. **Visualize and Compare Results**

## Detailed Steps

### 1. Import and Prepare Data
- Load cryptocurrency market data.
- Normalize the data using `StandardScaler`.

### 2. Find the Best Value for k Using Original Data
- Apply the elbow method by plotting inertia for k values 1 to 11.
- Determine the optimal k value where the inertia begins to plateau.

### 3. Cluster Cryptocurrencies Using Original Data
- Use `KMeans` clustering with the optimal k value determined previously.
- Assign cluster labels to each cryptocurrency.

### 4. Optimize Clusters with PCA
- Perform Principal Component Analysis (PCA) to reduce data dimensionality.
- Retain three principal components for clustering analysis.

### 5. Find the Best Value for k Using PCA Data
- Apply the elbow method to the PCA-transformed data.
- Confirm the consistency of the optimal k value with the original data.

### 6. Cluster Cryptocurrencies Using PCA Data
- Repeat the clustering process using the PCA-transformed data.
- Visualize the clusters formed in the space of the first two principal components.

### 7. Visualize and Compare Results
- Create composite plots to compare elbow curves and clustering results of the original and PCA-transformed data.
- Analyze the impact of using PCA for dimensionality reduction on clustering results.

## Conclusion
The analysis shows that both the original and PCA-transformed data suggest an optimal k value of 4. Clustering with K-Means before and after PCA reveals consistent structures, indicating that PCA is effective in dimensionality reduction without significant loss of clustering integrity. This approach simplifies the dataset and facilitates a more efficient clustering process, making it easier to visualize and interpret the results.
