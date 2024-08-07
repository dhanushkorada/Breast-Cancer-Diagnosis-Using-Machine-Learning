# Breast-Cancer-Diagnosis-Using-Machine-Learning
Welcome to the Breast Cancer Diagnosis project. This project focuses on predicting whether a breast cancer tumor is benign or malignant using machine learning techniques, utilizing the Breast Cancer Wisconsin (Original) Data Set from the UCI Machine Learning Repository.

## Table of Contents

- [Introduction](#introduction)
- [Dataset Information](#Dataset-Information)
- [Setup and Required Installs](#setup-and-required-installs)
- [Model Selection](#model-selection)
- [Hyperparameter Tuning](#hyperparameter-tuning)
- [Results](#results)
- [Conclusion](#conclusion)
- [License](#license)

## Introduction

Breast cancer is a common and potentially deadly disease, making early and accurate diagnosis crucial. This project aims to develop a machine learning model to classify breast cancer tumors as benign or malignant based on various features of cell nuclei obtained through fine needle aspiration. By identifying the key characteristics associated with malignant tumors, this model can assist healthcare professionals in making informed diagnostic decisions.

## Dataset Information
The Breast Cancer Wisconsin (Original) Data Set includes the following attributes:

1. Sample code number: id number
2. Clump Thickness: 1 - 10
3. Uniformity of Cell Size: 1 - 10
4. Uniformity of Cell Shape: 1 - 10
5. Marginal Adhesion: 1 - 10
6. Single Epithelial Cell Size: 1 - 10
7. Bare Nuclei: 1 - 10
8. Bland Chromatin: 1 - 10
9. Normal Nucleoli: 1 - 10
10. Mitoses: 1 - 10
11. Class: (2 for benign, 4 for malignant)

## Setup and Required Installs

To run the project, you need to set up your environment and install the required dependencies:

1. Clone this repository:

```git clone https://github.com/dhanushkorada/Breast-Cancer-Diagnosis-Using-Machine-Learning.git```
```cd Breast-Cancer-Diagnosis-Using-Machine-Learning```

2. Install the required dependencies:

```pip install -r requirements.txt```

## Model Selection

Several classification models are tested to predict the malignant cancer cells:

- KNN Classification
- Support Vector Machine
- Kernel SVM
- Decision Tree Classification
- Logistic Regression
- Naive Bayes

After evaluating the performance of various models using Accuracy Score the Decision Tree Classification model is chosen as the optimal model due to its higher accuracy in predictions.

## Hyperparameter Tuning
Hyperparameter tuning is performed using GridSearchCV to find the best parameters for the Decision Tree Classifier. The parameter grid includes:

- Criterion: ['gini', 'entropy']
- Splitter: ['best', 'random']
- Max Depth: [None, 10, 20, 30, 40, 50]
- Min Samples Split: [2, 5, 10]
- Min Samples Leaf: [1, 2, 4]

The best combination of parameters is selected based on cross-validation performance.

## Results
The results of the Decision Tree Classification model are discussed with the help of performance metrics in the Jupyter Notebook provided in the repository. These metrics provide insights into how well the model is able to distinguish between benign and malignant tumors.

## Conclusion
The Breast Cancer Diagnosis model developed in this project offers a valuable tool for early detection and diagnosis of breast cancer. By accurately predicting the nature of the tumor, healthcare professionals can make better-informed decisions, potentially improving patient outcomes.

## License

This project is licensed under the [MIT License](LICENSE).
