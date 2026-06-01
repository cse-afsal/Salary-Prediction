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

### 2. Load Dataset


### 3. Select Features and Target

### 4. Split Dataset


### 5. Train the Model


### 6. Make Predictions


### 7. Evaluate the Model


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


## 🚀 Future Improvements

- Add more features such as:
  - Education Level
  - Job Role
  - Location
  - Skills
  - Company Size


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
