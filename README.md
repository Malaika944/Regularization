## Project: Linear Regression vs Ridge Regression on Diabetes Dataset

## Dataset
Used the **Diabetes dataset** from `sklearn.datasets` — a standard benchmark dataset for regression tasks.

## What I Did

### **1. Linear Regression**
- Loaded and split the diabetes dataset into **train/test sets**
- Trained a **Linear Regression** model
- Evaluated using **R² Score** and **RMSE**

### **2. Ridge Regression**
- Trained a **Ridge Regression** model on the same dataset
- Evaluated using the same metrics for **fair comparison**

##  Results

| Metric | Linear Regression | Ridge Regression |
|--------|:-----------------:|:----------------:|
| **R² Score** | Lower | ✅ Improved |
| **RMSE** | Higher | ✅ Reduced |

##  Key Takeaway
**Ridge Regression** outperformed Linear Regression by achieving a **higher R² score** and **lower RMSE**, showing that **L2 regularization** helps reduce overfitting and improves **model generalization** on unseen data.

##  Part 2: Ridge Regression on Custom Dataset

---

##  Dataset
Generated a **custom dataset** using `make_regression` from Scikit-Learn.

| Property | Details |
|----------|---------|
| **Source** | `sklearn.datasets.make_regression()` |
| **Type** | Regression |
| **Purpose** | Controlled dataset to test regularization effects |

---

##  What I Did

### **Step 1 — Linear Regression (Baseline)**
- Generated dataset using `make_regression`
- Trained a **Linear Regression** model
- Evaluated using **R² Score** and **RMSE**

### **Step 2 — Ridge Regression with Different Alpha Values**
- Applied **Ridge Regression** with multiple alpha values
- Compared how different alpha values affect model performance
- Observed the effect of **L2 regularization strength**

| Alpha Value | Effect |
|-------------|--------|
| **Small (0.001)** | Less penalty → closer to Linear Regression |
| **Medium (1, 10)** | Balanced regularization |
| **Large (100, 1000)** | Strong penalty → more regularization |

### **Step 3 — Built Custom MyRidge Class**
- Created **MyRidge from scratch** without using Sklearn
- Implemented Ridge Regression manually
- Compared results with Sklearn's Ridge to verify correctness

---

##  Key Takeaways

- **Alpha controls regularization strength** — higher alpha = more penalty
- Too small alpha = **overfitting** (like Linear Regression)
- Too large alpha = **underfitting** (model too simple)
- **Sweet spot alpha** gives best R² Score and lowest RMSE
- Custom **MyRidge class** gave same results as Sklearn ✅

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/ScikitLearn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
