# Income Prediction using Machine Learning

This repository contains a machine learning project that predicts whether an individual earns more than $50k per year based on several demographic and employment features.

## Project Overview
The prediction of income level is a classic binary classification problem. This project utilizes the **Adult Census Income dataset**, often referred to as the "Adult" or "UCI Census" dataset. It includes features such as age, workclass, education, marital status, occupation, relationship, race, sex, and more.

## Dataset
The dataset used is `adult.csv`. It contains approximately 32,561 entries and 15 columns:
- **Target Variable**: `income` (<=50K or >50K)
- **Features**: Age, Workclass, Education, Marital Status, Occupation, Relationship, Race, Sex, Capital Gain, Capital Loss, Hours per week, and Native Country.

## Implementation Details

### 1. Data Preprocessing
- **Missing Values**: Handled records containing '?' by replacing them with NaN and dropping them to ensure data quality.
- **Categorical Encoding**: Used `LabelEncoder` from Scikit-Learn to convert categorical text data into numerical format for model compatibility.
- **Feature Scaling**: Implemented `StandardScaler` to normalize numerical features where necessary.

### 2. Exploratory Data Analysis (EDA)
- Visualized data distribution using histograms for all features to understand underlying patterns and correlations.

### 3. Machine Learning Models
The following classifiers were implemented and compared:
- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Gaussian Naive Bayes**
- **Support Vector Classifier (SVC)**

### 4. Evaluation Metrics
Models were evaluated using:
- Accuracy Score
- Confusion Matrix
- ROC Curve and AUC (Area Under the Curve)

## Requirements
To run this notebook, you will need the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Usage
1. Clone the repository.
2. Ensure you have the `adult.csv` file in the same directory or update the path in the notebook.
3. Run the Jupyter Notebook `Income_prediction_model_ML.ipynb`.

## Results
The project compares the accuracy of each model to determine the best approach for census-based income prediction. Detailed performance metrics and visualizations can be found within the notebook cells.
