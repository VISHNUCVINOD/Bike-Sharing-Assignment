# Bike-Sharing-Assignment
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free.Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.
A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic.So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.
In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19.
They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:
Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.
# Business Goal:
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.
## Table of Contents
1. Data Reading and Understanding data
    - Data Clearning
    - Dropping Columns
    -  Change few numerical variables to catergorical variable type
2. Data Visualization
3. Data Preparation
    - Create Dummy variables
    - Splitting data into train and test data
    - Rescaling the Features
4. Model building and evaluation
    - RFE - Recursive feature elimination
    - Model 1
    - Model 2
    - Model 3
    - Model 4
    - Residual Analysis
    - Model Summary

## General Information
- day.csv file is the dataset used in this project
- Analysis has been done using the day dataset.After cleaning the dataset the data was visualized for finding the corelations in numerical and categorical variables. Dummy variables where created for the categorical variables and different model was build using automated and manual approach to arrive at a possible conclusion.
- Provided solution / conclusion for the business problem where the factor contributing to the change in the count of bike rentals was found.

## Conclusions

- Found top features contributing significantly towards explaining the demand of the shared bikes

## Technologies Used

    import numpy as np
    import pandas as pd
    import matplotlib.pyplot as plt
    import seaborn as sns

    import sklearn
    from sklearn.model_selection import train_test_split
    from sklearn.preprocessing import MinMaxScaler
    from sklearn.feature_selection import RFE
    from sklearn.linear_model import LinearRegression

    import statsmodels.api as sm
    from statsmodels.stats.outliers_influence import variance_inflation_factor

    from sklearn.metrics import r2_score
    import warnings


## Contact
Created by [vishnucvinod@gmail.com] - feel free to contact me!
