# Validating Clusters

A quick summary of [this Wikipedia article](https://en.wikipedia.org/wiki/Cluster_analysis#Evaluation_and_assessment) about evaluating and assesing clusters.

**Last update**: 2017-07-09

## Internal evaluation

Evaluate the clusters based on the data that was actually clustered. E.g., a method will score high if most clusters have high within-cluster similarity but a low similarity between different clusters.

### Statsistics 

- Davies–Bouldin index
- Dunn index
- Silhouette coefficient

### Issues 

A major issue is that a clustering method will score better on the test if the clustering method and the test method make similar assumptions.

## External evaluation

Comparing cluster results to "gold-standards". These gold-standards are generally curated by domain experts. So a clustering method will score higher if it is more similar to the gold-standard.

### Statistics

- Purity
- Rand measure
- F measure
- Jaccard index (used to quantify similarity between two datasets)
- Fowlkes–Mallows index
- Mutual information
- Confusion matrix

## Cluster tendency

If you're interested in whether your data even has clusters, you can check for this. One way is to compare your actual data with random data with the idea that random data should not have clusters. 

### Statistics

There are some statistics (Hopkins stat) that measure for this but they often are not great for real data as they often measure deviation from a uniform distribution.