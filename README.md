# 🛒 Online Shoppers Purchasing Intention Prediction

## 📌 Project Overview
In the competitive e-commerce industry, predicting customer purchase behavior is crucial for improving sales and reducing cart abandonment.  
This project builds and evaluates machine learning models to predict whether an online shopper will make a purchase based on their session behavior and browsing attributes.

---

## 🎯 Objective
To develop a predictive machine learning model that determines whether a customer will generate revenue (`Revenue = 1`) based on their browsing behavior, session features, and technical details.

---

## 📊 Dataset
- **Source:** [UCI Machine Learning Repository – Online Shoppers Purchasing Intention Dataset](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset)  
- **Shape:** 12,330 sessions × 18 features  
- **Target Variable:** `Revenue` (1 = Purchase, 0 = No Purchase)  
- **Features include:**  
  - Administrative, Informational, Product-related pages and durations  
  - BounceRates, ExitRates, PageValues, SpecialDay  
  - Month, OperatingSystem, Browser, Region, TrafficType  
  - VisitorType, Weekend  

---

## ⚙️ Methodology
1. **Data Preprocessing**
   - Handled missing values and categorical encoding
   - Feature scaling (StandardScaler)
   - Train-test split

2. **Handling Class Imbalance**
   - Applied **SMOTE (Synthetic Minority Oversampling Technique)**  
   - Compared results before and after balancing

3. **Model Training & Evaluation**
   - Implemented and tuned the following models:
     - Logistic Regression  
     - Decision Tree  
     - K-Nearest Neighbors (KNN)  
     - Random Forest  
     - Gradient Boosting  
     - Naive Bayes  
     - Support Vector Machine (SVM)  
   - Evaluation Metrics: Accuracy, Confusion Matrix, Classification Report (Precision, Recall, F1-score)  
   - Hyperparameter tuning using **GridSearchCV**

4. **Feature Importance Analysis**
   - Identified key predictors using tree-based models  

---

## 🚀 Results
- **Random Forest** achieved the **best performance**:
  - **Best CV Accuracy:** ~87.8%  
  - **Test Accuracy:** ~80.5%  
- **Gradient Boosting** performed closely with ~79.4% test accuracy  
- Important features: **ExitRates, ProductRelated_Duration, Month**  
- Accuracy remained high, but recall for the minority class (purchases) was lower, highlighting the challenge of imbalanced data.

---

## ✅ Conclusion
- **Random Forest** is the most effective model for this dataset.  
- SMOTE improved balance but did not significantly boost overall accuracy.  
- Future work can explore **cost-sensitive learning, advanced ensembles, or hybrid resampling** to better capture purchase cases.  

---

## 🛠️ Technologies Used
- **Python**  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn, Imbalanced-learn  

---

## 📂 Project Structure
