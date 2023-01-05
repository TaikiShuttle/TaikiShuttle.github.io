---
layout: project
type: project
image: images/house_cg.jpg
title: "Predict House Selling Price in Illinois"
# All dates must be YYYY-MM-DD format!
date: 2022.03 - 2022.05
published: true
projecturl: https://github.com/TaikiShuttle/ECE4710J/tree/main/project
labels:
  - Data Science
  - Exploratory data Analysis
  - Machine Learning
summary: "A data model based on exploratory data analysis and machine learning to predict house selling price in Illinois."
---

House price is always a topic drawing people's attention. Purchasing a house with a reasonable price is what people keep seeking for. Thus, it becomes necessary to assess the overall condition of the house and predict a proper price for it. However, it is extremely time consuming to give a ideal selling price by human, for one have to do numerous comparisons between houses and related factors like location and decoration in order to have a rough estimation for the price.

Meanwhile, basic machine learning models like linear regression can take multiple factors into consideration and learn the "rules" from data. It thus becomes feasible to utilize such method in predicting house selling price.

In this project, data from Cook County Assessor’s Office (CCAO) in Illinois will be closely analyzed. The CCAO dataset consists of over 500 thousand records describing houses sold in Cook County in recent years (new records are still coming in every week!). The data set we will be working with has 61 features in total. Based on these features, several data cleaning and feature engineering steps are conducted, followed by a prediction model using machine learning. In general, this project can be divided into two parts.

## Project Part 1: Data Cleaning, EDA, and Feature Engineering

In this part, we try to efficiently explore the data and find some potential factors that have significant impact on the house selling price. Basic data manipulations like log transformation, key words extraction using regular expression, and one hot encoding are adopted. House features like the building area, number of bedrooms, and the neighborhood are inspected for potential relation with the selling price. At last, we combine all these preprocessing steps to a pipeline, which can be universally applied to all the entries of the dataset. 

The Jupyter Notebook file for this part can be found [here](https://github.com/TaikiShuttle/ECE4710J/blob/main/project/Project%20-%20part%201.ipynb).

## Project Part 2: Predicting House Selling Price

In this part, we try to use a Random Forest Regressors with 5-fold validation to fit the model. The fitting result is far more stronger than linear regression as a base line, which is quite satisfying.

The Jupyter Notebook file for this part can be found [here](https://github.com/TaikiShuttle/ECE4710J/blob/main/project/Project%20-%20part2.ipynb).
