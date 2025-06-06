# Task-8-Clustering
# Mall Customer Segmentation using K-Means Clustering

This project performs unsupervised machine learning using K-Means Clustering on a retail customer dataset to segment customers based on their spending behavior. It includes full exploratory data analysis (EDA), optimal cluster selection, dimensionality reduction, and model evaluation.


## Objectives

- Segment mall customers into distinct groups using K-Means.
- Discover patterns in customer demographics and spending scores.
- Visualize clusters in 2D using PCA for better understanding.
- Evaluate cluster quality using the Silhouette Score.

## Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Dataset

- Source: Kaggle - Customer Segmentation
- File: Mall_Customers.csv
- Features:
  - CustomerID (removed)
  - Gender
  - Age
  - Annual Income (k$)
  - Spending Score (1-100)

---

## Project Flow

1. Load Dataset  
2. Exploratory Data Analysis (EDA): statistics, correlations, visual analysis  
3. Data Preprocessing: encode gender, scale features  
4. Dimensionality Reduction: PCA for 2D visualization  
5. Cluster Number Selection: Elbow Method and Silhouette Score  
6. K-Means Clustering  
7. Cluster Visualization and Evaluation  
8. Extracting Business Insights

---

## Trends, Patterns and Insights

Based on the clustering output (K = 5), the following customer segments were identified:

### Cluster 0: High Income, High Spenders
- Young to middle-aged individuals with high annual income and spending score.
- Marketing strategy: Offer premium and luxury products or services.

### Cluster 1: Low Income, High Spenders
- Customers with relatively low income but high spending score.
- May respond to discounts or promotions.
- Strategy: Promote limited-time offers and membership deals.

### Cluster 2: High Income, Low Spenders
- High-income individuals with conservative spending habits.
- Strategy: Provide awareness of premium services and exclusive deals.

### Cluster 3: Older, Low Income, Low Spenders
- Elderly demographic with limited income and minimal spending.
- Strategy: Focus on affordability, senior discounts, and loyalty programs.

### Cluster 4: Young, Medium Income, Medium Spenders
- Middle-class young adults with average spending.
- Strategy: Engage with loyalty programs, mobile-first campaigns, and social media.

These insights help the business tailor marketing strategies, product placement, and customer service.

---

## Output Samples

All plots and reports are saved in the outputs/ directory:

- Correlation heatmap
- ![correlation_heatmap](https://github.com/user-attachments/assets/1b0ede9d-db1c-4b25-9faa-fe779aeea3db)

- Pairplot
- ![pairplot](https://github.com/user-attachments/assets/de98c6d9-e337-4d60-ad76-6cefe96cfa98)

- Elbow Method and Silhouette Analysis plot
- ![elbow_silhouette](https://github.com/user-attachments/assets/0b507d41-4359-4ba8-9e20-05a915cd14c7)

- PCA Cluster visualization
- ![pca_clusters](https://github.com/user-attachments/assets/9018561d-4821-4c58-8e03-b51bc858ec75)

- Distribution plots by feature
-![dist_Age](https://github.com/user-attachments/assets/4f790017-dbf9-4221-a12a-14372ef66b48)
![dist_Annual Income (k$)](https://github.com/user-attachments/assets/a3f3728f-f9de-4c74-bcdc-d9e53dbb3b98)
![dist_Spending Score (1-100)](https://github.com/user-attachments/assets/2a827e2b-f046-44a3-8be8-0849cab4c8ad)
![dist_Gender](https://github.com/user-attachments/assets/497188df-e42c-4939-ac1f-ab6356983061)

- Cluster summary as a CSV file


## Results

- Optimal number of clusters: 5
- Silhouette Score: Approximately 0.44 (moderate cluster separation)
- Clear segmentation based on age, income, and spending score

---

## Conclusion

This project successfully demonstrates how K-Means clustering can be applied to segment customers in a retail setting. Through exploratory data analysis, dimensionality reduction, and cluster evaluation, meaningful customer groups were identified based on spending behavior, income level, and age. These segments offer valuable insights that can guide targeted marketing strategies, personalized services, and overall customer relationship management. The approach is scalable and can be extended to other domains requiring behavioral segmentation.
