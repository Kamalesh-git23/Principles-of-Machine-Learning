# Experiment 2: Spam Email Classification using Naïve Bayes

## 📌 Objective
The objective of this experiment is to build and evaluate spam email classification models using different Naïve Bayes algorithms by:
- Performing data exploration and preprocessing
- Visualizing feature distributions and correlations
- Training and evaluating Naïve Bayes classifiers
- Comparing model performance using evaluation metrics

---

## 🛠️ Tools & Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📂 Dataset Description
- **Dataset Used:** `spambase.csv`
- **Target Column:** `class`
  - `0` → Not Spam  
  - `1` → Spam

---

## 📂 File Description
- **Ex2.ipynb** – Jupyter Notebook implementing spam classification using Naïve Bayes models.

---

## 🧪 Experiment Workflow

### 1. Data Loading and Exploration
- Loaded the dataset using Pandas
- Displayed the first few rows
- Checked dataset shape, data types, and summary statistics
- Verified missing values
- Analyzed class distribution (Spam vs Not Spam)

---

### 2. Data Visualization
- Visualized class distribution using count plots
- Plotted feature histograms
- Created box plots for selected important features
- Generated a correlation heatmap for feature relationships

---

### 3. Data Preprocessing
- Separated features (`X`) and target (`y`)
- Split data into training, validation, and testing sets
- Applied feature scaling using `StandardScaler` where required

---

### 4. Model Training
The following Naïve Bayes models were trained:
- Gaussian Naïve Bayes
- Multinomial Naïve Bayes
- Bernoulli Naïve Bayes

Training time for each model was recorded.

---

### 5. Model Evaluation
Each model was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve
- Prediction time

---

## 📊 Output
- Confusion matrices for each classifier
- ROC curves for performance comparison
- Printed evaluation metrics for all models
- Visualization of class distribution and feature behavior

---

## ✅ Learning Outcomes
After completing this experiment, you will be able to:
- Understand spam classification using Naïve Bayes
- Perform exploratory data analysis (EDA)
- Apply different Naïve Bayes algorithms
- Evaluate classification models using multiple metrics
- Compare model performance effectively

---

## ▶️ How to Run

1. Install required libraries:

  - pip install pandas numpy matplotlib seaborn scikit-learn

2. Open Jupyter Notebook:
  - jupyter notebook


3. Open and run Ex2.ipynb cell by cell.

---

## 📌 Conclusion

This experiment demonstrates the effectiveness of Naïve Bayes classifiers for spam detection. By comparing Gaussian, Multinomial, and Bernoulli Naïve Bayes models, the experiment highlights how different assumptions impact classification performance.
