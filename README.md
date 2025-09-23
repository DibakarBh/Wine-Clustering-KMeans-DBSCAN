- Interpretation of K-Means Clusters

# Cluster 1: Represents wines with higher tartness and richness (e.g., higher Malic_Acid and Color_Intensity) but fewer antioxidant properties(e.g. lower Flavanoids and OD280).

# Cluster 2: Groups antioxidant-rich wines with higher Alcohol and Flavanoids, indicating a strong and bold flavor profile.

# Cluster 3: Contains lighter wines with more balanced chemical attributes and relatively moderate Alcohol levels.

- Interpretation of DBSCAN Clusters:
# Cluster 1: The largest cluster, with 110 points (90 core and 20 border points). This represents the majority group of wine samples with similar principal component patterns.
# Cluster 2: A smaller but distinct cluster with 44 points (39 core and 5 border points), likely representing a subgroup of wines with unique characteristics.
# Noise (Cluster 0): Contains 24 points classified as noise, indicating outliers that do not belong to any dense cluster.

Influence of ε and minPts

- ε (epsilon): Defines the radius of a neighborhood. A small ε leads to many small clusters or noise points, while a large ε may merge distinct clusters.
- minPts: Minimum points required to form a dense cluster. A higher value reduces noise but may miss smaller clusters.

- Comparison of K-Means and DBSCAN
Feature 	K-Means 	DBSCAN
Requires k? 	Yes 	No
Handles Outliers? 	No 	Yes
Works for Arbitrary Shapes? 	No 	Yes
Cluster Density Sensitivity 	No 	Yes

- Conclusion

    K-Means is efficient for well-separated, spherical clusters.
    DBSCAN is useful for detecting noise and irregularly shaped clusters.
    The choice depends on dataset characteristics and clustering goals.

