# California Property Close Price Prediction

**Date Started:** June 2026  

## Project Overview
This repository contains the code and documentation for a 12-week Data Science project. The primary objective is to develop a machine learning model to predict the close price (final sales price) of single-family residential properties in California. The predictions are based on historical property characteristics sourced from CRMLS (California Regional Multiple Listing Service).

## Tech Stack
* **Languages:** Python, SQL
* **Data Processing & Analysis:** pandas, NumPy
* **Machine Learning:** scikit-learn (Linear Regression, Decision Trees, Random Forests), XGBoost / LightGBM 
* **Geospatial Analysis:** Spatial joins for geographic feature engineering 
* **Deployment (Planned):** Streamlit 

## Analysis Content & Methodology
The project follows a structured data science lifecycle, progressing from raw data to an interactive prediction application:

* **Data Exploration (EDA):** Analyzing the distributions of the target variable (Close Price) and evaluating key features such as LivingArea, Bedrooms, Bathrooms, and LotSize.
* **Data Preprocessing:** Handling missing values, encoding categorical fields, and normalizing numerical features. The data is split temporally, using the most recent month for testing.
* **Feature Engineering:** Engineering new variables (e.g., bed/bath ratio) and utilizing spatial joins to incorporate granular regional features like the California School District Areas.
* **Model Development:** * Training a baseline Linear Regression model.
  * Expanding to tree-based models including Decision Trees and Random Forests.
  * Implementing and tuning advanced Gradient Boosting models.
* **Evaluation:** Assessing model performance rigorously using $R^{2}$, MAPE, and MdAPE metrics across different price bands.
