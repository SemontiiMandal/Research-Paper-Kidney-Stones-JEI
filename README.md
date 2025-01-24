# A machine learning approach to detect renal calculi by studying the physical characteristics of urine

# Project Overview
The Kidney Stone Detection System is a machine learning-based solution designed to predict the presence of kidney stones before symptoms appear. By analyzing urine's physical characteristics, the system leverages supervised learning classifiers to identify potential abnormalities. This project aims to provide a cost-effective and non-invasive early detection method, minimizing reliance on imaging techniques like CT scans.
See full paper - https://emerginginvestigators.org/articles/23-066

#### Tools and Libraries Used
**Programming Language:**
Python

**Libraries and Frameworks:**
Pandas: For data manipulation and preprocessing.
NumPy: For numerical computations.
Scikit-learn: For machine learning models and evaluation.
Logistic Regression: For interpretable baseline modeling.
Decision Tree: For visual decision rules and high-performance classification.
Support Vector Machine (SVM): For non-linear classification and enhanced accuracy.
Matplotlib: For visualization of results.

**Dataset**
Source: The data were obtained from the laboratory of James S. Elliot M.D. of the Urology Section, Veteran's Administration Medical Center, Palo Alto and the Division of Urology, Stanford University School of Medicine, Stanford.
(Credit: Andrews, D.F., Herzberg, A.M. (1985). Physical Characteristics of Urines With and Without Crystals. In: Data. Springer Series in Statistics. Springer, New York, NY. https://doi.org/10.1007/978-1-4612-5098-2_45)

_**Dataset Features:**_
pH Level,
Calcium Concentration,
Urine Specific Gravity,
other relevant physical and chemical characteristics;
The dataset was preprocessed to remove missing values, standardize feature scales, and shuffle for unbiased training and testing.

**Methodology**

**Data Preprocessing:**
Cleaning: Missing values were imputed, and outliers were removed based on domain-specific thresholds.
Scaling: Continuous variables were standardized using StandardScaler to ensure consistency in feature ranges.
Train-Test Split: Data was divided into training and testing sets in an 80:20 ratio for robust evaluation.

**Model Building:**
Three machine learning classifiers were trained:

**Logistic Regression:**
Used as a baseline model.
Hyperparameters: Default settings for simplicity and interpretability.

**Decision Tree:**
Capable of handling non-linear relationships and feature importance visualization.
Hyperparameters: Default for tree depth, ensuring balanced complexity.

**Support Vector Machine (SVM):**
RBF kernel for handling non-linear relationships.
Hyperparameters:
C=1.0: Regularization parameter.
gamma='scale': Adjusts kernel computation sensitivity.

**Model Evaluation:**
Performance Metrics: Accuracy, Precision, Recall, and F1 Score on the test set.
Statistical Validation: One-way ANOVA was conducted to compare model performance and assess significance in classifier differences.

**Key Results**
All classifiers achieved over 80% accuracy and an F1 score above 85%, indicating reliable performance.
Logistic Regression provided interpretable results, while Decision Tree and SVM captured complex patterns for enhanced classification.

**Future Improvements**
Dataset Expansion: Incorporate larger, more diverse datasets to improve generalization.
Deployment: Integrate the solution into a mobile or web application for real-time predictions.
