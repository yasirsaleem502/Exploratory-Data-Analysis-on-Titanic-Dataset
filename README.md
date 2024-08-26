# Exploratory-Data-Analysis-on-Titanic-Dataset
The Titanic dataset is a classic problem often used in data science and machine learning projects to explore data and practice predictive modelling techniques. The dataset provides information on the passengers aboard the RMS Titanic, which sank on April 15, 1912. The primary objective of this case study was to perform an in-depth Exploratory Data Analysis (EDA) to understand the underlying patterns, relationships, and trends in the data. This EDA laid the groundwork for building predictive models and extracting valuable insights .

# Project Duration: 1 week

# Tools & Technologies: Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook

# Objective
The main objectives of this EDA were to:

Understand the distribution of various features such as age, gender, and class of passengers.
Identify correlations between different features and the survival rate.
Detect and handle missing data.
Visualize data to uncover trends and patterns.
Prepare the data for further machine learning tasks.

# Steps Involved

Data Collection :
The Titanic dataset was sourced from the Kaggle repository, which includes two CSV files: train.csv and test.csv. The train.csv was used for the EDA.
Data Understanding. The dataset contains 891 entries and 12 features, including categorical variables (e.g., Sex, Embarked), numerical variables (e.g., Age, Fare), and a target variable (Survived).
Data Cleaning

Handling Missing Values:
The Age column had approximately 20% missing values, which were imputed using the median age grouped by Pclass and Sex.
The Embarked column had two missing values, filled with the most common port of embarkation ('S').
The Cabin column had many missing values, so it was analyzed separately and later excluded from the initial analysis due to its sparsity.

Feature Engineering:
I created new features such as FamilySize (combining SibSp and Parch) and IsAlone (based on FamilySize) to capture the influence of family presence on survival.
Extracted titles from the Name column to analyze their impact on survival.

Univariate Analysis
Survival Rate:
Calculated the overall survival rate, which was around 38%.
Categorical Features: Analyzed the distribution of passengers by Pclass, Sex, and Embarked.
Numerical Features: Explored the distribution of Age, Fare, and FamilySize.
Bivariate Analysis

Survival by Class: Found that passengers in Pclass 1 had a significantly higher survival rate compared to those in Pclass 3.
Survival by Gender: Identified that females had a much higher survival rate (approximately 74%) compared to males (around 19%).
Survival by Age: Visualized age distribution with a focus on survival; children had a higher chance of survival.
Multivariate Analysis

Heatmap of Correlations: Created a heatmap to identify correlations between numerical features. Strong correlations were observed between Pclass and Fare, as well as FamilySize and IsAlone.
Pair Plot: Plotted pairwise relationships between features like Age, Fare, and Survived.
Data Visualization

Bar Plots: Visualized categorical data to compare survival rates across different groups.
Box Plots: Used to observe the distribution of Fare across classes and its impact on survival.
Histograms: Plotted for numerical features to understand their distribution.
Violin Plots: Used to visualize the distribution of age and fare across classes and gender.
Insights & Recommendations

Key Findings:
Wealthier passengers (higher class) and females were more likely to survive.
The survival rate varied significantly with age, with younger children having a better chance of survival.
Passengers traveling alone were less likely to survive.




