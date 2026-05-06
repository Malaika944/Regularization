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

## 📈 Results

| Metric | Linear Regression | Ridge Regression |
|--------|:-----------------:|:----------------:|
| **R² Score** | Lower | ✅ Improved |
| **RMSE** | Higher | ✅ Reduced |

## 💡 Key Takeaway
**Ridge Regression** outperformed Linear Regression by achieving a **higher R² score** and **lower RMSE**, showing that **L2 regularization** helps reduce overfitting and improves **model generalization** on unseen data.
