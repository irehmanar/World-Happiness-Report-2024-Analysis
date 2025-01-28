# World Happiness Report 2024 Analysis

This project focuses on analyzing the "Happiness Report 2024" dataset using clustering and regression techniques to uncover patterns and predict happiness scores based on socio-economic factors.

## Dataset

The dataset, **"Happiness Report 2024"**, is sourced from Kaggle and can be found [here](https://www.kaggle.com/datasets/ajaypalsinghlo/world-happiness-report-2024). It contains data on socio-economic indicators such as GDP, social support, health, freedom, generosity, and corruption, as well as the happiness scores (Ladder score) for various countries.

## Objectives

1. **Clustering Analysis**:
   - Use K-Means clustering with the Elbow Method to determine the optimal number of clusters (k = 4).
   - Apply Principal Component Analysis (PCA) for dimensionality reduction and visualization of clusters.
   - Compare results with the DBSCAN algorithm for arbitrary-shaped clusters.
   - Interpret clusters by analyzing mean values of socio-economic indicators within each cluster.

2. **Regression Modeling**:
   - Predict happiness scores (Ladder score) using socio-economic factors and cluster labels as predictors.
   - Train and evaluate a Random Forest Regressor on the dataset.
   - Assess model performance using:
     - **R² Score**: 0.9022
     - **Mean Absolute Error (MAE)**: 0.2631

## Methodology

1. **Preprocessing**:
   - Handle missing values to create a clean dataset.
   - Explore relationships between features using pair plots and correlation matrices.

2. **Clustering**:
   - Perform K-Means clustering and determine the optimal number of clusters using the Elbow Method.
   - Apply PCA for dimensionality reduction and visualize clusters in a 2D space.
   - Utilize DBSCAN for detecting arbitrary-shaped clusters and compare results with K-Means.

3. **Regression**:
   - Select happiness score (Ladder score) as the target variable.
   - Use socio-economic features and K-Means cluster labels as predictors.
   - Train a Random Forest Regressor to predict happiness scores.
   - Evaluate the model's performance using R² and MAE metrics.

## Results

- **Clustering**:
  - K-Means identified four distinct clusters, effectively grouping countries based on socio-economic indicators.
  - PCA provided a clear visual representation of the clusters, while DBSCAN revealed additional insights into the structure of the data.

- **Regression**:
  - The Random Forest Regressor demonstrated excellent performance with:
    - **R² Score**: 0.9022
    - **Mean Absolute Error (MAE)**: 0.2631
  - These results highlight the strong relationship between socio-economic factors and happiness scores.

## Key Insights

- Socio-economic factors such as GDP, social support, and health have a significant impact on happiness scores.
- Clustering techniques provide valuable insights into the grouping of countries based on similarities in socio-economic indicators.
- The Random Forest Regressor is highly effective in predicting happiness scores, showcasing the importance of feature selection and robust modeling.

## How to Run the Code

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/happiness-report-2024-analysis.git
   cd happiness-report-2024-analysis
