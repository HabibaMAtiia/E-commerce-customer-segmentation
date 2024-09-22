# E-commerce-customer-segmentation
## Project Overview
- This project aims to segment customers using unsupervised machine learning techniques based on their transactional behavior. The goal is to identify distinct customer groups that can be targeted with personalized coupons to enhance loyalty and satisfaction. In addition to the customer segmentation, a dashboard was designed to present key insights from the dataset for business managers and marketing teams. This dashboard helps stakeholders make informed, data-driven decisions by visualizing customer behaviors and trends.
## Objectives
 - Build a user-friendly and informative dashboard for Stakeholders and marketing teams.
 - Help stakeholders understand the customer base and adapt marketing campaigns accordingly.
 - Analyze loyalty patterns and help identify high-value customers for retention strategies.
 - Develop and train a machine learning model that segments customers based on their transactional behaviors and demographics.
 - Analyze each customer segment and provide insights into their behavior patterns.
 - Recommend personalized coupon strategies to target specific segments to boost engagement and loyalty.
## Dataset
- The dataset includes several tables, such as:
  - Customers Table: Contains customer demographic information (gender, city).
  - Transactions Table: Records coupon usage history (claimed, burnt).
  - Branches, Merchants, Cities Tables: Additional information about coupon burn locations.
## Installation
## Feature Engineering
  - Aggregation:
    - Recency: Time since the last transaction.
    - Transaction Frequency: How often customers claim or burn coupons.
    - Burn Rate: Ratio of burnt coupons to claimed ones.
    - Merchant Frequency: Number of interactions with different merchants.
    - City Frequency: Frequency of transactions across different cities.
 - Encoding categorical features:
    - Gender: One-hot encoded as gender_name_Female, gender_name_Male.
 - Scaling numerical features
    - Using Standard Scalar.
## Dimensionality Reduction
 - PCA
 - TSNE
## Model Development
  1. K-means
  2. DBSCAN
  3. Gaussian Mixture
  4. Hierarchical Clustering
## Evaluation Metrics
  - The model was evaluated using the following metrics:
    - Inertia (for K-Means): Measures how well the clusters are formed based on the distance between data points and their assigned cluster centroids.
    - Elbow Method: Used to decide the appropriate number of clusters.
    - Silhouette Score: Assesses how well customers are clustered, considers both the cohesion within clusters and separation between clusters.
## Results
 - K-Means with 2D PCA and 5 clusters was selected as the final model based on its performance in identifying meaningful customer groups.
