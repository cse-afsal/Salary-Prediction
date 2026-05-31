# 💰 Salary Prediction Using Machine Learning

## 📌 Project Overview

This project predicts employee salaries based on their years of experience using Machine Learning. A Linear Regression model is trained on historical salary data and used to estimate salaries for new employees.

---

## 🎯 Objective

The objective of this project is to build a Machine Learning model that can predict an employee's salary based on years of experience.

---

## 📊 Dataset

The dataset contains the following columns:

| Column Name | Description |
|------------|-------------|
| YearsExperience | Number of years of work experience |
| Salary | Employee salary (Target Variable) |

### Sample Data

| YearsExperience | Salary |
|---------------|---------|
| 1.1 | 39343 |
| 1.3 | 46205 |
| 3.2 | 54445 |
| 5.0 | 66029 |
| 10.5 | 121872 |

---

## 🛠 Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn

---

## 📂 Project Structure

```text
salary-prediction/
│
├── salary_data.csv
├── salary_prediction.py
├── model.pkl
├── requirements.txt
└── README.md
```

---

## ⚙️ Machine Learning Workflow

### 1. Import Required Libraries

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import r2_score
```

### 2. Load Dataset

```python
data = pd.read_csv("salary_data.csv")
```

### 3. Select Features and Target

```python
X = data[['YearsExperience']]
y = data['Salary']
```

### 4. Split Dataset

```python
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42
)
```

### 5. Train the Model

```python
model = LinearRegression()
model.fit(X_train, y_train)
```

### 6. Make Predictions

```python
predictions = model.predict(X_test)
```

### 7. Evaluate the Model

```python
score = r2_score(y_test, predictions)
print("R² Score:", score)
```

---

## 📈 Data Visualization

```python
plt.scatter(X, y)
plt.plot(X, model.predict(X))
plt.xlabel("Years of Experience")
plt.ylabel("Salary")
plt.title("Salary Prediction using Linear Regression")
plt.show()
```

---

## 🔍 Example Prediction

```python
experience = [[7]]
predicted_salary = model.predict(experience)

print("Predicted Salary:", predicted_salary[0])
```

### Example Output

```text
Predicted Salary: 92000
```

> Note: The output may vary depending on the dataset used.

---

## 📏 Model Evaluation

### R² Score

The R² score measures how well the model fits the data.

| R² Score | Performance |
|-----------|------------|
| 1.0 | Perfect Fit |
| 0.9 - 1.0 | Excellent |
| 0.7 - 0.9 | Good |
| Below 0.7 | Needs Improvement |

---

## 🚀 Future Improvements

- Add more features such as:
  - Education Level
  - Job Role
  - Location
  - Skills
  - Company Size

- Use advanced algorithms:
  - Random Forest Regressor
  - XGBoost
  - Gradient Boosting
  - Neural Networks

- Deploy the model using:
  - Flask
  - Django
  - Streamlit

---

## 🎓 What I Learned

- Data Loading and Exploration
- Data Preprocessing
- Feature Selection
- Train-Test Splitting
- Linear Regression
- Model Evaluation
- Data Visualization
- Salary Prediction

---

## 📜 Conclusion

This project demonstrates how Linear Regression can be used to predict salaries based on years of experience. It is a beginner-friendly Machine Learning project that helps understand the complete ML workflow, from data preparation to prediction and evaluation.

---

### ⭐ If you found this project useful, consider giving it a star on GitHub.
