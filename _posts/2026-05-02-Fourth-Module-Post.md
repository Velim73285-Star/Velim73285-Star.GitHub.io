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

1.	Identify missing values.
   
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



## 3.	What exactly have I learnt and how?
To be completed

### 3.1 What have I learnt from this module?
To be completed

### 3.2 The how part of learning the above
To be completed

## 4.	Professional skills matrix and action plan (PDP)
To be completed

