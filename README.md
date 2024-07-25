# BMI Data Analysis and Obesity Prediction

## Project Overview

This project aims to analyze BMI data to predict obesity. It involves performing exploratory data analysis, feature selection, and model training using various classification algorithms. The dataset is divided into training and testing sets, and the best model is selected based on multiple evaluation metrics.

## Project Structure

- `datasets/`: Contains the dataset used for the analysis.
- `notebooks/`: Jupyter notebooks detailing the analysis and model training steps.
- `results/`: Contains the visualizations and results generated during the analysis.
- `README.md`: This file.

## Data Description

The dataset used in this project is `Bmi-Data-1.csv`. It contains various features related to BMI and a target variable `obese` indicating whether a person is obese.

## Steps Performed

### A. Exploratory Data Analysis (EDA)

1. **Importing Modules**: Import necessary libraries for data analysis and visualization.
2. **Loading Data**: Load the dataset and display the first few rows.
3. **Categorical Variable Analysis**: Analyze the distribution of the target variable `obese`.
4. **Statistical Information**: Generate descriptive statistics for the dataset.
5. **Checking for Missing Values**: Identify any missing values in the dataset.
6. **Bivariate Analysis**: Analyze the relationship between categorical features and the target variable.
7. **Correlation Analysis**: Generate a correlation heatmap to visualize the relationships between features.

### B. Data Splitting

1. Split the data into training (70%) and testing (30%) sets.
2. Standardize the data using `StandardScaler`.

### C. Feature Selection

1. Use `ExtraTreesClassifier` to perform feature selection and identify the top 11 important features.

### D. Model Training and Evaluation

1. Train various classification models including Logistic Regression, Linear Discriminant Analysis, K-Nearest Neighbors, and Random Forest.
2. Evaluate the models using metrics such as Accuracy, Balanced Accuracy, F1-Score, Precision, Recall, MCC, and Specificity.
3. Perform grid search with cross-validation to find the best hyperparameters for each model.
4. Evaluate the best model on the test set and generate ROC and AUC scores.
5. Visualize the confusion matrices and ROC curves for each model.

### E. Oversampling

1. Use SMOTE to handle class imbalance in the training data.
2. Re-train the models on the oversampled data and evaluate their performance.

## Visualizations

- **Class Distribution**: Visualize the distribution of the `obese` class.
- **Categorical Features**: Visualize the categorical features with respect to the target variable.
- **Correlation Heatmap**: Display the correlation between features.
- **Feature Importance**: Bar plot of the top 11 important features.
- **ROC Curves**: ROC curves for each model.
- **Confusion Matrices**: Confusion matrices for each model.

## Results

The results of the analysis and model training are saved in the `results/` directory. This includes:
- Visualizations of the EDA.
- Feature importance plot.
- Confusion matrices.
- ROC curves.

## Conclusion
This project demonstrates a comprehensive approach to analyzing BMI data and predicting obesity using various machine learning models. The use of feature selection, model evaluation, and handling class imbalance are key components of this analysis.
