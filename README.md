# 🧠 Predicting Employee Attrition Using Machine Learning

> A complete ML pipeline to predict whether an employee is likely to leave the company, using HR analytics data.

---

## 📌 Problem Statement

Employee attrition is a major issue faced by organizations. This project explores a machine learning-based solution using HR-related features to predict the likelihood of an employee leaving (Yes/No).

---

## 📂 Dataset

- Source: IBM HR Analytics Dataset
- Records: ~1,470 employees
- Target column: `Attrition` (`Yes` = left company, `No` = stayed)

---

## 🛠 Technologies & Tools Used

- **Python**
- **Pandas**, **NumPy**, **Matplotlib**, **Seaborn**
- **Scikit-learn** (Logistic Regression, Random Forest, model evaluation)
- **Jupyter Notebook**

---

## 🔄 Workflow

1. **Data Cleaning**
   - Handled categorical variables using `.map()` and `.apply()`
   - Verified no missing values

2. **Feature Engineering**
   - Encoded binary columns like `Gender`, `OverTime`, `Over18`
   - Dropped irrelevant columns (e.g., EmployeeCount, StandardHours)

3. **Train-Test Split**
   - Used 80-20 split with `train_test_split()`

4. **Model Training**
   - ✅ Logistic Regression for baseline
   - ✅ Random Forest for improved performance
   - Compared accuracy and precision scores

5. **Evaluation**
   - Confusion matrix, classification report
   - Accuracy score

---

## 🧪 Results

| Model             | Accuracy | Notes                         |
|------------------|----------|-------------------------------|
| LogisticRegression | ~84%     | Fast, interpretable baseline  |
| RandomForest       | ~88%     | Better performance, less interpretable |

---

## 📈 Visuals

- Bar plots for categorical distributions
- Correlation heatmap
- Feature importance (Random Forest)

---

## 📌 Key Learnings

- Binary classification pipeline using Scikit-learn
- Encoding string categories correctly using `apply()` and `map()`
- Model comparison using metrics, not just accuracy
- Avoiding common mistakes like data leakage and label mismatch

---

## 🧠 Author

**Siddhardha Naidu Gorja**  
[GitHub Profile](https://github.com/siddhardha23g)

---

## 📂 How to Run This

1. Clone the repo:
   ```bash
   git clone https://github.com/siddhardha23g/employee-attrition-ml.git
   cd employee-attrition-ml
