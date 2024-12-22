# *Phishing URL Detector by FETI Group*
# IF3070 Foundations of Artificial Intelligence | Tugas Besar 2

## **Group Information**
- **Group Number:** 16  
- **Group Members:**
  - **Thalita Zahra Sutejo (18222023)**  
  - **Irfan Musthofa (18222056)**  
  - **Eleanor Cordelia (18222059)**  
  - **Muhammad Faiz Atharrahman (18222063)**  

---

## **Project Overview**

Phishing attacks have become a significant threat in the digital era, targeting individuals and organizations by mimicking legitimate websites to steal sensitive data. To combat this, machine learning offers robust solutions for identifying and classifying phishing URLs based on patterns, behaviors, and characteristics of the URLs.

This project focuses on implementing and evaluating **Phishing URL Detection** using **K-Nearest Neighbors (KNN)** and **Gaussian Naive-Bayes** classifiers. The goal is to compare the accuracy and efficiency of custom-built algorithms (*from scratch*) with well-established implementations in *scikit-learn*. This process also incorporates critical steps like data preprocessing, missing value handling, and feature engineering to ensure optimal model performance.

---

## **Project Requirements**
### **1. K-Nearest Neighbors (KNN)**
- **Custom Implementation:**
  - Accepts **two parameters**:
    1. Number of neighbors (*k*)
    2. Distance metric (**Euclidean**, **Manhattan**, or **Minkowski**)
  - Efficiently computes distances and predicts the class label based on majority voting among neighbors.
- **Scikit-Learn Implementation:**  
  - Use *scikit-learn*'s **KNeighborsClassifier** to replicate and evaluate the results.

### **2. Gaussian Naive-Bayes**
- **Custom Implementation:**
  - Utilizes probability theory to calculate posterior probabilities for classification.
  - Handles continuous features by assuming a **Gaussian (Normal) distribution**.
- **Scikit-Learn Implementation:**  
  - Use *scikit-learn*'s **GaussianNB** for comparison.

---

## **Process Workflow**

### **1. Data Preprocessing**
- Validate and clean the data to ensure consistency:
  - Convert data types where necessary (e.g., categorical to numeric).
  - Handle missing values with appropriate techniques, such as mean, median, or group-based imputation.
- Engineer relevant features:
  - Extract **TLD**, **Domain**, **Character Ratios**, **Obfuscation Flags**, etc., based on domain-specific knowledge.

### **2. Model Implementation**
- Implement **KNN** and **Gaussian Naive-Bayes** from scratch, ensuring:
  - Proper handling of parameters like distance metrics and data distributions.
  - Efficient computation to handle large datasets.
- Save and load models for reproducibility using formats like .pkl or `.txt`.

### **3. Evaluation**
- Train models using the processed dataset and validate them on unseen data.
- Compare the **accuracy**, **confusion matrix**, and **classification report** of:
  1. Scratch implementations.
  2. Scikit-learn implementations.
- Analyze differences and evaluate the effectiveness of custom algorithms versus library solutions.

---

## **How to Run the Project**
1. **Preprocessing Data:**  
   - Run the data cleaning and preprocessing pipeline provided in the script.
2. **Training Models:**  
   - Train both custom and scikit-learn implementations of KNN and Gaussian Naive-Bayes.
3. **Evaluation:**  
   - Evaluate the models and view metrics such as accuracy, precision, recall, and F1-score.
4. **Saving & Loading Models:**  
   - Save trained models and reload them for predictions.

---

## **Conclusion**
This project demonstrates the application of machine learning for phishing URL detection by exploring the nuances of model implementation, preprocessing, and evaluation. By comparing custom-built and scikit-learn implementations, this study offers valuable insights into the strengths and weaknesses of different approaches for detecting phishing URLs.
