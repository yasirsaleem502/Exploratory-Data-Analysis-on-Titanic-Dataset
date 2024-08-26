
# Exploratory Data Analysis on Titanic Dataset

![Titanic](https://img.shields.io/badge/dataset-Titanic-blue)
![Python](https://img.shields.io/badge/Python-3.8+-green)
![Jupyter Notebook](https://img.shields.io/badge/Tools-Jupyter%20Notebook-orange)
![Pandas](https://img.shields.io/badge/Library-Pandas-yellow)
![Seaborn](https://img.shields.io/badge/Library-Seaborn-lightblue)

## Project Overview

This project performs an in-depth Exploratory Data Analysis (EDA) on the famous Titanic dataset. The goal is to uncover insights about the passengers on the Titanic, the factors that influenced survival rates, and the relationships between different features. The analysis lays the foundation for building predictive models to predict passenger survival.

## Table of Contents

- [Introduction](#introduction)
- [Dataset Description](#dataset-description)
- [Data Cleaning](#data-cleaning)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Conclusions](#conclusions)
- [How to Run](#how-to-run)
- [Dependencies](#dependencies)
- [License](#license)

## Introduction

The sinking of the Titanic is one of the most infamous shipwrecks in history. In this project, we analyze the dataset of passengers aboard the Titanic to understand the factors that led to survival. This analysis involves data cleaning, feature engineering, and extensive visualizations to extract meaningful insights.

## Dataset Description

The dataset consists of 891 entries with 12 features:

- **PassengerId**: Unique ID for each passenger
- **Survived**: Survival (0 = No, 1 = Yes)
- **Pclass**: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- **Name**: Name of the passenger
- **Sex**: Gender of the passenger
- **Age**: Age of the passenger
- **SibSp**: Number of siblings or spouses aboard the Titanic
- **Parch**: Number of parents or children aboard the Titanic
- **Ticket**: Ticket number
- **Fare**: Passenger fare
- **Cabin**: Cabin number
- **Embarked**: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Data Cleaning

The dataset required significant cleaning due to missing values and inconsistencies. Key steps included:

- **Handling Missing Values**: Imputation of missing values in the `Age`, `Embarked`, and `Cabin` columns.
- **Feature Transformation**: Created new features like `FamilySize` and `IsAlone` to better understand the impact of family presence on survival.
- **Outlier Detection**: Identified and handled outliers in the `Fare` and `Age` columns.

## Exploratory Data Analysis

The EDA phase involved analyzing the distribution of data, relationships between features, and key trends affecting survival. Major insights included:

- **Survival by Class**: Passengers in 1st class had a higher survival rate compared to those in 3rd class.
- **Gender Impact**: Females had a significantly higher survival rate than males.
- **Age Distribution**: Younger passengers, especially children, had a higher chance of survival.
- **Embarked Port**: Passengers who embarked at Cherbourg had a higher survival rate.

## Feature Engineering

To enhance the predictive power of the dataset, additional features were engineered:

- **FamilySize**: Combined `SibSp` and `Parch` to reflect the total family size.
- **IsAlone**: A binary feature indicating if a passenger was alone (FamilySize = 1).
- **Title**: Extracted titles from passenger names to understand social status and its impact on survival.

## Conclusions

The EDA provided critical insights into the Titanic dataset, revealing that survival rates were influenced by factors such as class, gender, age, and family presence. These insights will guide the development of predictive models in subsequent steps.

## How to Run

To run the analysis on your local machine:

1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/titanic-eda.git
    ```
2. Navigate to the project directory:
    ```bash
    cd titanic-eda
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```
4. Open the Jupyter Notebook:
    ```bash
    jupyter notebook Titanic_EDA.ipynb
    ```

## Dependencies

- Python 3.8+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

To install the dependencies, run:
```bash
pip install pandas numpy matplotlib seaborn jupyter





