# 🌲 Random Forest – Summary

## What is Random Forest?

- Random Forest is a **supervised machine learning algorithm** used for both **classification and regression** tasks.
- It builds an **ensemble of Decision Trees** (`n_estimators`), each limited in depth (e.g. `max_depth=5`).

## Key Concepts

- **Bootstrapping**: Each tree is trained on a **random sample (with replacement)** from the original dataset.
- **Feature Bagging**: At each split, only a **random subset of features** is considered, not all features.
- This introduces variation: trees might have **different root nodes** and different splits, even on the same data.

## How the Final Decision is Made

- For classification: the algorithm uses a **majority vote** across all trees.
- For regression: it calculates the **average prediction** from all trees.

## Why Use Random Forest?

- It **reduces overfitting** that single Decision Trees often suffer from.
- It is an example of **ensemble learning**: multiple weak learners (trees) form a strong learner.
- It is generally more robust and accurate than a single Decision Tree.

## Summary

> A Random Forest is a collection of randomized Decision Trees working together.  
> Each tree sees a slightly different dataset and a different feature subset,  
> and the group decides together. The randomness introduces diversity,  
> and the ensemble makes the model powerful and stable.