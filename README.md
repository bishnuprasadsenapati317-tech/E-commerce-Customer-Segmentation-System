# E-commerce-Customer-Segmentation-System
SmartCart Clustering System uses unsupervised machine learning to segment e-commerce customers by spending, demographics, and engagement, helping businesses personalize marketing and improve retention.

## Project Objective

SmartCart currently uses the same marketing strategy for all customers, which can lead to inefficient campaigns and missed business opportunities. This project solves that problem by grouping customers into meaningful clusters based on their behavior and engagement.

The main goal is to support data-driven decision-making for:

- Customer segmentation
- Personalized marketing
- High-value customer identification
- Churn-risk analysis
- Better campaign targeting
- Customer retention improvement

## Dataset Overview

The dataset contains customer information from an e-commerce platform.

It includes:

- Customer demographics such as age, education, marital status, income, and household details
- Purchase behavior across product categories such as wines, fruits, meat, fish, sweets, and gold products
- Purchase frequency through web, catalog, store, and discount-based channels
- Website activity such as monthly web visits
- Customer recency, complaints, and campaign response

Dataset size:

- 2,240 customer records
- 22 original features

## Work Done

The notebook performs the following steps:

1. Data loading and exploration
2. Missing value handling using median income
3. Feature engineering
   - Age
   - Customer tenure
   - Total spending
   - Total children
   - Living status
4. Category simplification for education and marital status
5. Outlier removal for income and age
6. Correlation analysis using heatmap
7. One-hot encoding of categorical variables
8. Feature scaling using StandardScaler
9. Dimensionality reduction using PCA
10. Optimal cluster selection using Elbow Method and Silhouette Score
11. Customer clustering using:
    - KMeans Clustering
    - Agglomerative Clustering
12. Cluster visualization using 3D PCA plots
13. Cluster characterization using spending, income, family size, and engagement behavior

## Machine Learning Techniques Used

- Data preprocessing
- Feature engineering
- One-hot encoding
- Standard scaling
- Principal Component Analysis
- Elbow Method
- Silhouette Score
- KMeans Clustering
- Agglomerative Clustering
- Cluster profiling and visualization

## Technologies Used

- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Kneed
- Jupyter Notebook

## Files

- `smartcart.ipynb` - Main notebook containing data preprocessing, analysis, clustering, visualization, and cluster profiling

## Results

The analysis found that the optimal number of customer clusters is 4.

The final clusters show different customer patterns based on income, total spending, purchase channels, number of children, response rate, and living status.

One cluster shows customers with more web visits , with partner , more children and minimal web , store purchases .They can categorized into "Family Shoppers". They can be offered Discounts and Coupons.

Another cluster shows customers mostly Alone , higher age , less web visits but High web purchases and High Store purchaces . They can be categorized into "High Value Singles". They can be offered Premium Services.

Another cluster shows customers with low age , more children, High web visits but very less purchases.
They can be categorized into "Digital Browsers". They can be offered Sales , heavy discounts and cupons.

The Remaining Cluster shows customers with fewer children, higher age, with partners , less web visits but high web purchases and store purchases. They shows average response . We can offer them Loyality Programs .

These insights can be used by SmartCart to create targeted marketing campaigns and improve customer engagement.
