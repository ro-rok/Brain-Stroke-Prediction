# Brain Stroke Prediction Data Analysis and Report

## Introduction

- The provided text contains a series of code snippets and outputs related to the analysis of a dataset for predicting the risk of stroke.
- The analysis includes data preprocessing, exploration, and the application of various machine learning models to predict the risk of stroke.
- This report aims to provide a comprehensive summary of the analysis and its findings.

## Data Preprocessing

### Missing Values

- The analysis begins by examining the dataset for missing values.

### Handling Missing Values

- Missing values in the 'bmi' column are a critical concern as BMI (Body Mass Index) is an essential factor in determining the risk of stroke.
- The following steps are taken to address this issue:

### Outliers

- The analysis identifies outliers in the 'bmi' column using the Interquartile Range (IQR) method.

## Data Exploration

### Data Visualization

- Data visualization is a crucial step in data exploration.

### Correlation Analysis

- A correlation matrix is created for the numeric columns in the dataset to understand the relationships between variables.

## Model Building and Evaluation

- The analysis applies various machine learning models to predict the risk of stroke.
- The following models are used:

| Model            | AUC  | Accuracy | F1 Score | Precision | Sensitivity | Specificity |
|------------------|------|----------|----------|-----------|-------------|-------------|
| Decision Tree    | 0.93 | 0.93     | 0.93     | 0.92      | 0.94        | 0.91        |
| SVM              | 0.95 | 0.88     | 0.88     | 0.86      | 0.90        | 0.85        |
| Naive Bayes      | 0.88 | 0.67     | 0.74     | 0.60      | 0.98        | 0.36        |
| Logistic Regression | 0.93 | 0.85 | 0.85 | 0.84 | 0.87 | 0.84 |
| Random Forest    | 0.99 | 0.95     | 0.95     | 0.94      | 0.97        | 0.94        |
| K-NN             | 0.95 | 0.93     | 0.93     | 0.92      | 0.94        | 0.92        |
| LightGBM         | 0.99 | 0.95     | 0.95     | 0.93      | 0.97        | 0.93        |
| XGBoost          | 0.99 | 0.95     | 0.95     | 0.94      | 0.96        | 0.94        |

## Data Transformation and Balancing

- To balance the dataset, Synthetic Minority Over-sampling Technique (SMOTE) is applied.
- The original dataset contains 249 instances with a stroke, and the resampled dataset has 4861 instances with a stroke, ensuring a balanced distribution.

## Conclusion

- The analysis provides valuable insights into predicting the risk of stroke using machine learning models.
- Missing values in the 'bmi' column have been imputed, and outliers have been detected and addressed.
- Various machine learning models have been applied, and their performance has been evaluated.
- The best-performing models are Random Forest, LightGBM, and XGBoost, with high AUC values and balanced accuracy, precision, and sensitivity.
- These models can be considered for further development and deployment to predict stroke risk.
- Additionally, data preprocessing and feature engineering are critical for improving model performance and prediction accuracy.
- It is important to note that this analysis provides a snapshot of the process, and further refinement and optimization may be required for real-world implementation.

