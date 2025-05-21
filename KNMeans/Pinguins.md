# 🐧 K-Means Clustering – Penguins Example

## Goal

Use **K-Means Clustering** to group penguins into `k = 3` clusters based on numeric features.  
This shows how K-Means can identify natural groups **without knowing the species**.

## Dataset

We use the **Palmer Penguins dataset** with features like:

- `bill_length_mm`
- `bill_depth_mm`
- `flipper_length_mm`
- `body_mass_g`

All species labels are **ignored** during clustering – they’re only used later for evaluation.

## Steps

1. Load and clean the dataset (remove NaN).
2. Standardize features using `StandardScaler`.
3. Apply `KMeans(n_clusters=3, init='k-means++', random_state=42)`.
4. Visualize the clusters with Matplotlib or Seaborn.
5. Compare clusters with actual species (optional, for evaluation only).

## Observations

- K-Means creates 3 clusters based on feature similarity.
- Cluster centers represent "average penguins" in each group.
- Clusters may not perfectly match species labels – **K-Means doesn't know what a species is**.
- Still, clusters often resemble actual species groups.

## Pros Demonstrated

- Shows unsupervised learning in action
- Reveals natural groupings in real-world data
- Easy to visualize in 2D or 3D

## Key Learning

> K-Means does not predict labels – it groups similar data points  
> into `k` clusters based purely on feature distance. Evaluation against  
> true labels (species) is only for measuring how good the clustering was.

