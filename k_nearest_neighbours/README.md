# k-Nearest Neighbors (kNN)

## Table of Contents

- [Section 1](#section-1): Intro to kNN
- [Section 2](#section-2): Classification with kNN
- [Section 3](#section-3): Hyperparameter Tuning for k with T-fold Cross Validation
- [Section 4](#section-4): Regression with kNN

## Section 1: Intro to kNN

In this section, we will introduce the k-Nearest Neighbors (kNN) algorithm, a versatile machine learning algorithm used for both classification and regression tasks. kNN is a non-parametric and lazy learning algorithm, which means it does not make any assumptions about the underlying data distribution and defers learning until predictions are needed.

## Section 2: Classification with kNN

kNN can be employed for classification tasks, where the goal is to assign a new data point to a specific class or category. In this section, we will explore how kNN works for classification. The algorithm starts by calculating the distance between the new data point and all other points in the dataset. Then, it selects the k nearest neighbors based on the chosen distance metric. The new data point is classified based on the majority class among its k nearest neighbors.

## Section 3: Hyperparameter Tuning for k with T-fold Cross Validation

The performance of kNN heavily depends on the value of k, the number of neighbors to consider. In this section, we will discuss the process of hyperparameter tuning for k using T-fold cross-validation. By evaluating the algorithm's performance for various k values on different subsets of the dataset, we can find the optimal k value that results in the best model performance.

## Section 4: Regression with kNN

In addition to classification, kNN can also be utilized for regression tasks, where the goal is to predict continuous values instead of discrete classes. In this section, we will explore how kNN can be adapted for regression. The algorithm works similarly to the classification case, but instead of taking the majority vote of the target values, it calculates the mean value of the target variable among its k nearest neighbors to make predictions.

kNN's simplicity and flexibility make it a valuable algorithm for various machine learning tasks, but selecting the appropriate k value and understanding its implications are critical for achieving optimal results.

