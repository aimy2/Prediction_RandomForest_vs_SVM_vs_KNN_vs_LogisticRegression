# Income Prediction: Random Forest vs SVM vs KNN vs Logistic Regression

A machine learning project that predicts whether a person earns more or less than $50K per year using the UCI Adult (Census Income) dataset. Four classification algorithms are implemented and their performance is compared.

## 📋 Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Models](#models)
- [Requirements](#requirements)
- [Usage](#usage)
- [Results](#results)
- [Project Structure](#project-structure)

## Overview

This project benchmarks four supervised learning algorithms on the classic income classification problem. The goal is to predict whether an individual's annual income exceeds $50K based on demographic and employment features.

## Dataset

The project uses the **UCI Adult / Census Income** dataset, which contains the following features:
[DatasetLink:](https://www.kaggle.com/datasets/wenruliu/adult-income-dataset)

| Feature | Description |
|---|---|
| age | Age of the individual |
| workclass | Type of employer (Private, Self-emp, Gov, etc.) |
| fnlwgt | Final weight (census sampling weight) |
| education | Highest level of education |
| education-num | Number of years of education |
| marital-status | Marital status |
| occupation | Type of occupation |
| relationship | Relationship status |
| race | Race of the individual |
| sex | Gender |
| capital-gain | Capital gain |
| capital-loss | Capital loss |
| hours-per-week | Average hours worked per week |
| native-country | Country of origin |
| income | **Target**: `<=50K` or `>50K` |

## Models

Four classification models are trained and evaluated:

1. **Random Forest** — An ensemble of decision trees that reduce overfitting through bagging and feature randomness.
2. **Support Vector Machine (SVM)** — Finds the optimal hyperplane that maximizes the margin between classes.
3. **K-Nearest Neighbors (KNN)** — Classifies a sample based on the majority vote of its K nearest neighbors.
4. **Logistic Regression** — A linear probabilistic classifier that estimates class membership probabilities.

## Requirements

```
Python >= 3.7
pandas
numpy
scikit-learn
matplotlib
seaborn
```


## Usage

1. **Clone the repository**

```bash
git clone https://github.com/aimy2/Prediction_RandomForest_vs_SVM_vs_KNN_vs_LogisticRegression.git
cd Prediction_RandomForest_vs_SVM_vs_KNN_vs_LogisticRegression
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Run the main script**

```bash
python main.py
```

This will:
- Load and preprocess the dataset
- Train all four models
- Evaluate and compare their accuracy, precision, recall, and F1-score
- Display a comparison chart of model accuracies

## Results

The models are compared using the following metrics:

- **Accuracy** — Overall fraction of correct predictions
- **Precision** — Fraction of positive predictions that are actually positive
- **Recall** — Fraction of actual positives that are correctly identified
- **F1-Score** — Harmonic mean of precision and recall

A bar chart is generated to visualize the accuracy of all four models side-by-side.

## Project Structure

```
Prediction_RandomForest_vs_SVM_vs_KNN_vs_LogisticRegression/
│
├── Datasets/
│   └── adult.csv            # UCI Adult / Census Income dataset
│
├── allmodelscomparison.ipynb   # Entry point — trains and evaluates all models
└── README.md                # Project documentation
```

## Author

**Syeda Aiman Mumtaz Sherazi** — [GitHub](https://github.com/aimy2)
