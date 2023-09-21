# CryptoClustering
# Cryptocurrency Clustering with K-Means and PCA

## Overview

This project involves the clustering of cryptocurrencies using the K-Means clustering algorithm and Principal Component Analysis (PCA). The primary goal is to group cryptocurrencies into clusters based on their market data and visualize the results.

## Project Structure

The project is structured into several key steps:

### 1. Data Preparation

- Load cryptocurrency market data from a CSV file.
- Display sample data and generate summary statistics.
- Plot the data to visualize its structure.

### 2. Data Preprocessing

- Use the `StandardScaler()` module from scikit-learn to normalize the data.
- Create a DataFrame with the scaled data.
- Copy the cryptocurrency names from the original data.
- Set the coinid column as the index.

### 3. Finding the Optimal Value for k

- Create a list of k-values from 1 to 11.
- Create an empty list to store the inertia values.
- Compute the inertia for each value of k using K-Means.
- Create a dictionary and DataFrame for plotting the Elbow curve.
- Plot the Elbow curve to determine the optimal value for k.

### 4. Clustering with K-Means Using Original Data

- Initialize the K-Means model using the best value for k.
- Fit the K-Means model using the scaled data.
- Predict the clusters and add a new column for cluster labels.

### 5. Principal Component Analysis (PCA)

- Create a PCA model instance and set `n_components=3`.
- Use PCA to reduce the data to three principal components.
- Retrieve the explained variance to assess the information captured.

### 6. Finding the Optimal Value for k (PCA Data)

- Create a list of k-values from 1 to 11.
- Create an empty list to store the inertia values.
- Compute the inertia for each value of k using K-Means with PCA data.
- Create a dictionary and DataFrame for plotting the Elbow curve.
- Plot the Elbow curve to determine the optimal value for k.

### 7. Clustering with K-Means Using PCA Data

- Initialize the K-Means model using the best value for k.
- Fit the K-Means model using the PCA-transformed data.
- Predict the clusters and add a new column for cluster labels.

### 8. Visualize and Compare Results

- Create visualizations to contrast the clustering results with and without PCA.
- Analyze the impact of dimensionality reduction on clustering.

## Conclusion

- The project demonstrates how to cluster cryptocurrencies using K-Means and PCA.
- The optimal value for k is determined through the Elbow curve method.
- Clustering results are visualized and compared, highlighting the impact of PCA on clustering.
- This project provides insights into grouping cryptocurrencies based on market data and can be extended for further analysis or investment strategies.

For detailed code and implementation, refer to the project files and code documentation.
