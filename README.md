# Car Accident Analysis
<img width="971" height="1217" alt="image" src="https://github.com/user-attachments/assets/56d0ebbd-f5b1-438a-a360-888a9e2c7a0a" />

## Project Overview
This project was developed as part of a **Data Science Bootcamp**. It aims to analyze road accident data and predict accident severity using machine learning. The project explores how different factors, such as weather conditions, road types, speed limits, and time of day, relate to accident severity.

The CatBoost classification algorithm is used to build a predictive model.

## Dataset
The project uses the **Road Accident Dataset** available on Kaggle.

Dataset Link: https://www.kaggle.com/datasets/nextmillionaire/car-accident-dataset

The dataset includes information about road accidents, such as:
- Accident severity
- Weather conditions
- Road and surface conditions
- Speed limits
- Vehicle types
- Number of vehicles and casualties
- Accident time

## Tools and Libraries
The project was developed using Python in Jupyter Notebook.

The main libraries include:
- **Pandas and NumPy:** Data manipulation and analysis.
- **Matplotlib and Seaborn:** Data visualization.
- **SciPy:** Statistical analysis.
- **Scikit-learn:** Data splitting and model evaluation.
- **CatBoost:** Accident severity classification.
- **KaggleHub:** Dataset downloading.

## Project Implementation

### 1. Data Inspection
The dataset is loaded and examined to understand its structure, data types, statistical information, and missing values.

### 2. Missing Data Analysis and Cleaning
Missing values are analyzed using percentages, visualizations, and statistical tests to investigate missingness patterns.

The `Carriageway_Hazards` column is removed because of excessive missing values. Missing categorical values are filled using the most frequent value, and inconsistent severity labels are corrected.

### 3. Exploratory Data Analysis (EDA)
Different visualizations are created to explore accident patterns and relationships between accident severity and other factors.

The analysis includes weather conditions, road types, vehicle types, speed limits, road surface conditions, and accident time.

### 4. Feature Engineering
New features are created to improve data representation:
- **Hour:** Extracted from the accident time.
- **Rush_Category:** Identifies rush and non-rush hours.
- **Is_Rush_Hour:** Binary indicator for rush hours.
- **Weather_Binary:** Classifies weather conditions as good or bad.

### 5. Data Splitting
The dataset is divided into:
- **80% Training Data**
- **20% Testing Data**

Stratified sampling is used to maintain the accident severity class distribution.

### 6. Model Training
A CatBoost classifier is trained to predict accident severity.

The model handles categorical features and uses automatic class weighting to address class imbalance.

### 7. Model Evaluation
The model's performance is evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### 8. Feature Importance
Feature importance analysis is performed to identify which variables contribute most to the model's predictions.

The top 10 important features are displayed using a bar chart.

## Conclusion
This project demonstrates how data science and machine learning can be applied to road accident analysis. Developed as part of a Data Science Bootcamp, it combines data preprocessing, exploratory analysis, feature engineering, and CatBoost classification to investigate factors associated with accident severity and build a predictive model.# DataScienceBootcamp
