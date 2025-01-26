# CryptoClustering
Module 19 Challenge - Machine Learning

## Project Overview

The analysis includes the following steps:
1. **Data Preprocessing**: Standardizing the cryptocurrency market data using `StandardScaler`.
2. **Elbow Method**: Identifying the optimal number of clusters (k) for K-Means using the inertia values.
3. **K-Means Clustering**: Clustering the cryptocurrencies based on their price change percentages.
4. **Principal Component Analysis (PCA)**: Reducing the dimensionality of the data to optimize clustering.
5. **Visualization**: Comparing clustering results with and without PCA through scatter plots and Elbow curves.

## Prerequisites
Ensure the following Python libraries are installed:
- `pandas`
- `hvplot`
- `scikit-learn`


## Key Steps in the Analysis

### 1. Data Preprocessing
- The dataset is normalized using `StandardScaler` to standardize the range of features.
- Key features include price changes over different timeframes (24h, 7d, 14d, etc.).

### 2. Elbow Method
- An Elbow curve is plotted to determine the optimal number of clusters (k).
- The inertia values for k = 1 to 10 are calculated and plotted.

### 3. K-Means Clustering
- Cryptocurrencies are clustered using K-Means with the optimal k value identified from the Elbow curve.
- Clustering is performed both on the original scaled data and the PCA-transformed data.

### 4. Principal Component Analysis (PCA)
- Dimensionality reduction is applied to reduce the data to 3 principal components.
- The reduced data retains significant variance while simplifying the clustering process.

### 5. Visualization
- Scatter plots show clusters formed based on:
  - Original scaled data (price change percentages).
  - PCA-transformed data (principal components).
- Composite Elbow curves compare the inertia values for both datasets.

## Results
- The optimal number of clusters (`k`) is consistently identified as 3 for both datasets.
- PCA simplifies the data and enhances computational efficiency without losing significant information.

### Author
[Sait0uAsuka](https://github.com/Sait0uAsuka)



## License
This project is licensed under the MIT License. See the LICENSE file for details.