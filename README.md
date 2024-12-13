# Applied-Data-Science-2
# README: Exploring the K-Means Algorithm with FIFA 22 Player Dataset
# Overview
This project explores the K-Means clustering algorithm, focusing on its application to the FIFA 22 player dataset. The study evaluates the impact of different initialization methods and techniques for determining the optimal number of clusters, such as the Elbow Method and Silhouette Analysis. Additionally, we compare the effectiveness of Random Initialization and K-Means++ for centroid selection.
# Objectives
1.Apply K-Means clustering to segment FIFA 22 players based on attributes such as overall rating, potential, market value, wage, and age.

2.Determine the optimal number of clusters (K) using:

-**Elbow Method**
-**Silhouette Analysis**

3.Compare the performance of:

-**Random Initialization**
_**K-Means++ Initialization**
## Dataset
The dataset used is players_22.csv, containing detailed information about FIFA 22 players. Key features analyzed in this project include:

Overall: Current skill level of the player.

Potential: Projected skill improvement.

Value (EUR): Market value of the player.

Wage (EUR): Weekly wage in euros.

Age: Player's age.

# Methods and Implementation
# 1. K-Means Algorithm
 Clustering technique that minimizes within-cluster variance.
Steps:
1.Select K (number of clusters).

2.Initialize centroids (Random Initialization or K-Means++).

3.Assign points to the nearest centroid.

4.Update centroids and iterate until convergence.

# 2. Optimal K Determination

Elbow Method: Plots WCSS against K to identify the "elbow" point where improvement diminishes.

Silhouette Analysis: Measures how well points fit within their assigned clusters versus other clusters.

# 3. Initialization Methods

**Random Initialization**:Centroids selected randomly from the dataset.
**K-Means++**:Selects initial centroids based on distance, ensuring they are spread out.
# Key Findings
**Elbow Method** : Indicates K = 4 as a potential optimal value.
**Silhouette Analysis**: Suggests K = 2 for best cluster separation and cohesion.
**Initialization Comparison**:
**K-Means++** outperforms Random Initialization:
Produces lower WCSS and higher silhouette scores.
Achieves faster convergence and more stable clustering results.

# Results and Discussion
K = 2 yields the most meaningful clusters, as supported by the Silhouette Analysis.
K-Means++ provides better-defined clusters and outperforms Random Initialization in both accuracy and computational efficiency.

# Conclusion
The K-Means algorithm is highly effective for clustering tasks, but its performance depends on the choice of K and initialization method. Using the Elbow and Silhouette Methods, K = 2 was identified as the optimal number of clusters for the FIFA 22 dataset. K-Means++ consistently produced better results than Random Initialization, demonstrating its advantages in cluster quality and convergence speed.

