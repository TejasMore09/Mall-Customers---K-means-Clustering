# Mall-Customers---K-means-Clustering
This project implements K-Means Clustering using Scikit-learn to segment customers based on selected features from a retail dataset.

# Objective
The main objective of this project is to apply unsupervised learning using K-Means clustering to identify different groups of customers based on their age, annual income, and spending score. This helps in better customer understanding and targeted marketing.

Tools and Libraries Used

Python
Pandas
Matplotlib
Seaborn
Scikit-learn

# Dataset Overview
The dataset contains 200 records with the following fields:

CustomerID
Gender
Age
Annual Income 
Spending Score 

Only numerical fields were used for clustering. Gender was ignored to avoid additional preprocessing like encoding.

# Steps Performed

**Data Loading and Preprocessing**
The dataset was read using Pandas. Columns like CustomerID and Gender were dropped. Features were scaled using StandardScaler to normalize values before clustering.

**PCA for Visualization**
Principal Component Analysis (PCA) was optionally applied to reduce the 3D feature space to 2D. This made it easier to visualize clusters.

**Elbow Method**
The Elbow Method was used to determine the optimal number of clusters by plotting the inertia for different values of k (typically from 1 to 10). The 'elbow' point on the graph suggests the ideal number of clusters.

**Applying K-Means**
KMeans was applied using the selected value of k. The resulting cluster labels were added to the dataset.

**Visualization of Clusters**
The data was plotted using the first two principal components (if PCA was used), with points color-coded according to their assigned cluster.

**Evaluation**
Silhouette Score was used to evaluate how well-separated the clusters are. A higher score indicates better clustering performance.
