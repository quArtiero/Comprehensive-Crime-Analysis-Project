# Comprehensive Crime Analysis and Prediction in São Paulo

## Overview

This project analyzes crime data from São Paulo between 2001 and 2021, identifying trends, patterns, and developing predictive models to forecast future crime occurrences. The dataset contains various crime types, police productivity, and crime rates across neighborhoods. The analysis is divided into several steps, including data cleaning, exploratory data analysis, and predictive modeling.

## Table of Contents

- [Introduction](#introduction)
- [Data Collection and Preprocessing](#data-collection-and-preprocessing)
  - [Handle Missing Values and Inconsistencies](#handle-missing-values-and-inconsistencies)
  - [Data Cleaning](#data-cleaning)
  - [Standardize Timestamps and Address Formats](#standardize-timestamps-and-address-formats)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Descriptive Statistics](#descriptive-statistics)
  - [Visualization](#visualization)
- [Predictive Modeling](#predictive-modeling)
  - [Objective](#objective)
  - [Feature Engineering](#feature-engineering)
  - [Model Training and Evaluation](#model-training-and-evaluation)
- [Conclusion](#conclusion)
- [How to Run the Project](#how-to-run-the-project)
- [Contributors](#contributors)
- [License](#license)

## Introduction

This project uses comprehensive crime data from São Paulo to explore historical crime trends and predict future crime occurrences. The analysis focuses on:
- Cleaning and preprocessing the data
- Exploring trends through visualizations
- Building predictive models to forecast crime rates in different neighborhoods

## Data Collection and Preprocessing

### Handle Missing Values and Inconsistencies
Missing values are handled by:
- Removing rows with critical missing data
- Imputing missing values where appropriate

### Data Cleaning
- Duplicate records are removed
- Timestamps are standardized to ensure consistent temporal analysis
- Numerical data (e.g., crime rates) are cleaned to remove inconsistencies such as improper formatting of decimal points

### Standardize Timestamps and Address Formats
- Timestamps across datasets are converted to a consistent format
- Address formats are standardized to improve spatial analysis

## Exploratory Data Analysis (EDA)

### Descriptive Statistics
- Descriptive statistics provide insights into both numerical and categorical data, giving a broad view of crime trends.

### Visualization
- **Temporal Analysis**: Visualizes the number of incidents per year
- **Spatial Analysis**: Examines crime distribution across different neighborhoods
- **Category Analysis**: Analyzes the frequency of different crime types

## Predictive Modeling

### Objective
Two predictive models are developed:
1. Predicting the likelihood of being robbed in a neighborhood
2. Predicting the value of items stolen during robberies

### Feature Engineering
- Features are extracted from timestamps (e.g., year, month) and categorical variables are encoded for modeling
- The target variables for the models are prepared from crime occurrence data

### Model Training and Evaluation
Two machine learning models are trained:
- **Likelihood of Robbery**: A Random Forest Classifier predicts the probability of robbery occurrence in a neighborhood
- **Value of Items Stolen**: A Gradient Boosting Regressor predicts the estimated value of items stolen

## Conclusion

This analysis has provided insights into crime patterns in São Paulo, including:
- **Robbery Trends**: Higher robbery rates were observed in certain regions, and the Random Forest model successfully predicted the likelihood of robbery in these areas.
- **Theft Patterns**: The theft rate model provided moderate accuracy, offering predictive insights into theft incidents.

These models can assist law enforcement and policymakers in making informed decisions to mitigate future crime occurrences, with an emphasis on targeted resource allocation.

## How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/quArtiero/crime-analysis-sao-paulo.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
   Execute the cells in the notebook to perform data analysis and run predictive models.

## Contributors

- Pedro Quartiero (https://github.com/quArtiero)

## License

This project is licensed under the MIT License.
```
