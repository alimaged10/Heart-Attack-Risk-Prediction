# Heart Attack Risk Prediction using Machine Learning

## Overview

This project aims to predict the risk of heart attacks among patients using various machine learning algorithms. By leveraging a comprehensive dataset of health and lifestyle factors, we develop predictive models that can help healthcare providers assess and mitigate heart attack risks more effectively.

## Project Structure

- **data**: Contains the dataset used for training and testing the models.
- **notebook**: Jupyter notebook for data preprocessing, exploratory data analysis (EDA), model training, and evaluation.
- **report**: Project report and related documentation.

## Dataset

The dataset consists of 8763 records from global patients, including features such as age, gender, cholesterol levels, blood pressure, smoking status, and more. The target variable is binary, indicating the presence (1) or absence (0) of heart attack risk.

## Data Preprocessing

1. **Initial Checks and Cleaning**: Ensured no missing data across all features.
2. **Feature Engineering**: Transformed "Blood Pressure" into systolic/diastolic ratio.
3. **Handling Class Imbalance**: Applied SMOTE (Synthetic Minority Over-sampling Technique) to balance classes.
4. **Categorical Encoding**: Encoded categorical features using LabelEncoder.
5. **Correlation Analysis**: Dropped highly correlated geographical attributes to reduce multicollinearity.
6. **Dimensionality Reduction**: Applied PCA (Principal Component Analysis) to retain 90% variance.
7. **Normalization**: Standardized numeric features using StandardScaler.

## Models and Algorithms

We employed three different machine learning algorithms to build the predictive models:

1. **Random Forest Classifier**: An ensemble learning method that constructs multiple decision trees and outputs the mode of the classes or mean prediction of the individual trees.
2. **AdaBoost Classifier**: Combines multiple weak classifiers to create a strong classifier, focusing more on misclassified instances iteratively.
3. **Support Vector Classifier (SVC)**: Finds the hyperplane that best separates the classes using kernel functions like RBF and sigmoid.

## Model Evaluation

The models were evaluated using various metrics:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**
- **AUC-ROC Curve**

### Results

- **Random Forest**: Accuracy: 0.58, F1-Score (Class 0): 0.70, F1-Score (Class 1): 0.32
- **SVM**: Accuracy: 0.64, F1-Score (Class 0): 0.78, F1-Score (Class 1): 0.28
- **AdaBoost**: Accuracy: 0.50, F1-Score (Class 0): 0.56, F1-Score (Class 1): 0.41

## Future Work

To enhance the model performance, future work will focus on:

1. **Advanced Feature Engineering**: To reduce feature overlap and improve class distinction.
2. **Exploring Alternative Models**: Including neural networks and advanced ensembles like XGBoost.
3. **Dimensionality Reduction Techniques**: Using techniques like t-SNE or UMAP.
4. **Expanding the Dataset**: To capture a more comprehensive range of data patterns.

## Project Submitted by 3rd year SBME2025 students:

- [Mina Adel](https://github.com/Mina-A-Tayeh)
- [Hazem Zakaria](https://github.com/hazemzakariasaad)
- [Mariem Magdy](https://github.com/MariemMagdi)
- [Ali Maged](https://github.com/alimaged10)
