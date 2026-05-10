---
layout: post
title: Machine Learning
subtitle: Each post has a subtitle
categories: Modules
tags: [Github, Modules, Python, R]
---

## 1. A summary of the learning outcomes of the module
•	Learn about the key paradigms and algorithms in machine learning.

•	Get an understanding of data analytics based on machine learning and using modern programming tools, such as Python or R.

•	Experience how machine learning and data analytics can be used in real-world applications.

•	Acquire the ability to gather and synthesise information from multiple sources to aid in the systematic analysis of complex problems using machine learning tools and algorithms.

•	Articulate the legal, social, ethical, and professional issues faced by machine learning professionals.

•	Understand the applicability and challenges associated with different datasets for the use of machine learning algorithms.

•	Apply and critically appraise machine learning techniques to real-world problems, particularly where technical risk and uncertainty is involved.

•	Systematically develop and implement the skills required to be effective member of a development team in a virtual professional environment, adopting real-life perspectives on team roles

and organisation

## 2.	The artefacts created during the module
### 2.1 Unit 1 – 3: Collaborative Discussion
### Discussion topic
Read the article by Metcalf (2024) and discuss the impact of industry 4.0 and/or Industry 5.0 on the sector in which you are involved or interested.

### Initial post


### 2.2 Unit 2: Seminar Exploratory Data Analysis (EDA) tutorial 
Apply EDA using the dataset Auto-mpg dataset (Unit02_uto-mpg.csv) and answer the following questions.

1.Identify missing values.
#### Python code to answer the question
import pandas as pd
#### Load the dataset
df = pd.read_csv("Unit02_uto-mpg.csv")
#### Replace '?' with NaN for proper missing value detection
df.replace("?", pd.NA, inplace=True)
#### Check for missing values in each column
missing_summary = df.isnull().sum()

print("Missing values per column:")

print(missing_summary)

#### Optionally, display rows with missing values
print("\nRows with missing values:")

print(df[df.isnull().any(axis=1)])

![Boxplot of income](https://raw.githubusercontent.com/Velim73285-Star/Velim73285-Star.GitHub.io/main/assets/images/banners/Missing_values_Per_Variable.PNG)

2.Estimate Skewness and Kurtosis.

#### Python code to answer the question
import pandas as pd

from scipy.stats import skew, kurtosis

#### Load dataset
df = pd.read_csv("Unit02_uto-mpg.csv")
#### Replace '?' with NaN and convert columns to numeric where possible
df.replace("?", pd.NA, inplace=True)

df = df.apply(pd.to_numeric, errors='ignore')

#### Select only numeric columns
numeric_cols = df.select_dtypes(include=['number']).columns

#### Calculate skewness and kurtosis for each numeric column
results = {}

for col in numeric_cols:

    results[col] = {
    
        "Skewness": skew(df[col].dropna()),
        
        "Kurtosis": kurtosis(df[col].dropna())
        
    }

#### Display results
for col, stats in results.items():

    print(f"{col}: Skewness = {stats['Skewness']:.3f}, Kurtosis = {stats['Kurtosis']:.3f}")

![Boxplot of income](https://raw.githubusercontent.com/Velim73285-Star/Velim73285-Star.GitHub.io/main/assets/images/banners/Estimation_of_Skewness_and_Kurtosis.PNG)

#### Key findings 
a.Skewness tells us whether a dataset’s distribution is tilted to one side, while Kurtosis tells us how heavy or light the tails are compared to a normal distribution. Together, they describe the shape of the data beyond just mean and variance.

b.Skewness (asymmetry of distribution)

• Most variables show mild positive skewness (mpg, cylinders, displacement, horsepower, weight, acceleration, origin).  This means their distributions lean slightly to the right, with a longer tail of higher values.

•	Model year has skewness close to 0, indicating a nearly symmetric distribution.

c.	Kurtosis (outlier presence)

•	Negative kurtosis for mpg, cylinders, displacement, weight, model year, origin. These means the variables has a flatter distribution than normal, with fewer extreme outliers.

•	Horsepower and acceleration show positive kurtosis, meaning heavier tails and more extreme values compared to normal.

3.Correlation Heat Map.

#### Python code to answer the question
import pandas as pd

import seaborn as sns

import matplotlib.pyplot as plt

#### Load dataset
df = pd.read_csv("Unit02_uto-mpg.csv")

#### Replace '?' with NaN and convert columns to numeric where possible
df.replace("?", pd.NA, inplace=True)

df = df.apply(pd.to_numeric, errors='ignore')

#### Select only numeric columns
numeric_df = df.select_dtypes(include=['number'])

#### Compute correlation matrix
corr_matrix = numeric_df.corr()

#### Plot heatmap
plt.figure(figsize=(10, 6))

sns.heatmap(corr_matrix, annot=True, cmap="coolwarm", fmt=".2f", linewidths=0.5)

plt.title("Correlation Heatmap - Unit02_uto-mpg Dataset")

plt.show()

![Boxplot of income](https://raw.githubusercontent.com/Velim73285-Star/Velim73285-Star.GitHub.io/main/assets/images/banners/Correlation_Heat_Map.PNG)

#### Key relationships 
MPG (fuel efficiency)

•	Strong negative correlations:

o	Weight (-0.83), Displacement (-0.80), Horsepower (-0.78), Cylinders (-0.78). → This means heavier, larger, and more powerful cars consume more fuel.

•	Positive correlations:

o	Acceleration (0.42), Model year (0.58), Origin (0.56). → Newer models and cars from non-US origins (Europe/Asia) tend to be more fuel-efficient.

Engine and size variables

•	Cylinders and Displacement (0.95) → Larger engines almost always have more cylinders.

•	Displacement and Weight (0.93) → Bigger engines are found in heavier cars.

•	Horsepower and Weight (0.86) → More powerful cars are heavier.

## 3.	What exactly have I learnt and how?
To be completed

### 3.1 What have I learnt from this module?
To be completed

### 3.2 The how part of learning the above
To be completed

## 4.	Professional skills matrix and action plan (PDP)
To be completed

