# 🚢 Titanic Survival Prediction using Machine Learning

A Machine Learning project that predicts whether a passenger survived the Titanic disaster based on demographic and travel-related information. This project demonstrates the complete Machine Learning pipeline, from data preprocessing and exploratory data analysis (EDA) to model training, evaluation, and prediction.

## 📌 Overview

The Titanic Survival Prediction project uses historical passenger data from the Titanic disaster to predict survival outcomes. By applying Machine Learning techniques, the model learns patterns from passenger information and determines the probability of survival.

This project is ideal for understanding:

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Classification Algorithms
- Model Evaluation
- Predictive Analytics

---

## 📊 Dataset Information

The dataset contains information about Titanic passengers and whether they survived.

### Features Included

| Feature | Description |
|----------|------------|
| PassengerId | Unique Passenger Identifier |
| Survived | Survival Status (0 = No, 1 = Yes) |
| Pclass | Passenger Class (1st, 2nd, 3rd) |
| Name | Passenger Name |
| Sex | Gender |
| Age | Passenger Age |
| SibSp | Number of Siblings/Spouses Aboard |
| Parch | Number of Parents/Children Aboard |
| Ticket | Ticket Number |
| Fare | Passenger Fare |
| Cabin | Cabin Information |
| Embarked | Port of Embarkation |

### Target Variable

```text
Survived
0 = Did Not Survive
1 = Survived
```

---

## 🎯 Features

✅ Data Cleaning and Preprocessing

✅ Missing Value Handling

✅ Data Visualization

✅ Feature Encoding

✅ Logistic Regression Model

✅ Model Evaluation

✅ Survival Prediction

✅ Performance Analysis

---

## 🛠️ Technologies Used

### Programming Language

- Python

### Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

### Development Environment

- Jupyter Notebook

---

## 🔄 Project Workflow

### Step 1: Data Collection

The Titanic dataset is loaded into a Pandas DataFrame and inspected for structure, missing values, and data types.

### Step 2: Data Cleaning

The dataset contains missing values which are handled appropriately.

#### Missing Value Treatment

- Cabin column removed due to excessive missing values.
- Missing Age values replaced using the mean age.
- Missing Embarked values filled using the most frequent category.

### Step 3: Exploratory Data Analysis (EDA)

EDA is performed to understand the relationship between passenger attributes and survival.

Analysis includes:

- Survival Distribution
- Gender Distribution
- Passenger Class Distribution
- Survival by Gender
- Survival by Passenger Class

### Step 4: Data Visualization

Several visualizations are generated:

- Count Plot of Survival Status
- Gender Distribution Plot
- Survival vs Gender Plot
- Passenger Class Distribution Plot
- Passenger Class vs Survival Plot

### Step 5: Feature Encoding

Machine Learning models require numerical inputs.

#### Gender Encoding

| Gender | Value |
|----------|----------|
| Male | 0 |
| Female | 1 |

#### Embarked Encoding

| Port | Value |
|----------|----------|
| S | 0 |
| C | 1 |
| Q | 2 |

### Step 6: Feature Selection

The following features are selected for training:

```text
Pclass
Sex
Age
SibSp
Parch
Fare
Embarked
```

Target:

```text
Survived
```

### Step 7: Train-Test Split

Dataset division:

```text
Training Data : 80%
Testing Data  : 20%
```

Random State:

```python
random_state = 2
```

---

## 🤖 Model Building

### Logistic Regression

The project uses the Logistic Regression algorithm for binary classification.

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()
model.fit(X_train, Y_train)
```

### Why Logistic Regression?

- Simple and efficient
- Suitable for binary classification
- Easy to interpret
- Good baseline model

---

## 📈 Results

### Model Accuracy

| Metric | Accuracy |
|----------|----------|
| Training Accuracy | 80.76% |
| Testing Accuracy | 78.21% |

The model achieves nearly 80% accuracy and successfully captures important survival patterns within the dataset.

---

## 📊 Visualizations Included

The notebook contains the following visual analyses:

### Survival Distribution

Shows the number of passengers who survived versus those who did not survive.

### Gender Distribution

Displays the count of male and female passengers.

### Gender vs Survival

Illustrates survival rates across genders.

### Passenger Class Distribution

Displays the distribution of passengers among different classes.

### Passenger Class vs Survival

Shows how passenger class influenced survival probability.

---

## ▶️ Usage

1. Open the notebook.
2. Run all cells sequentially.
3. Observe data preprocessing steps.
4. Explore visualizations.
5. Train the Logistic Regression model.
6. Evaluate performance metrics.
7. Generate survival predictions.

---

## 📂 Project Structure

```text
CODTECH-Projects/
│
├── Project1_Titanic_Survival_Prediction.ipynb
├── Titanic-Dataset.csv
├── README.md
│
└── outputs/
    ├── survival_analysis.png
    ├── gender_distribution.png
    ├── pclass_distribution.png
    └── model_results.png
```

---

## 💡 Key Insights

### Gender Matters

Female passengers had a significantly higher survival rate compared to male passengers.

### Passenger Class Matters

First-class passengers had a greater chance of survival than second and third-class passengers.

### Age Influence

Younger passengers generally showed better survival probabilities.

### Socioeconomic Factors

Ticket class and fare were important indicators of survival likelihood.

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:
```
- Data Preprocessing
- Handling Missing Values
- Feature Engineering
- Data Visualization
- Machine Learning Algorithms
- Model Evaluation
- Predictive Modeling
- End-to-End ML Workflow

---
```
