# Ad Click Prediction using Machine Learning

## Overview

This project builds a machine learning model to predict whether a user will click on an online advertisement based on demographic and behavioral features.

The dataset contains information about users such as:

* Daily time spent on site
* Age
* Area income
* Daily internet usage
* Gender
* Timestamp of interaction

The goal is to classify whether a user **clicked on an advertisement or not**.

---

## Dataset

The dataset contains **1000 observations** and multiple features describing user behavior and demographics.

Key features include:

* **Daily Time Spent on Site**
* **Age**
* **Area Income**
* **Daily Internet Usage**
* **Gender**
* **Timestamp**

Target variable:

```
Clicked on Ad
```

Values:

* `0` → User did not click the advertisement
* `1` → User clicked the advertisement

---

## Feature Engineering

Additional features were created from the timestamp:

* **Season** (Winter, Spring, Summer, Autumn)
* **Period of the day** (Morning / Evening)

Categorical variables were encoded using **One-Hot Encoding**.

---

## Machine Learning Models

Several classification algorithms were tested:

* Logistic Regression
* K-Nearest Neighbors
* Support Vector Machine
* Decision Tree
* Random Forest
* XGBoost
* Naive Bayes

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## Best Performing Model

The **Random Forest classifier** achieved the best performance on the test set.

Example results:

Accuracy: ~96%

---

## Libraries Used

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn
* xgboost
* joblib

---

## Model Saving

The trained model and scaler are saved using `joblib` for later use.

```
model.pkl
scaler.pkl
```

---

## Project Structure

```
project/
│
├── advertising.csv
├── notebook.ipynb
├── model.pkl
├── scaler.pkl
└── README.md
```

---


