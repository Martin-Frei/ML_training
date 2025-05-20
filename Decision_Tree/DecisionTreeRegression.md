# 🌿 Decision Tree Regressor – Summary

## What is a Decision Tree Regressor?

- A Decision Tree Regressor is used for **predicting continuous numeric values**.
- Like the classifier, it uses **recursive splitting** of the data based on feature thresholds.

## How It Works

- The algorithm splits data into regions where each **leaf node holds a constant value** (mean of the target in that region).
- Splits are chosen to **minimize the mean squared error (MSE)** within each region.
- Parameters like `max_depth`, `min_samples_split`, and `min_samples_leaf` control the complexity.

## Pros

- Captures non-linear patterns
- No need for feature scaling
- Can handle mixed feature types (categorical + numerical)

## Cons

- Easily **overfits** if not properly regularized
- Predictions are **not smooth** (stepwise output)

## Summary

> A Decision Tree Regressor breaks the feature space into rectangular  
> regions and predicts the mean target value in each region.  
> It's simple and interpretable but prone to overfitting.
