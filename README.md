# 🚢 Titanic Survival Prediction

### CodSoft Data Science Internship Project

A Data Science project that predicts whether a passenger survived the Titanic disaster based on demographic and travel-related information. This project demonstrates the complete data science workflow, including data preprocessing, exploratory data analysis (EDA), model training, evaluation, and prediction.

---

## 📌 Overview

The Titanic Survival Prediction project uses historical passenger data from the Titanic disaster to predict survival outcomes. By applying Machine Learning techniques, the model learns patterns from passenger information and estimates the probability of survival.

This project covers:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Classification Algorithms
* Model Evaluation
* Predictive Analytics

---

## 📊 Dataset Information

The dataset contains information about Titanic passengers and whether they survived.

### Features Included

| Feature     | Description                       |
| ----------- | --------------------------------- |
| PassengerId | Unique Passenger Identifier       |
| Survived    | Survival Status (0 = No, 1 = Yes) |
| Pclass      | Passenger Class (1st, 2nd, 3rd)   |
| Name        | Passenger Name                    |
| Sex         | Gender                            |
| Age         | Passenger Age                     |
| SibSp       | Number of Siblings/Spouses Aboard |
| Parch       | Number of Parents/Children Aboard |
| Ticket      | Ticket Number                     |
| Fare        | Passenger Fare                    |
| Cabin       | Cabin Information                 |
| Embarked    | Port of Embarkation               |

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
✅ Exploratory Data Analysis (EDA)
✅ Data Visualization
✅ Feature Encoding
✅ Logistic Regression Model
✅ Model Evaluation
✅ Survival Prediction

---

## 🛠️ Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

### Development Environment

* Google Colab

---

## 🔄 Project Workflow

### Step 1: Data Collection

Load the Titanic dataset into a Pandas DataFrame and inspect its structure.

### Step 2: Data Cleaning

* Removed the `Cabin` column due to excessive missing values.
* Replaced missing `Age` values using the mean.
* Filled missing `Embarked` values using the mode.

### Step 3: Exploratory Data Analysis (EDA)

Performed analysis on:

* Survival Distribution
* Gender Distribution
* Passenger Class Distribution
* Survival by Gender
* Survival by Passenger Class

### Step 4: Data Visualization

Generated:

* Survival Count Plot
* Gender Distribution Plot
* Survival vs Gender Plot
* Passenger Class Distribution Plot
* Passenger Class vs Survival Plot

### Step 5: Feature Encoding

#### Gender Encoding

| Gender | Value |
| ------ | ----- |
| Male   | 0     |
| Female | 1     |

#### Embarked Encoding

| Port | Value |
| ---- | ----- |
| S    | 0     |
| C    | 1     |
| Q    | 2     |

### Step 6: Feature Selection

Features Used:

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

```text
Training Data : 80%
Testing Data  : 20%
Random State  : 2
```

---

## 🤖 Model Building

### Logistic Regression

```python
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()
model.fit(X_train, Y_train)
```

### Why Logistic Regression?

* Simple and efficient
* Suitable for binary classification
* Easy to interpret
* Strong baseline model

---

## 📈 Results

| Metric            | Accuracy |
| ----------------- | -------- |
| Training Accuracy | 80.76%   |
| Testing Accuracy  | 78.21%   |

The model achieves nearly 80% accuracy and successfully captures important survival patterns within the dataset.

---

## 📂 Project Structure

```text
codsoft-Titanic-Survival-Prediction/
│
├── Titanic_Survival_Prediction.ipynb
├── Titanic-Dataset.csv
└── README.md
```

---

## 💡 Key Insights

* Female passengers had significantly higher survival rates.
* First-class passengers had a greater chance of survival.
* Younger passengers generally showed better survival probabilities.
* Passenger class and fare strongly influenced survival outcomes.

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

* Data Preprocessing
* Handling Missing Values
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Data Visualization
* Classification Algorithms
* Model Evaluation
* Predictive Modeling
* End-to-End Data Science Workflow

---

## 👨‍💻 Author

**Nigam Kumar**

🔗 GitHub: https://github.com/nigamkumar3435-spec

---

## ⭐ Acknowledgements

This project was developed as part of the **CodSoft Data Science Internship Program** and demonstrates the application of Data Science and Machine Learning techniques to predict passenger survival using historical Titanic data.

If you found this project useful, please consider giving the repository a ⭐ Star!
