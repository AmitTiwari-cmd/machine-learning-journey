# Decision Trees

## Purpose

Decision Trees are supervised machine learning algorithms used for both Classification and Regression problems.

## Key Idea

A Decision Tree splits data into smaller groups based on feature values until it can make predictions.

Example:

Petal Length < 2.5 ?

* Yes → Iris Setosa
* No → Further Split

The model learns these decision rules from training data.

---

## Important Concepts

### Root Node

The first node of the tree where the initial split occurs.

### Internal Node

A node that further splits the data.

### Leaf Node

The final node that gives the prediction.

### Entropy

Measures the impurity or randomness of a dataset.

Lower entropy = more pure data.

### Information Gain

Measures how much entropy decreases after a split.

The tree chooses the split with the highest Information Gain.

### Gini Impurity

Another measure of impurity used instead of Entropy.

---

## Workflow

1. Load Dataset
2. Data Preprocessing
3. Train-Test Split
4. Train Decision Tree
5. Make Predictions
6. Evaluate Model
7. Tune Hyperparameters

---

## Important Hyperparameters

### max_depth

Maximum depth of the tree.

* Small depth → Underfitting
* Large depth → Overfitting

### min_samples_split

Minimum samples required to split a node.

### min_samples_leaf

Minimum samples required in a leaf node.

### criterion

Method used to choose splits.

Options:

* gini
* entropy

---

## Overfitting

Decision Trees can easily memorize training data.

Example:

Train Accuracy = 100%
Test Accuracy = 60%

This indicates overfitting.

Reducing max_depth can help prevent overfitting.

---

## Advantages

* Easy to understand
* Easy to visualize
* Handles non-linear data
* Requires little data preprocessing

---

## Disadvantages

* Can overfit easily
* Sensitive to small data changes
* Single trees may not generalize well

---

## Evaluation Metrics

For Classification:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## Project Completed

### Iris Flower Species Classification

Features:

* Sepal Length
* Sepal Width
* Petal Length
* Petal Width

Target:

* Iris Setosa
* Iris Versicolor
* Iris Virginica

### Hyperparameter Tuning

Tested different values of:

max_depth = 1 to 10

Observation:

* Depth 1–2 → Lower Accuracy (~94–95%)
* Depth 3 → Achieved 100% Accuracy
* Higher depths did not improve performance

---

## Interview Questions

Q. What is a Decision Tree?

A. A supervised learning algorithm that makes predictions using a tree-like structure of decisions.

Q. What causes overfitting in Decision Trees?

A. Excessive tree depth and overly specific splits.

Q. How can overfitting be reduced?

A. By tuning max_depth, min_samples_split, and min_samples_leaf.

Q. Difference between Entropy and Gini?

A. Both measure impurity. Entropy uses logarithms, while Gini is computationally simpler.

---

## Revision Keywords

Decision Tree, Entropy, Information Gain, Gini Impurity, Overfitting, max_depth, Hyperparameter Tuning, Classification.
