# 🛒 Online Shoppers Purchasing Intention - Python ML Project

This project explores and builds a machine learning pipeline to predict whether an online shopper will generate revenue (make a purchase) based on their session behavior. The dataset used is the **Online Shoppers Purchasing Intention Dataset** from the UCI Machine Learning Repository.

---

##  Dataset Overview

The dataset contains session-level information for online shopping, including:

- Page visit durations (Administrative, Informational, ProductRelated)
- Bounce and Exit rates
- Month and Weekend indicators
- VisitorType and SpecialDay info
- Target: `Revenue` (whether the visitor generated revenue)

📁 Dataset Source: [UCI ML Repository](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset)

---

##  Project Workflow

### ✅ 1. Data Preprocessing
- Loaded and explored the dataset
- Identified data types and handled missing values (if any)

### ✅ 2. Outlier Detection and Handling
- Implemented a reusable Python **class** using the **IQR method**
- Outliers were detected and handled using **capping**

### ✅ 3. Encoding Categorical Variables
- Boolean columns (`Weekend`, `Revenue`) were converted to binary (0/1)
- One-hot encoding applied to `Month` and `VisitorType`

### ✅ 4. Feature Scaling
- Used `StandardScaler` to normalize numerical features

### ✅ 5. Train-Test Split
- Data was split into training and testing sets (80/20) using `train_test_split`
- Stratified split used to maintain class balance in the target variable

###  ✅ 6. Model Training
Implemented and tuned the following machine learning models:

* Logistic Regression

* Decision Tree

* K-Nearest Neighbors (KNN)

* Random Forest

* Gradient Boosting

* Naive Bayes

* Support Vector Machine (SVM)

## 📊 Evaluation Metrics
Used the following metrics to assess model performance:

* Accuracy

* Confusion Matrix

 * Classification Report

## 🔍 Feature Importance Analysis
Identified top predictors for tree-based models using feature_importances_.

## ⚙️ Hyperparameter Tuning
Optimized parameters using GridSearchCV to improve accuracy and generalization.





