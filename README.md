

# 🚀 Empowering Early Detection of Heart Attack Risks with Machine Learning

## 📌 Project Overview
Heart disease is one of the leading causes of mortality worldwide, primarily due to late detection and delayed medical intervention. This project aims to develop a **machine learning-based prediction model** to assess heart attack risk using patient health records. The goal is to **enable early medical intervention** and **personalized treatment plans**.

## 📊 Dataset Information
- **Source**: Kaggle 
- **Records**: 445,132  
- **Features**: 40 (6 numerical, 34 categorical)  
- **Target Variable**: `HadHeartAttack`  
- **Data Issues**:
  - 157 duplicate rows  
  - Presence of missing values  
  - Imbalanced target distribution  

## 🔍 Exploratory Data Analysis (EDA)
### Univariate Analysis
- Most numeric features are **right-skewed**.
- Presence of **outliers** in numerical columns.
- Majority of data points belong to **Females** and the **White race**.
- Most patients are **aged between 65-69**.

### Bivariate & Multivariate Analysis
- **Imbalance in target variable** observed.
- **Correlation** between `Weight in Kg` and `BMI`.
- **Heatmaps & Pair plots** used for identifying trends and relationships.

## 🛠 Data Preprocessing & Feature Engineering
### Handling Missing Values
- **KNN Imputation** for numerical variables.
- **Logical and Mode Imputation** for categorical variables.
- **BMI calculated** using `Weight(kg)/Height(m)^2`.

### Feature Engineering
- Extracted **Race** and **Ethnicity** from `RaceEthnicityCategory`.
- Created a **Region** feature by grouping states.
- **Encoding**:
  - **Label Encoding**: Binary categorical variables.
  - **Ordinal Encoding**: `General Health` and `LastCheckupTime` (as they have a hierarchy).
  - **One-Hot Encoding**: Other categorical features.

### Data Scaling
- Used `StandardScaler` to normalize numerical features.

### Train-Test Split
- **70:30 ratio** applied for training and testing.

## 🤖 Machine Learning Models Used
- **Baseline Model**: Logistic Regression  
- **Supervised Learning Models**:
  - KNN Classifier  
  - Naïve Bayes Classifier  
  - Decision Tree Classifier  
  - Random Forest  
  - AdaBoost  
  - Gradient Boosting  
  - XGBoost (Best Performing Model)  

## ⚡ Model Tuning & Evaluation
- **Hyperparameter Tuning**:  
  - Applied **Grid Search** for optimizing parameters.  
  - Adjusted **learning rate, tree depth, sample split**, etc.  
- **Performance Metrics**:  
  - **Accuracy**  
  - **Recall**  
  - **Confusion Matrix**  
  - **ROC Curve Analysis**  

## 🎯 Key Findings & Business Impact
- **XGBoost achieved the best accuracy & recall**, making it the optimal model for predicting heart attack risks.  
- Early prediction can **improve patient outcomes**, **reduce medical costs**, and **increase survival rates**.  
- **Addressed challenges** like missing data and class imbalance through **data imputation and under-sampling/class weights**.  

## 📌 Future Scope
- Enhancing model **interpretability** with SHAP values.  
- Deploying the model as a **web application** for real-time predictions.  
- Exploring **deep learning models** for further performance improvement.  

## 🙌 Team Members & Contributions
- **Mentor**: Mr. Ankush Bansal  
- **Team**:
  - Raghavendra S  
  - Baljit Singh Karnavat  
  - Nikhil Vinod   
  - Shashwat Girish Irny  
  - Vergin J  

---

