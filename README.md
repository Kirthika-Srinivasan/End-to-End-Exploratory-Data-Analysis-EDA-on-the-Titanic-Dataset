# 🚢 Exploratory Data Analysis & Survival Prediction on the Titanic Dataset

An end-to-end exploratory data analysis (EDA) and baseline machine-learning pipeline to understand and predict passenger survival on the Titanic dataset.

---

## 📌 Objective

The main objective of this project is to:

- Explore and understand the factors that influenced passenger survival on the Titanic.
- Perform structured exploratory data analysis using visualisations and summary statistics.
- Prepare and transform the data for modelling.
- Build a baseline machine-learning model to predict survival.
- Evaluate model performance and interpret the results.

This notebook focuses primarily on **insight generation through EDA**, followed by a **simple and interpretable predictive model**.

---

## 📊 Dataset

This project uses the popular **Titanic dataset from Kaggle**.

The dataset contains information for **891 passengers**, including demographic, ticket, and travel-related attributes.

### Key features

| Feature        | Description |
|---------------|-----------|
| PassengerId  | Unique identifier for each passenger |
| Survived     | Target variable (0 = did not survive, 1 = survived) |
| Pclass       | Passenger class (1 = First, 2 = Second, 3 = Third) |
| Name         | Passenger name |
| Sex          | Gender |
| Age          | Age in years |
| SibSp        | Number of siblings / spouses aboard |
| Parch        | Number of parents / children aboard |
| Ticket       | Ticket number |
| Fare         | Passenger fare |
| Cabin        | Cabin number (many missing values) |
| Embarked     | Port of embarkation |

The dataset is well-suited for:

- binary classification
- feature importance analysis
- exploratory visualisation of social and economic patterns

---

## 🧠 Model Architecture

The notebook follows a simple and transparent modelling pipeline:

### 1. Data preprocessing
- Missing value handling for key variables (such as `Age` and `Embarked`)
- Removal or limited use of high-missing features (such as `Cabin`)
- Encoding of categorical variables

### 2. Feature preparation
- Selection of core explanatory variables:
  - `Pclass`, `Sex`, `Age`, `Fare`, `SibSp`, `Parch`, `Embarked`
- Conversion of categorical variables into numeric form

### 3. Classification model

A **binary classification model** is trained to predict:

Typical models used for survival prediction include:

- Logistic Regression
- Random Forest Classifier
- Support Vector Machine (SVM)
- Gradient Boosting Machines

In many Titanic tutorials, Logistic Regression is a baseline because it’s simple and interpretable for binary classification. More advanced or ensemble methods (e.g., Random Forest) may be compared for performance.


## 📈 Evaluation & Performance

Model performance is evaluated using:

- **Accuracy**
- **Confusion matrix**
- **Train / validation split**

The evaluation focuses on:

- how well the model generalises to unseen data
- whether the extracted features from EDA translate into predictive power

Typical validation accuracy for this setup lies in the range of:

**~70% – 85%**, depending on:
- feature selection
- handling of missing values
- model configuration

The goal is not leaderboard optimisation, but rather:
**consistent and explainable performance.**
