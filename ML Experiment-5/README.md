# Experiment 5: Perceptron vs Multilayer Perceptron with Hyperparameter Tuning

## 📌 Objective
The objective of this experiment is to implement and compare the performance of a **Single-Layer Perceptron Learning Algorithm (PLA)** and a **Multilayer Perceptron (MLP)** for handwritten character recognition by:
- Understanding linear vs nonlinear classifiers
- Implementing PLA from scratch
- Implementing MLP using deep learning techniques
- Performing hyperparameter tuning
- Evaluating and comparing both models using standard metrics

---

## 🛠️ Tools & Technologies Used
- Python  
- Jupyter Notebook  
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  
- TensorFlow / Keras  

---

## 📂 File Description
- **Ex5.ipynb** – Jupyter Notebook containing the complete implementation of PLA and MLP along with evaluation and comparison.

---

## 🧪 Experiment Workflow

### 1. Data Loading and Exploration
- Loaded dataset using `pandas`
- Read image file names and labels from `english.csv`
- Verified dataset size and class distribution
- Ensured correct mapping between images and labels

---

### 2. Data Preprocessing
- Resized images to **28 × 28 pixels**
- Converted images to **grayscale**
- Normalized pixel values to the range **[0, 1]**
- Flattened images into **784-dimensional feature vectors**
- Encoded class labels into numerical values
- Split dataset into **training and testing sets (80:20)**

---

### 3. Perceptron Learning Algorithm (PLA) Implementation
- Implemented PLA from scratch using Python
- Used **step activation function**
- Applied perceptron weight update rule
- Extended PLA to multiclass classification using **One-vs-Rest (OvR)**
- Tracked misclassification rate per epoch as training loss

---

### 4. Multilayer Perceptron (MLP) Implementation
- Implemented MLP using **TensorFlow/Keras**
- Designed input layer with **784 neurons**
- Added hidden layers with nonlinear activation functions
- Used **Softmax** activation in output layer
- Trained model using **backpropagation**
- Used **categorical cross-entropy** as loss function

---

### 5. Hyperparameter Tuning
The following hyperparameters were tuned to improve performance:
- Learning Rate  
- Batch Size  
- Optimizer (SGD, Adam)  
- Activation Function (ReLU, Tanh)  
- Number of Hidden Layers  

Multiple configurations were trained and compared to identify the best-performing model.

---

### 6. Model Evaluation
The models were evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  
- ROC Curves (Micro and Macro Average)  
- Training and Validation Loss vs Epochs Curve  

---

## 📊 Output
- Printed classification metrics for PLA and MLP
- Displayed confusion matrices
- Plotted ROC curves for both models
- Visualized training convergence behavior
- Compared overall performance of PLA and MLP

---

## ✅ Learning Outcomes
After completing this experiment, you will be able to:
- Understand the limitations of linear classifiers
- Implement PLA and MLP models
- Perform hyperparameter tuning in neural networks
- Evaluate classification models using multiple metrics
- Analyze convergence behavior and overfitting

---

## ▶️ How to Run

1. Install required libraries:

   - pip install numpy pandas matplotlib scikit-learn tensorflow

   
2. Open Jupyter Notebook:

    - jupyter notebook

3. Open and run Ex4.ipynb cell by cell.

---

## 📌 Conclusion

This experiment demonstrates that the Multilayer Perceptron significantly outperforms the Single-Layer Perceptron for handwritten character recognition. While PLA is simple and computationally efficient, it fails to capture nonlinear patterns. The MLP, when combined with proper hyperparameter tuning, achieves higher accuracy and stable convergence, making it more suitable for complex image-based classification tasks.
