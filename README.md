# CryptoClustering

## Project Summary

This project involves the analysis of a cryptocurrency dataset using unsupervised learning techniques, specifically Principal Component Analysis (PCA). The analysis compares the clustering results with and without optimization techniques to understand the impact on cluster formation.

## Repository Structure

The repository contains the following files and directories:

- `Resources/`: A folder containing the CSV file with the cryptocurrency data.
  - `crypto_market_data.csv`: The dataset used for the analysis.
- `crypto_analysis.ipynb`: A Jupyter Notebook file where the analysis and clustering were conducted.
- `README.md`: This file, providing an overview of the project and its dependencies.

## Dependencies

The following dependencies are required to run the analysis:

- pandas
- hvplot pandas
- KMeans
- PCA
- StandardScaler
- filterwarnings

## Analysis Summary

The analysis was conducted using both the original dataset and a reduced dataset obtained via PCA. The steps included:

1. **Data Preparation**: Loaded and preprocessed the data, including normalization using `StandardScaler`.
2. **Elbow Method**: Applied the Elbow method to determine the optimal number of clusters (k) for both the original and PCA-transformed data.
3. **Clustering**: Performed K-Means clustering on both datasets using the identified optimal k.
4. **Visualization**: Created scatter plots to visualize the clusters and composite plots to compare the elbow curves from both datasets.

### Key Observations

- **Elbow Plot Analysis**: Both the original and PCA-transformed datasets resulted in the same optimal k. However, the inertia was lower for the PCA-transformed data, indicating more compact clusters.
- **Scatter Plot Analysis**: The scatter plots for the PCA-transformed data showed less scatter, suggesting more distinct and cohesive clusters compared to the original data.
