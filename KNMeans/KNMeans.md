# 💠 K-Means Clustering – Summary "The Pinguins"

## What is K-Means?

- K-Means is an **unsupervised learning algorithm** used for **clustering**.
- It groups data into `k` clusters based on **feature similarity** (usually Euclidean distance).
- The goal: **Minimize intra-cluster distance** and **maximize inter-cluster distance**.

## How It Works

1. Choose number of clusters `k`.
2. Randomly initialize `k` cluster centroids.
3. Repeat until convergence:
   - Assign each point to the **nearest centroid**.
   - Recalculate centroids as the **mean of assigned points**.
4. Stop when centroids don't change (or change very little).

## Key Concepts

- **Centroid**: The "center" of a cluster (mean of its members).
- **Inertia**: Sum of squared distances from points to their centroids – used as a cost function.
- **Initialization matters** – use `k-means++` to reduce randomness.
- You must define `k` in advance – or test multiple values and use methods like the **Elbow method**.

## Pros

- Simple and fast
- Works well when clusters are well-separated and spherical
- Scales to large datasets

## Cons

- Requires choosing `k` in advance
- Sensitive to initial centroids and outliers
- Assumes clusters of similar size/density (not good for complex shapes)

## Summary

> K-Means is used to group similar data points into `k` clusters  
> by minimizing distance to the cluster centroids. It's unsupervised,  
> meaning it works without labeled data – but needs careful setup and tuning.
