# 🌳 Decision Tree Classifier – Summary

## What is a Decision Tree?

- A Decision Tree is a **supervised learning algorithm** used for **classification**.
- It learns **if/else rules** to split the dataset based on feature values.
- Each internal node represents a feature, each branch a decision, and each leaf a class label.

## How It Works

- Splits are made to **maximize class purity** (reduce impurity).
- Common criteria:
  - `gini` (Gini Impurity, default in scikit-learn)
  - `entropy` (Information Gain)
- The tree grows until:
  - A maximum depth (`max_depth`) is reached
  - A minimum number of samples is in a node (`min_samples_split`)
  - All leaves are pure (only one class)

## Pros

- Easy to understand and visualize
- No feature scaling needed
- Can capture non-linear relationships

## Cons

- High risk of **overfitting** (especially with deep trees)
- Can be sensitive to small data changes (instability)

## Summary

> A Decision Tree Classifier splits data into branches using feature values  
> to classify samples. It tries to create pure groups by maximizing  
> the separation between classes. Careful pruning or limits are needed  
> to avoid overfitting.
