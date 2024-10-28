# Loan Prediction Model

This project demonstrates a machine learning pipeline for predicting loan approval status using a [Support Vector Machine (SVM)](https://en.wikipedia.org/wiki/Support_vector_machine) classifier. The dataset used in this project is assumed to be a CSV file containing various features related to loan applications.

## Project Overview

The goal of this project is to predict whether a loan will be approved or not based on several features such as applicant's education, marital status, and property area. The model is trained using a linear kernel SVM, and the dataset is preprocessed to handle missing values and categorical data.

## Steps Involved

1. **Data Loading and Exploration**:
   - The dataset is loaded using [Pandas](https://pandas.pydata.org/) and initial exploration is performed to understand its structure and contents.
   - The shape of the dataset, summary statistics, and missing values are examined.

2. **Data Cleaning**:
   - Missing values are removed from the dataset.
   - The target variable `Loan_Status` is encoded to binary values (1 for 'Y' and 0 for 'N').

3. **Data Transformation**:
   - Categorical variables such as `Dependents`, `Married`, `Gender`, `Self_Employed`, `Property_Area`, and `Education` are encoded into numerical values.
   - The `Dependents` feature is transformed to replace '3+' with 4.

4. **Data Visualization**:
   - [Seaborn](https://seaborn.pydata.org/) is used to create count plots to visualize the distribution of `Loan_Status` across different categories of `Education` and `Married`.

5. **Feature Scaling**:
   - Features are standardized using `StandardScaler` to ensure they have a mean of 0 and a standard deviation of 1.

6. **Model Training and Evaluation**:
   - The dataset is split into training and testing sets with a 90-10 split.
   - A Support Vector Machine (SVM) with a linear kernel is trained on the training data.
   - The model's accuracy is evaluated on both the training and testing datasets.

## Results

The model achieves an accuracy of approximately 80.79% on the training data and 81.25% on the testing data, indicating a good generalization performance.

## Dependencies

- [Python 3.x](https://www.python.org/)
- [NumPy](https://numpy.org/)
- [Pandas](https://pandas.pydata.org/)
- [Seaborn](https://seaborn.pydata.org/)
- [Scikit-learn](https://scikit-learn.org/stable/)

## Usage

To run this project, ensure you have the necessary dependencies installed and execute the script in a Python environment. The dataset should be available at the specified path in the script.

This project serves as a basic example of building a machine learning model for classification tasks, with a focus on data preprocessing and model evaluation.
        
