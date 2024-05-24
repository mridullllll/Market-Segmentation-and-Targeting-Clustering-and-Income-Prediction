# Market-Segmentation-and-Targeting-Clustering-and-Income-Prediction

## Project Overview

This project involves segmenting a market using clustering techniques with the aim to assist Whole Foods Market Inc. in identifying potential locations for expansion in Canada. The analysis is based on Census data from Statistics Canada, focusing on demographic and socioeconomic variables.

## Steps Involved

### 1. Pre-processing

Data preparation is a crucial step in ensuring the quality and reliability of the analysis. The pre-processing steps include:

- **Loading Data**: The dataset is sourced from Census Canada 2021, split into training and test sets.
- **Data Cleaning**: Removal of null values, duplicate columns, and unnecessary data points.
- **Feature Engineering**: Aggregating columns such as construction periods and types of households to create meaningful features.
- **Feature Selection**: Using Random Forest to identify important features for clustering.

### 2. Modelling

In the modelling phase, the project employs clustering algorithms to segment the market:

- **Standardization**: Features are standardized using Min-Max Normalization to ensure uniformity in data scale.
- **Clustering Algorithm**: K-Means clustering is used, with the optimal number of clusters determined using the Silhouette Score. Additionally, the BIRCH clustering model is compared.
- **Model Training**: K-Means is trained on the pre-processed data, and various regression models (Ridge, KNN, Decision Tree, ANN) are applied within each cluster to predict median income.

### 3. Results

The results are evaluated to determine the effectiveness of the clustering:

- **Cluster Evaluation**: Performance of each clustering configuration is evaluated using the Silhouette Score. The optimal number of clusters is found to be 3.
- **Visualization**: Scatter plots and heat maps are used to visualize the clusters and the correlation between features.
- **Model Performance**: The regression models are evaluated using Mean Squared Error (MSE) and Mean Absolute Error (MAE), with Ridge Regression performing best in most clusters.

### 4. Analysis & Insights

Key findings from the analysis include:

- **Cluster Characteristics**: Detailed examination of clusters reveals differences in income levels, household types, and construction periods.
- **Market Segmentation**: Clusters are categorized into high-income, middle-income, and low-income groups, providing insights for targeted marketing strategies.

### 5. Challenges & Considerations

Several challenges and considerations are noted:

- **Data Limitations**: The absence of geographic information limits the analysis, as location is a crucial factor for store placement.
- **Cluster Size**: Some clusters contain a large number of observations, suggesting the need for further segmentation.
- **Model Selection**: The choice of clustering and regression models significantly impacts the results, highlighting the importance of model evaluation.

## Conclusion

This project demonstrates the application of clustering techniques in market segmentation for strategic decision-making. The insights gained from the analysis can help Whole Foods Market Inc. identify optimal locations for expansion in Canada. However, further data collection, particularly geographic information, and recursive clustering are recommended for more refined targeting.
