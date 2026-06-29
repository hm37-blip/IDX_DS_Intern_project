# California Property Close Price Prediction

**Date Started:** June 2026  

## Project Overview
This repository contains the code and documentation for a 12-week Data Science project. [cite_start]The primary objective is to develop a machine learning model to predict the close price (final sales price) of single-family residential properties in California[cite: 5, 13, 14]. [cite_start]The predictions are based on historical property characteristics sourced from CRMLS (California Regional Multiple Listing Service)[cite: 14, 16].

## Tech Stack
* **Languages:** Python, SQL
* **Data Processing & Analysis:** pandas, NumPy
* [cite_start]**Machine Learning:** scikit-learn (Linear Regression, Decision Trees, Random Forests), XGBoost / LightGBM [cite: 63, 68, 83]
* [cite_start]**Geospatial Analysis:** Spatial joins for geographic feature engineering [cite: 76]
* [cite_start]**Deployment (Planned):** Streamlit [cite: 91]

## Analysis Content & Methodology
[cite_start]The project follows a structured data science lifecycle, progressing from raw data to an interactive prediction application[cite: 40]:

* [cite_start]**Data Exploration (EDA):** Analyzing the distributions of the target variable (Close Price) and evaluating key features such as LivingArea, Bedrooms, Bathrooms, and LotSize[cite: 50].
* [cite_start]**Data Preprocessing:** Handling missing values, encoding categorical fields, and normalizing numerical features[cite: 55, 56, 57]. [cite_start]The data is split temporally, using the most recent month for testing[cite: 58].
* [cite_start]**Feature Engineering:** Engineering new variables (e.g., bed/bath ratio) and utilizing spatial joins to incorporate granular regional features like the California School District Areas[cite: 75, 76].
* [cite_start]**Model Development:** * Training a baseline Linear Regression model[cite: 63].
  * [cite_start]Expanding to tree-based models including Decision Trees and Random Forests[cite: 68].
  * [cite_start]Implementing and tuning advanced Gradient Boosting models[cite: 83, 84].
* [cite_start]**Evaluation:** Assessing model performance rigorously using $R^{2}$, MAPE, and MdAPE metrics across different price bands[cite: 88, 89].
