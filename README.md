# 🧠 Quantum-Enhanced Heart Disease Prediction

## 📌 Project Overview

This project presents a comparative study of **classical** and **quantum-enhanced machine learning algorithms** for the **binary classification** of heart disease using the well-known **Cleveland Heart Disease dataset** from the UCI Machine Learning Repository.

The core objective is to evaluate whether **quantum machine learning (QML)** techniques can offer superior or comparable predictive performance to traditional algorithms for medical diagnosis, especially in the early detection of cardiovascular conditions.

We implement six different models — three classical, two quantum-native, and one hybrid ensemble — to investigate performance variations across methodologies.

---

## ⚙️ Models Implemented

### 🧪 Classical Machine Learning Models:

* **Support Vector Machine (SVM)** – A supervised learning algorithm effective in high-dimensional spaces.
* **Artificial Neural Network (ANN)** – A classical multi-layer perceptron (MLP) trained using backpropagation.

### 🔬 Quantum Machine Learning Models:

* **Quantum Support Vector Classifier (QSVC)** – Leverages quantum kernels with a ZFeatureMap and evaluates inner products on a simulated quantum backend.
* **Quantum Neural Network (QNN)** – A parameterized quantum circuit trained to predict class labels using a parity-based interpretation.
* **Variational Quantum Classifier (VQC)** – Utilizes a variational form and quantum feature map to optimize the classification boundary.

### 🧩 Hybrid Model:

* **Bagging-QSVC** – A quantum-enhanced ensemble classifier built by bootstrapping multiple QSVC models using scikit-learn’s BaggingClassifier, enhancing stability and accuracy.

---

## 📊 Dataset Description

* **Source**: [UCI Machine Learning Repository – Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+Disease)

* **Total Attributes**: 13 features, including medical indicators such as:

  * `cp` (chest pain type)
  * `thal` (thalassemia)
  * `ca` (number of major vessels colored by fluoroscopy)
  * `exang` (exercise-induced angina)
  * `slope` (slope of the ST segment)

* **Target**: `target`
  Binary classification —

  * `0`: No heart disease
  * `1`: Presence of heart disease

* **Preprocessing**:

  * Feature selection using Recursive Feature Elimination (RFE)
  * Scaling via MinMaxScaler or StandardScaler
  * Dimensionality reduction using PCA (for QNN and VQC models)

---

## 🧪 Experimental Results

The table below summarizes the classification accuracy of each model tested on the dataset:

|                                   **Model** | **Accuracy** |
| ------------------------------------------: | -----------: |
|                Support Vector Machine (SVM) |       85.24% |
|             Artificial Neural Network (ANN) |       85.24% |
|                          Quantum SVM (QSVC) |       88.52% |
|                Quantum Neural Network (QNN) |       87.00% |
|        Variational Quantum Classifier (VQC) |       86.89% |
| **Bagging Ensemble of QSVC (Bagging-QSVC)** |   **90.16%** |

✅ The **Bagging-QSVC** model outperformed all others, demonstrating the potential of ensemble quantum methods in binary medical classification tasks.

---

##  GitHub Portfolio
📁 Heart-Disease-Quantum-ML
├── 📄 README.md
├── 📄 requirements.txt
├── 📁 data
│   └── Cleveland Dataset.csv
├── 📁 models
│   ├── SVM.py
│   ├── ANN.py
│   ├── QSVC.py
│   ├── QNN.py
│   ├── VQC.py
│   └── Bagging_QSVC.py
├── 📁 notebooks
│   └── QSVC_SVM_QNN_ANN_VQC_BaggingQSVC.ipynb
└── 📁 outputs
    ├── confusion_matrices/
    ├── roc_curves/
    └── accuracy_reports/

📁 Heart-Disease-Quantum-ML
├── 📄 README.md
├── 📄 requirements.txt
├── 📁 data
│   └── Cleveland Dataset.csv
├── 📁 models
│   ├── SVM.py
│   ├── ANN.py
│   ├── QSVC.py
│   ├── QNN.py
│   ├── VQC.py
│   └── Bagging_QSVC.py
├── 📁 notebooks
│   └── QSVC_SVM_QNN_ANN_VQC_BaggingQSVC.ipynb
└── 📁 outputs
    ├── confusion_matrices/
    ├── roc_curves/
    └── accuracy_reports/
