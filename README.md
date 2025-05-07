# Mall-Customers---K-means-Clustering
This project implements K-Means Clustering using Scikit-learn to segment customers based on selected features from a retail dataset.

# Objective
The main objective of this project is to apply unsupervised learning using K-Means clustering to identify different groups of customers based on their age, annual income, and spending score. This helps in better customer understanding and targeted marketing.

Tools and Libraries Used

Python, 
Pandas, 
Matplotlib, 
Seaborn, 
Scikit-learn &
Colab

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
The dataset was read using Pandas. Columns like CustomerID and Gender were dropped. Features were scaled using StandardScaler to normalise values before clustering.

**PCA for Visualisation**
Principal Component Analysis (PCA) was optionally applied to reduce the 3D feature space to 2D. This made it easier to visualize clusters.

**Elbow Method**
The Elbow Method was used to determine the optimal number of clusters by plotting the inertia for different values of k (typically from 1 to 10). The 'elbow' point on the graph suggests the ideal number of clusters.

**Applying K-Means**
K-Means was applied using the selected value of k. The resulting cluster labels were added to the dataset.

**Visualisation of Clusters**
The data was plotted using the first two principal components (if PCA was used), with points colour-coded according to their assigned cluster.

**Evaluation**
Silhouette Score was used to evaluate how well-separated the clusters are. A higher score indicates better clustering performance.

# Result
The K-Means clustering model successfully segmented the customers into 5 distinct groups based on their age, income, and spending behaviour. Visualisations using PCA showed clear boundaries between clusters, and the silhouette score confirmed good clustering performance. These insights can help in creating targeted marketing campaigns.

# Future Insights
This project can be extended by integrating demographic or transactional data for more accurate segmentation. It can also be deployed as a web dashboard where businesses upload their customer data and get instant cluster analysis. Adding advanced clustering techniques like DBSCAN or hierarchical clustering can further enhance the model’s capability.
