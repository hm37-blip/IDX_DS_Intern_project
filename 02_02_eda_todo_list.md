# 📈 Exploratory Data Analysis (EDA) todo——list

## 1. Univariate Analysis

### 🎯 Target Variable

Analyze the distribution of the target variable (`close_price`).

- [ ] Plot a histogram of **Close Price**
- [ ] Examine the distribution (normal vs. skewed)
- [ ] Determine whether a **log transformation** is necessary

### 🏠 Numerical Features

Inspect the distributions of the primary numerical features.

Features:

- LivingArea
- BedroomsTotal
- BathroomsTotalInteger
- LotSizeSquareFeet

Tasks:

- [ ] Plot a histogram for each feature
- [ ] Identify skewness and long-tail distributions
- [ ] Check for unreasonable values (e.g., negative or zero)

### 📉 Residual Analysis

- [ ] Check residual distribution
- [ ] Verify whether residuals are approximately uniformly/randomly distributed

---

# 2. Multivariate Analysis

## 🔥 Correlation Analysis

Evaluate relationships among numerical variables.

Tasks:

- [ ] Compute the correlation matrix
- [ ] Visualize correlations using a **Heatmap**
- [ ] Identify highly correlated features (possible multicollinearity)

---

## 📊 Feature Distribution

For each numerical variable:

- [ ] Plot a histogram
- [ ] Compare distributions across variables
- [ ] Identify potential feature engineering opportunities

---

# 3. Data Quality Check

## 🧩 Missing Values

Evaluate data completeness.

Tasks:

- [ ] Count missing values for every column
- [ ] Calculate the percentage of missing values
- [ ] Remove columns with extremely high missing rates
- [ ] Plan imputation strategies for columns with low missing rates

---

## 🚨 Outlier Detection

Detect abnormal or unrealistic observations.

Tasks:

- [ ] Visualize distributions using histograms and boxplots
- [ ] Identify impossible or suspicious records

Examples:

- Property with **0 bedrooms** but **5,000 sq ft** living area
- Property sold for **$10**
- Negative lot size
- Extremely large living area compared with similar homes

Potential actions:

- Remove obvious data errors
- Cap extreme values (Winsorization)
- Apply log transformation if appropriate
