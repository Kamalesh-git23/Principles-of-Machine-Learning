# 🧪 Experiment 9: Clustering Human Activity Recognition Data

## 📌 Objective
This experiment focuses on applying and comparing different clustering algorithms on the Human Activity Recognition (HAR) dataset:
- K-Means Clustering
- DBSCAN (Density-Based Clustering)
- Hierarchical Agglomerative Clustering (HAC)

The goal is to analyze clustering performance, visualize clusters, and evaluate results using multiple metrics.

---

## 📊 Dataset Description

- **Dataset**: Human Activity Recognition Using Smartphones  
- **Source**: UCI Machine Learning Repository  
- **Samples**: 10,299  
- **Features**: 561  
- **Activities**:  
  - WALKING  
  - WALKING_UPSTAIRS  
  - WALKING_DOWNSTAIRS  
  - SITTING  
  - STANDING  
  - LAYING  

- **Sensors Used**:
  - 3-axis Accelerometer
  - Gyroscope (50 Hz)

---

## ⚙️ Preprocessing Steps

- Merged training and testing datasets  
- Assigned feature names  
- Converted numeric labels to activity names  
- Checked for missing values (none found)  
- Standardized features using `StandardScaler`  
- Applied PCA and t-SNE for visualization  

---

## 🔍 Exploratory Data Analysis

- Feature distribution visualization  
- PCA (linear dimensionality reduction)  
- t-SNE (non-linear visualization)  

---

## 🤖 Clustering Algorithms

### 🔹 K-Means Clustering
- Used Elbow Method (WCSS) and Silhouette Score  
- Optimal clusters chosen: **k = 6**  
- Produced well-separated and interpretable clusters  

### 🔹 DBSCAN
- Parameters: `eps`, `min_samples`  
- Detected noise points successfully  
- Struggled with high-dimensional data  

### 🔹 Hierarchical Clustering (HAC)
- Used Ward linkage  
- Generated dendrogram  
- Produced compact clusters similar to K-Means  

---

## 📈 Evaluation Metrics

### Internal Metrics
- Silhouette Score  
- Davies–Bouldin Index  
- Calinski–Harabasz Index  

### External Metrics
- Adjusted Rand Index (ARI)  
- Normalized Mutual Information (NMI)  

---

## 📊 Visualizations

- Feature Distribution  
- PCA & t-SNE plots  
- Elbow Curve  
- Silhouette Curve  
- K-Means Clusters  
- DBSCAN Clusters  
- Hierarchical Clusters  
- Dendrogram  
- Metrics Comparison  

---

## 📌 Observations

- K-Means produced the most meaningful clusters  
- K-Means is sensitive to the choice of k  
- DBSCAN detected noise but struggled with clustering  
- Ward linkage performed best in hierarchical clustering  
- Silhouette Score aligned well with visual cluster quality  

---

## 🚀 Technologies Used

- Python  
- NumPy, Pandas  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## 📁 Output

All generated visualizations are saved in the `images/` directory.

---


## ▶️ How to Run

1. Install required libraries
    - pip install numpy pandas matplotlib seaborn scikit-learn

2. Launch Jupyter Notebook
    - jupyter notebook

3. Open and run
    - Open Ex9.ipynb and execute all cells sequentially


## 📌 Conclusion

This experiment demonstrates that clustering performance depends heavily on data structure and algorithm choice.

- K-Means performed best due to compact and well-separated clusters  
- Hierarchical clustering also produced good results but is computationally expensive  
- DBSCAN struggled due to high-dimensional feature space  

Dimensionality reduction techniques such as PCA and t-SNE helped in visualizing cluster separation.

Overall, clustering effectiveness depends on parameter tuning and dataset characteristics.