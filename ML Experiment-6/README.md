# 🌳 Experiment 6: Decision Tree vs Random Forest with Hyperparameter Tuning

---

## 📌 Objective

The objective of this experiment is to implement and compare the performance of a **Decision Tree Classifier** and a **Random Forest Classifier** for breast cancer classification by:

- Understanding single-tree vs ensemble learning models  
- Implementing Decision Tree as a baseline model  
- Implementing Random Forest as an ensemble extension  
- Performing hyperparameter tuning using 5-Fold Cross-Validation  
- Evaluating and comparing both models using standard classification metrics  

---

## 🛠️ Tools & Technologies Used

- Python  
- Jupyter Notebook  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 📂 File Description

- **Ex6.ipynb** – Jupyter Notebook containing the complete implementation of Decision Tree and Random Forest models along with hyperparameter tuning and evaluation.

---

## 📊 Dataset Description

- **Dataset Name:** Wisconsin Diagnostic Breast Cancer Dataset  
- **Source:** UCI Machine Learning Repository  
- **Total Samples:** 569  
- **Features:** 30 numerical attributes  
- **Target Classes:**  
  - Malignant (M)  
  - Benign (B)  

This is a binary classification problem.

---

## 🧪 Experiment Workflow

### 1️⃣ Data Loading and Exploration

- Loaded dataset (`wdbc.data`) using `pandas`
- Assigned appropriate column names
- Encoded class labels (M → 1, B → 0)
- Verified dataset size and class distribution

---

### 2️⃣ Data Preprocessing

- Removed ID column (non-informative feature)
- Separated features and target variable
- Performed **80:20 stratified train-test split**
- Ensured balanced class distribution

*(Note: Scaling was not required since tree-based models are scale-invariant.)*

---

### 3️⃣ Decision Tree Implementation

- Implemented Decision Tree classifier
- Tuned the following hyperparameters:
  - Criterion (Gini, Entropy)
  - Max Depth
  - Min Samples Split
  - Min Samples Leaf
- Applied **5-Fold Stratified Cross-Validation**
- Selected best model based on highest Average F1-score
- Evaluated on test set

---

### 4️⃣ Random Forest Implementation

- Implemented Random Forest classifier
- Tuned hyperparameters:
  - Number of Estimators
  - Max Depth
  - Max Features (sqrt, log2)
  - Bootstrap
- Performed 5-Fold Cross-Validation
- Selected best configuration based on F1-score
- Evaluated on test set

---

### 5️⃣ Hyperparameter Tuning

- Used Stratified 5-Fold Cross-Validation
- Evaluation metrics:
  - Accuracy
  - F1-score
- Selected optimal parameters based on highest average F1-score

---

### 6️⃣ Model Evaluation

Both models were evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  
- ROC Curve  
- AUC Score  

Comparative ROC curves were plotted to analyze performance differences.

---

## 📈 Results Summary

- Decision Tree achieved approximately **94–96% accuracy**
- Random Forest achieved approximately **97–99% accuracy**
- Random Forest demonstrated:
  - Reduced variance
  - Higher AUC
  - Better generalization

---

## 📉 Visualizations Included

- Class Distribution Plot  
- Correlation Heatmap  
- Decision Tree Confusion Matrix  
- Random Forest Confusion Matrix  
- ROC Curve (Individual & Comparison)  

---

## ✅ Learning Outcomes

After completing this experiment, you will be able to:

- Understand overfitting in Decision Trees  
- Analyze variance reduction using ensemble methods  
- Perform hyperparameter tuning using cross-validation  
- Evaluate classification models using multiple metrics  
- Compare baseline and ensemble models effectively  

---

## ▶️ How to Run

1. Install required libraries
  
  - pip install numpy pandas matplotlib seaborn scikit-learn


2. Launch Jupyter Notebook
  - jupyter notebook

3. Open and run
  - Open Ex6.ipynb and execute cells sequentially.

---

## 📌 Conclusion

This experiment demonstrates that the Random Forest Classifier outperforms the Decision Tree Classifier in terms of stability, generalization, and overall predictive performance.

While Decision Trees are simple and interpretable, Random Forest improves performance through ensemble learning, bootstrap aggregation, and feature randomness, resulting in higher accuracy and AUC.