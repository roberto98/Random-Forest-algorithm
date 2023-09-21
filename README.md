# Random Forest for Data Classification
📚 "Machine Learning" project (Artificial Intelligence, UniGe)

A detailed report and a presentation on this project can be found here:
- [Random_Forest_algorithm_report.pdf](https://github.com/roberto98/Random-Forest-algorithm/files/12685478/project_presentation_random_forest.pdf)
- [Random_Forest_algorithm_presentation.pdf](https://github.com/roberto98/Random-Forest-algorithm/files/12685477/report_random_forest.pdf)

## Overview
This repository contains the implementation of the Random Forest algorithm, a supervised machine learning method used for classification and regression tasks. It combines the output of multiple decision trees to reach a single result by taking the average or majority of predictions. The algorithm's success is attributed to the low correlation between its models (trees), making it an extension of the bagging method that utilizes both bagging and feature randomness.

![image](https://github.com/roberto98/Random-Forest-algorithm/assets/32781888/7dc03de0-d0e4-4091-896a-dfaacd508868)

Here's a more schematic representation of the Random Forest algorithm:

1. **Data Generation:**
  - A training set is created by drawing a data sample from the original dataset with replacement, called the bootstrap sample.
  - One-third of the training sample is set aside as test data, known as the out-of-bag (oob) sample.

2. **Construction and Training of the Model:**
  - Each tree in the ensemble is created from a bootstrap sample.
  - Feature randomness is introduced through a random selection of features to split each node, adding more diversity to the dataset and reducing the correlation among decision trees.

3. **Cross-Validation and Prediction:**
  - The oob sample is used for cross-validation, finalizing the prediction.
  - The algorithm's output is based on majority voting or averaging, which helps solve the problem of overfitting.
  - The Random Forest algorithm is very stable, as even if a new data point is introduced in the dataset, the overall algorithm is not affected much since new data may impact one tree, but it is challenging for it to impact all the trees.

## Advantages and Disadvantages of the Random Forest algorithm
**Advantages:**
- It can be used in classification and regression problems.
- It's more accurate than the decision tree algorithm.
- It solves the problem of overfitting.
- This algorithm is very stable.

**Disadvantages:**
- It is highly complex compared to decision trees.
- Training time is longer compared to other models due to its complexity.


## ⚙ How to Run
To run the Random_Forest_algorithm.ipynb file, follow these steps:

1. Download the Random_Forest_algorithm.ipynb file from the provided link.
2. Install the required libraries by running the following commands in your terminal or command prompt:
  ```
  pip install numpy
  pip install pandas
  pip install scikit-learn
  pip install matplotlib
  ```
3. Open the Random_Forest_algorithm.ipynb file using Jupyter Notebook or any other compatible IDE.
4. Run the cells in the notebook sequentially, following the instructions and comments provided in the notebook.
