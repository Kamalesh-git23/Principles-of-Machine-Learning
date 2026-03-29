# 📊 Experiment 8: Effect of PCA on Regression and Classification Models

---

## 📌 Objective

The objective of this experiment is to study the impact of **Principal Component Analysis (PCA)** on machine learning models by:

- Understanding dimensionality reduction using PCA  
- Training models with and without PCA  
- Comparing model performance using 5-Fold Cross-Validation  
- Evaluating the effect of PCA on regression and classification tasks  
- Analyzing when PCA improves model performance  

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

- **Ex8.ipynb** – Jupyter Notebook containing PCA implementation, regression and classification models, and performance comparison  

---

## 📊 Dataset Description

- **Dataset Name:** PCA Full Lab Dataset (1000 Samples)  
- **Features:** Academic and performance-related attributes  
- **Regression Target:** Final_Score_Regression  
- **Classification Target:** Performance_Level_Classification  

This dataset contains student academic performance data and includes both regression and classification tasks.

---

## 🧪 Experiment Workflow

### 1️⃣ Data Loading and Exploration

- Loaded dataset using `pandas`  
- Checked dataset shape, columns, and data types  
- Analyzed target distributions  
- Verified missing values  

---

### 2️⃣ Data Preprocessing

- Handled missing values using mean imputation  
- Encoded classification target using Label Encoding  
- Separated features and target variables  
- Standardized features using `StandardScaler` (important for PCA)  

---

### 3️⃣ PCA Implementation

- Applied PCA on standardized features  
- Generated Scree Plot  
- Computed explained variance ratio  
- Selected number of components to retain **95% variance**  
- Transformed dataset into reduced feature space  

---

### 4️⃣ Regression Models

- Implemented:
  - Linear Regression  
  - Random Forest Regressor  

- Evaluated using:
  - Mean Squared Error (MSE)  
  - R² Score  

- Compared performance:
  - With PCA  
  - Without PCA  

---

### 5️⃣ Classification Models

- Implemented:
  - Logistic Regression  
  - Support Vector Machine (SVM)  

- Evaluated using:
  - Accuracy  
  - F1-score  

- Compared performance:
  - With PCA  
  - Without PCA  

---

### 6️⃣ Model Evaluation

All models were evaluated using **5-Fold Cross-Validation** to ensure reliable and unbiased results.

---

## 📈 Results Summary

### 🔹 Regression Models

- **Linear Regression slightly improved with PCA**
- **Random Forest also showed slight improvement**

### 🔹 Classification Models

- **Logistic Regression improved with PCA**
- **SVM performance decreased after PCA**

---

## 📉 Visualizations Included

- Scree Plot  
- Cumulative Explained Variance Plot  
- MSE Comparison (Regression)  
- R² Score Comparison (Regression)  
- Accuracy Comparison (Classification)  
- F1-score Comparison (Classification)  

---

## ✅ Learning Outcomes

After completing this experiment, you will be able to:

- Understand PCA and dimensionality reduction  
- Analyze the effect of PCA on different models  
- Identify when PCA is useful  
- Compare model performance using cross-validation  
- Understand trade-offs between performance and interpretability  

---

## ▶️ How to Run

1. Install required libraries
    - pip install numpy pandas matplotlib seaborn scikit-learn

2. Launch Jupyter Notebook
    - jupyter notebook

3. Open and run
    - Open Ex8.ipynb and execute all cells sequentially

## 📌 Conclusion

This experiment demonstrates that PCA can improve model performance by reducing dimensionality, noise, and multicollinearity.

Linear models such as Logistic Regression benefit more from PCA
Random Forest showed slight improvement
SVM performance decreased due to possible loss of important feature information
PCA is most useful when features are highly correlated

Overall, PCA helps improve generalization and model stability but introduces a trade-off between interpretability and performance.