# 🌳 Experiment 7: Bagging, Boosting, and Stacked Ensemble Models

---

## 📌 Objective

The objective of this experiment is to implement and compare different **ensemble learning techniques** for breast cancer classification by:

- Understanding Bagging, Boosting, and Stacking methods  
- Implementing Bagging using Decision Trees  
- Implementing Boosting algorithms (AdaBoost and Gradient Boosting)  
- Building a Stacked Ensemble model using multiple base learners  
- Performing hyperparameter tuning using 5-Fold Cross-Validation  
- Evaluating and comparing ensemble models using standard metrics  

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

- **Ex7.ipynb** – Jupyter Notebook containing implementation of Bagging, Boosting, and Stacking models along with hyperparameter tuning and evaluation.

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
- Verified dataset structure and class distribution  

---

### 2️⃣ Data Preprocessing

- Removed ID column (non-informative feature)  
- Separated features and target variable  
- Performed **80:20 stratified train-test split**  
- Maintained class balance  

---

### 3️⃣ Bagging Implementation

- Implemented **Bagging Classifier** using Decision Tree as base estimator  
- Tuned hyperparameters:
  - Number of estimators  
  - Max samples  
  - Max features  
- Applied **5-Fold Cross-Validation**  
- Evaluated model on test data  

---

### 4️⃣ Boosting Implementation

- Implemented:
  - **AdaBoost Classifier**
  - **Gradient Boosting Classifier**  
- Tuned hyperparameters:
  - Number of estimators  
  - Learning rate  
  - Max depth (for Gradient Boosting)  
- Used 5-Fold Cross-Validation  
- Evaluated performance on test set  

---

### 5️⃣ Stacked Ensemble Implementation

- Built **Stacking Classifier** using:
  - Base Models: Decision Tree + KNN  
  - Meta Learner: Logistic Regression  
- Tuned meta-learner parameters:
  - Regularization parameter (C)  
  - Solver type  
- Evaluated using cross-validation and test set  

---

### 6️⃣ Hyperparameter Tuning

- Used **GridSearchCV with 5-Fold Cross-Validation**  
- Evaluation metrics:
  - Accuracy  
  - F1-score  
- Selected best models based on highest performance  

---

### 7️⃣ Model Evaluation

All models were evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  
- ROC Curve  
- AUC Score  

---

## 📈 Results Summary

- **AdaBoost achieved the best performance (~98.25% accuracy)**  
- **Bagging performed strongly (~97.37% accuracy)**  
- **Gradient Boosting achieved ~96.49% accuracy**  
- **Stacking achieved ~92–93% accuracy**  

### Key Insights:
- Bagging reduced variance effectively  
- Boosting reduced bias and improved prediction  
- Stacking performance depends on model diversity  

---

## 📉 Visualizations Included

- Class Distribution Plot  
- Correlation Heatmap  
- Confusion Matrices (Bagging, AdaBoost, Gradient Boosting, Stacking)  
- ROC Curve Comparison  

---

## ✅ Learning Outcomes

After completing this experiment, you will be able to:

- Understand ensemble learning techniques  
- Analyze bias vs variance trade-off  
- Implement Bagging, Boosting, and Stacking models  
- Perform hyperparameter tuning using cross-validation  
- Evaluate and compare multiple models effectively  

---

## ▶️ How to Run

1. Install required libraries
  - pip install numpy pandas matplotlib seaborn scikit-learn


2. Launch Jupyter Notebook
  - jupyter notebook

3. Open and run
  - Open Ex7.ipynb and execute all cells sequentially.

## 📌 Conclusion

This experiment demonstrates that ensemble learning significantly improves model performance compared to individual models.

AdaBoost performed the best, achieving the highest accuracy and F1-score by effectively reducing bias through sequential learning.
Bagging also performed well, reducing variance and improving stability.
Gradient Boosting showed strong performance, while Stacking achieved comparatively lower accuracy due to limited diversity among base models.

Overall, ensemble methods provide better generalization, robustness, and predictive performance in classification tasks.