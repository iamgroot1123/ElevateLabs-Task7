# Task 7: Support Vector Machines (SVM)

This repository contains the seventh task of my internship at **Elevate Labs**, focused on implementing **Support Vector Machines (SVM)** for binary classification using both linear and RBF kernels.

## 📌 Objective

The objective of this task was to apply SVMs to a binary classification problem, understand the impact of different kernels (linear and RBF), tune hyperparameters, and evaluate performance using cross-validation.

## 🛠️ Tools Used

- Python  
- Scikit-learn  
- NumPy  
- Matplotlib  

## 🔍 Steps Performed

1. **Dataset**  
   Used the Breast Cancer Wisconsin dataset to classify tumors as malignant or benign based on various cell features.

2. **Preprocessing**  
   - Dropped irrelevant columns (`id`, `Unnamed: 32`)  
   - Converted categorical labels in the `diagnosis` column into binary numerical values (Malignant = 1, Benign = 0)  
   - Split the dataset into features (X) and labels (y)  
   - Performed feature scaling using `StandardScaler`  
   - Split the data into training and test sets (80:20)

3. **Model Training**  
   - Trained an SVM with a **linear kernel** and evaluated performance  
   - Trained an SVM with an **RBF kernel** and evaluated performance  
   - Compared the performance of both kernels  

4. **Model Evaluation**  
   - Evaluated models using:
     - Accuracy Score  
     - Confusion Matrix  
     - Classification Report  
     - Cross-validation (Stratified K-Fold)  

5. **Hyperparameter Tuning**  
   - Used `GridSearchCV` to find the optimal values for `C` and `gamma` for the RBF kernel

6. **Visualization**  
   - Applied PCA to reduce the dataset to 2D and plotted decision boundaries for both kernels

## 📁 Files

- `task7.ipynb` – Jupyter Notebook containing all implementations  
- `Breast_Cancer_Wisconsin.csv` – Original dataset  
- `README.md` – Documentation for this task

## 📊 Dataset

Dataset: Breast Cancer Wisconsin Dataset (569 entries, 30 numerical features, binary target: diagnosis)

## 📈 Evaluation Metrics

- **Accuracy Score**  
- **Confusion Matrix**  
- **Classification Report**  
- **Cross-validation**  
- **GridSearchCV Scores**
