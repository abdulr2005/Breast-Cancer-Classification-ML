# Diagnostic Breast Cancer Classification

This project aims to classify breast cancer tumors as **Malignant** or **Benign** using machine learning techniques based on clinical characteristics.

## 📊 Dataset Overview
The dataset contains 30 features derived from a digitized image of a fine needle aspirate (FNA) of a breast mass. 
- **Target:** Diagnosis (Malignant = 1, Benign = 0)
- **Features:** Mean, standard error, and "worst" of radius, texture, perimeter, area, smoothness, etc.

## 🛠️ Technologies Used
- **Python** (Pandas, NumPy)
- **Scikit-learn** (Logistic Regression, Random Forest)
- **Matplotlib & Seaborn** (Data Visualization)

## 🚀 Project Workflow
1. **Data Preprocessing:** Handled missing values (if any), dropped unnecessary columns (ID), and encoded the target variable.
2. **Feature Scaling:** Applied `StandardScaler` to normalize the data for the Logistic Regression model.
3. **Modeling:**
   - **Logistic Regression:** Used as a baseline classifier.
   - **Random Forest:** Used to handle non-linear relationships and identify feature importance.
4. **Evaluation:** Measured performance using Accuracy, Recall, and Confusion Matrix.

## 📈 Results Comparison

| Model | Accuracy | Recall (Malignant) |
| :--- | :---: | :---: |
| **Logistic Regression** | 98.2% | 0.98 |
| **Random Forest** | 96.5% | 0.93 |

> **Note:** Logistic Regression performed better in terms of Recall, which is crucial in medical diagnosis to minimize false negatives.

## 🔍 Key Insights (Feature Importance)
According to the Random Forest model, the top factors affecting the diagnosis are:
1. Worst Area
2. Worst Concave Points
3. Mean Concave Points

## 💻 How to Run
1. Clone the repository.
2. Install dependencies: `pip install pandas scikit-learn seaborn matplotlib`.
3. Run the Jupyter Notebook `task.ipynb`.
