# 🧠 HR Employee Attrition Prediction

## 📄 Overview
This project analyzes employee attrition using real-world HR data to identify patterns that lead to employee turnover.  
The goal was to build a reliable machine learning pipeline that predicts whether an employee is likely to leave the organization and helps HR teams act proactively.

We experimented with **multiple algorithms** — from interpretable statistical models to modern deep learning — to understand trade-offs between explainability, performance, and scalability.

---

## 🚀 Project Objectives
- Perform **exploratory data analysis (EDA)** to uncover factors driving attrition  
- Build a **machine learning pipeline** for preprocessing, feature encoding, and modeling  
- Compare multiple models:
  - **Logistic Regression** → Baseline interpretability  
  - **Random Forest Classifier** → Nonlinear performance benchmark  
  - **Neural Network (TensorFlow/Keras)** → Deep relationship modeling  
- Evaluate performance and determine the most suitable approach

---

## 🧩 Dataset
- **Source:** [IBM HR Analytics Employee Attrition Dataset (Kaggle)](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Size:** 1470 rows × 35 columns  
- **Target Variable:** `Attrition` (Yes / No)  
- **Key Features:**
  - Demographics (Age, Gender, MaritalStatus)  
  - Job-related (JobRole, Department, Overtime, YearsAtCompany)  
  - Satisfaction and performance metrics  

---

## ⚙️ Preprocessing
- Encoded binary and categorical features using **LabelEncoder** and **One-Hot Encoding**
- Removed irrelevant columns (`EmployeeNumber`, etc.)
- Standardized features using **StandardScaler**
- Split dataset into training and test sets (80/20 split with stratification)

---

## 🧮 Models Implemented

| Model | Purpose | Key Insights |
|--------|----------|--------------|
| **Logistic Regression** | Baseline linear model | High interpretability, shows direct feature impact |
| **Random Forest Classifier** | Ensemble model for nonlinear relationships | Captures feature interactions and improves accuracy |
| **Neural Network (TensorFlow)** | Deep model with hidden layers | Learns complex dependencies; strong generalization potential |

---

## 🧠 Model Comparison
| Metric | Logistic Regression | Random Forest | Neural Network |
|---------|--------------------|---------------|----------------|
| Interpretability | ⭐⭐⭐⭐ | ⭐⭐ | ⭐ |
| Accuracy | Moderate | High | High (with tuning) |
| Overfitting Risk | Low | Medium | High (regularized with Dropout) |
| Training Speed | Fast | Medium | Slow |
| Scalability | Good | Good | Excellent |

Each model served a purpose:
- **Logistic Regression** → Business interpretability  
- **Random Forest** → Balanced accuracy and feature interaction  
- **Neural Network** → Captures deeper patterns and can scale with more data  

---

## 📈 Results
- Random Forest provided the best balance of **accuracy** and **stability** for tabular data.  
- Neural Network in TensorFlow achieved similar results but required careful tuning (batch size, learning rate, dropout).  
- Logistic Regression remained valuable for **explainable insights** in HR discussions.

---

## 🧰 Tech Stack
- **Languages:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, TensorFlow/Keras  
- **Environment:** Jupyter Notebook  

---

## 💡 Future Improvements
- Handle class imbalance with **SMOTE** or **weighted loss**  
- Optimize neural network with **EarlyStopping** and **Learning Rate Scheduling**  
- Deploy via **Streamlit dashboard** for HR decision support  

---

## 🧍 Author
**Siddhardha Naidu Gorja**  
- Data Analyst & Machine Learning Enthusiast  
- Focused on applied analytics, automation, and real-world problem solving  
- [GitHub Profile](#) | [LinkedIn](#)
