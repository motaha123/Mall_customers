# Mall_customers
This Jupyter notebook performs a data analysis and clustering task on a dataset of mall customers, focusing on customer segmentation based on Annual Income and Spending Score.
1. Data Loading and Preprocessing
The dataset (Mall_Customers.csv) is loaded and cleaned by removing the CustomerID column.

Missing values are checked, and none are found.

The data includes gender, age, annual income, and spending score.

2. Exploratory Data Analysis (EDA)
Gender Distribution: A pie chart visualizes the distribution of male and female customers.

Age Analysis: Customers are categorized into age groups (18-29, 30-49, 50-70), and a count plot shows the distribution.

Income Analysis: A box plot visualizes the distribution of annual income, and outliers are removed using the Interquartile Range (IQR) method.

Spending Score Analysis: A box plot visualizes the spending score distribution.

3. Principal Component Analysis (PCA)
The data is standardized, and PCA is applied to reduce the dimensionality of the dataset (focusing on Annual Income and Spending Score).

Eigenvalues and eigenvectors are computed from scratch using Power Iteration and Deflation.

The data is projected onto the top 2 principal components for 2D visualization.

4. Clustering with K-Means
K-Means clustering is applied to both the original and PCA-reduced data.

The Silhouette Score is used to evaluate the clustering performance.

Clustering results are visualized for both the original and PCA-reduced data.

5. Key Insights
PCA reduces the dataset to 2 principal components, retaining most of the variance.

Clustering on PCA-reduced data yields a slightly better Silhouette Score compared to the original data.

Visualizations show distinct customer segments based on income and spending behavior.

Summary
This notebook demonstrates a data-driven approach to customer segmentation using PCA for dimensionality reduction and K-Means for clustering. The results help identify distinct customer groups, which can be useful for targeted marketing strategies.
