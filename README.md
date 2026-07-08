# Project Overview
Real estate valuation is a critical aspect of the housing market, influencing property sales, investment decisions, taxation, and mortgage lending. Accurately estimating property values is often challenging because house prices are affected by multiple factors, including location, accessibility, property age, and nearby amenities. Traditional valuation methods typically rely on expert appraisals, which can be time-consuming, subjective, and influenced by market fluctuations.

The value of a residential property is determined by several key characteristics, such as the transaction date, house age, distance to the nearest MRT station, number of nearby convenience stores, and geographic location (latitude and longitude). Since the relationship between these features and property prices is complex and nonlinear, conventional statistical methods may not always provide the most accurate predictions.

This project leverages machine learning techniques to predict residential property prices based on historical real estate transaction data from Sindian District, New Taipei City, Taiwan. By developing and evaluating regression models on the UCI Real Estate Valuation dataset, the project demonstrates how data-driven approaches can improve property price estimation, support real estate professionals and investors in decision-making, and provide more consistent and objective property valuations.

## Project Goal
This project is aimed at using supervised machine learning (regression) to predict the unit price of residential real estate using property characteristics, accessibility measures, and geographic location.

## Variables
Target(Output): house price of unit area  
Features (Input): X1 transaction date, X2 house age, X3 distance to the nearest MRT station, X4 number of convenience stores, X5 latitude, X6 longitude

## Data Source
This project uses a publicly available dataset that follows standard academic citation practices.  
Dataset Name: Real Estate Valuation  
Source: UCI Machine Learning Repository  
Authors: I-Cheng Yeh  
Year: 2018  
DOI / Reference: https://doi.org/10.24432/C5J30W

## Methodology
The project follows a structured machine learning workflow:
- Data Overview/collection
- Data Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Feature Analysis
- Model Evaluation
- Model Selection

## Key Findings
* Transaction date does not have strong influence on house price.
* The highest-priced property transaction in the dataset occurred in April 2013, while the majority of property transactions were recorded in May 2013.
* The majority of high-price observations are concentrated in a dense cluster around 121.53–121.55° longitude and 24.97–24.98° latitude. This spatial concentration suggests that houses in this specific area command a price premium due their proximity to the MRT station.
* Prices decrease as house age increases up to about 20–25 years. This pattern suggests that the relationship between House Age and House Price is nonlinear.
* The number of convenience stores exhibits a positive (direct) relationship with house price per unit area. Overall, properties located in areas with more convenience stores tend to have higher prices. However, the considerable variation in house prices at each convenience store count indicates that other factors, such as proximity to MRT stations, house age, and location, also contribute significantly to property values.
* The Random Forest model delivered the best overall performance, achieving the lowest prediction error and the highest coefficient of determination (R²).


## Tech Stack
Programming Language: Python  
Libraries: NumPy, Pandas, Matplotlib, Seaborn  
Machine Learning: Scikit-Learn  
Model Used: Linear Regression, Ridge Regression, Polynomial Regression, Support Vector Machine (SVR), RandomForest, XGBoost  
Environment: Jupyter Notebook

