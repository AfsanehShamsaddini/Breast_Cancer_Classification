# ​ Breast Cancer Classification

This repository contains a machine learning pipeline for classifying breast tumors as **Malignant** or **Benign** using clinical features and various classification algorithms.

---

##  Objective
To compare the performance of multiple classifiers and determine the most accurate model for breast cancer detection.

---

##  Dataset
- **Source**: `breast-cancer.csv`
- **Features** include: `radius_mean`, `texture_mean`, `perimeter_mean`, `area_mean`, etc.
- **Target variable**: `diagnosis` (`M` = Malignant, `B` = Benign)

---

##  Exploratory Data Analysis (EDA)
- Diagnosis distribution visualization
- Histograms and boxplots for key features
- Pairplots and correlation heatmap to study relationships among features

---

##  Preprocessing
- Encoding `diagnosis` as `0` (Benign) and `1` (Malignant)
- Dropping the `id` column
- Feature scaling using `StandardScaler` in model pipelines

---

##  Models Evaluated
- Logistic Regression
- Ridge Classifier
- Support Vector Machine (SVM)
- Random Forest Classifier
- Naive Bayes
- K-Nearest Neighbors (KNN) with cross-validation to optimize `k`
- Decision Tree Classifier

---

##  Model Evaluation
- Metrics: Accuracy, Confusion Matrix, Precision, Recall, F1-score (via `classification_report`)
- Visualizations: Confusion matrix heatmaps for each model

---

##  Usage

```bash
git clone https://github.com/AfsanehShamsaddini/Breast_Cancer_Classification.git
cd Breast_Cancer_Classification
# Install dependencies if needed
# Run the notebook:
jupyter notebook Breast_Cancer_Classification.ipynb
