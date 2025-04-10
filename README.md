## CryptoClustering
The purpose of the project is to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.


## Data used: 
crypto_market_data.csv


## Key Steps:
# Data Preprocessing
Loaded historical crypto market data and standardized the features using StandardScaler to ensure comparability.

# Initial Clustering with K-Means
Applied the K-Means algorithm to the original scaled data. Used the Elbow Method to determine the optimal number of clusters (k = 4).

# Dimensionality Reduction with PCA
Reduced the number of features from 7 to 3 principal components using PCA, retaining ~89% of the total variance.

# Optimized Clustering
Re-applied K-Means to the PCA-transformed data and re-evaluated the best value of k, which remained at 4.

# Visualization and Comparison
Used hvPlot to visually compare clustering results before and after PCA, and to highlight how dimensionality reduction improved cluster separation.
