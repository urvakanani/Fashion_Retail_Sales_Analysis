# Fashion Retail Sales Analysis

## Introduction
In this project, I analyzed fashion retail sales data to gain insights into customer purchasing behavior, item popularity, and payment method trends. The analysis was performed using Python libraries such as pandas, matplotlib, seaborn, and scikit-learn.

## Objectives
My objectives were to:
- Clean and preprocess the dataset to ensure data quality.
- Perform exploratory data analysis (EDA) to identify patterns and trends.
- Build a regression model to predict purchase amounts based on review ratings and payment methods.
- Provide actionable insights and recommendations for business decisions.

## Dataset Description
The dataset contains the following columns:
1. **Customer Reference ID**: A unique identifier for each customer.
2. **Item Purchased**: Name of the item purchased.
3. **Purchase Amount (USD)**: Amount spent by the customer.
4. **Date Purchase**: Date of purchase.
5. **Review Rating**: Customer rating for the item purchased (scale of 1 to 5).
6. **Payment Method**: Payment method used (e.g., Credit Card, Cash).

## Steps Performed

### 1. Data Cleaning
I cleaned the dataset by:
- Filling missing values in `Review Rating` with the mean value.
- Filling missing values in `Purchase Amount (USD)` with the median value.
- Removing duplicate rows using `.drop_duplicates()`.
- Detecting and treating outliers in `Purchase Amount (USD)` using the Interquartile Range (IQR) method.
- Standardizing categorical columns (`Item Purchased` and `Payment Method`) using `.str.lower()` and `.replace()`.

### 2. Exploratory Data Analysis (EDA)

#### Key Visualizations
1. **Top 10 Items with Highest Average Purchase Amount**:
   - I found that premium items like "raincoat," "sweater," and "blouse" generate higher average purchase amounts.

2. **Correlation Matrix**:
   - There is a weak correlation between `Review Rating` and `Purchase Amount (USD)`, indicating that review ratings do not strongly influence spending behavior.

3. **Box Plot**:
   - Outliers in purchase amounts were successfully removed during data cleaning.

### 3. Regression Modeling

#### Model Setup
I built a linear regression model using scikit-learn to predict `Purchase Amount (USD)` based on:
- Independent Variables: `Review Rating` and `Payment Method_credit_card`.
- Dependent Variable: `Purchase Amount (USD)`.

#### Model Performance
- Mean Squared Error (MSE): 2448.686
- R-squared Value: -0.0057

#### Interpretation
The negative R-squared value indicates that the model performs worse than a simple mean-based prediction, suggesting that these variables are weak predictors of purchase amounts.

## Insights
1. Premium items like "raincoat," "sweater," and "blouse" are high-value products contributing significantly to revenue.
2. Payment methods do not have a significant impact on purchase amounts.
3. Review ratings have little correlation with purchase amounts, indicating that customer satisfaction does not strongly influence spending behavior.

## Recommendations
1. Focus marketing efforts on high-value items like "raincoats," "sweaters," and "blouses" to maximize revenue.
2. Offer discounts or promotions on low-performing items to boost sales.
3. Encourage customers to leave reviews after purchases to improve brand reputation.
4. Collect additional customer data (e.g., demographics, seasonal trends) for better predictive modeling in future analyses.
5. Explore advanced machine learning models (e.g., Random Forests or Gradient Boosting) for more accurate predictions of purchase behavior.

## Files Included
1. `Fashion_Retail_Analysis.ipynb`: Jupyter Notebook containing code for data cleaning, EDA, regression modeling, and visualizations.
2. `Fashion_Retail_Sales.csv`: Original dataset used for analysis.
3. `Cleaned_Fashion_Retail_Sales.csv`: Cleaned dataset after preprocessing.

## How# Fashion Retail Sales Analysis

## Introduction
In this project, I analyzed fashion retail sales data to gain insights into customer purchasing behavior, item popularity, and payment method trends. The analysis was performed using Python libraries such as pandas, matplotlib, seaborn, and scikit-learn.

## Objectives
My objectives were to:
- Clean and preprocess the dataset to ensure data quality.
- Perform exploratory data analysis (EDA) to identify patterns and trends.
- Build a regression model to predict purchase amounts based on review ratings and payment methods.
- Provide actionable insights and recommendations for business decisions.

## Dataset Description
The dataset contains the following columns:
1. **Customer Reference ID**: A unique identifier for each customer.
2. **Item Purchased**: Name of the item purchased.
3. **Purchase Amount (USD)**: Amount spent by the customer.
4. **Date Purchase**: Date of purchase.
5. **Review Rating**: Customer rating for the item purchased (scale of 1 to 5).
6. **Payment Method**: Payment method used (e.g., Credit Card, Cash).

## Steps Performed

### 1. Data Cleaning
I cleaned the dataset by:
- Filling missing values in `Review Rating` with the mean value.
- Filling missing values in `Purchase Amount (USD)` with the median value.
- Removing duplicate rows using `.drop_duplicates()`.
- Detecting and treating outliers in `Purchase Amount (USD)` using the Interquartile Range (IQR) method.
- Standardizing categorical columns (`Item Purchased` and `Payment Method`) using `.str.lower()` and `.replace()`.

### 2. Exploratory Data Analysis (EDA)

#### Key Visualizations
1. **Top 10 Items with Highest Average Purchase Amount**:
   - I found that premium items like "raincoat," "sweater," and "blouse" generate higher average purchase amounts.

2. **Correlation Matrix**:
   - There is a weak correlation between `Review Rating` and `Purchase Amount (USD)`, indicating that review ratings do not strongly influence spending behavior.

3. **Box Plot**:
   - Outliers in purchase amounts were successfully removed during data cleaning.

### 3. Regression Modeling

#### Model Setup
I built a linear regression model using scikit-learn to predict `Purchase Amount (USD)` based on:
- Independent Variables: `Review Rating` and `Payment Method_credit_card`.
- Dependent Variable: `Purchase Amount (USD)`.

#### Model Performance
- Mean Squared Error (MSE): 2448.686
- R-squared Value: -0.0057

#### Interpretation
The negative R-squared value indicates that the model performs worse than a simple mean-based prediction, suggesting that these variables are weak predictors of purchase amounts.

## Insights
1. Premium items like "raincoat," "sweater," and "blouse" are high-value products contributing significantly to revenue.
2. Payment methods do not have a significant impact on purchase amounts.
3. Review ratings have little correlation with purchase amounts, indicating that customer satisfaction does not strongly influence spending behavior.

## Recommendations
1. Focus marketing efforts on high-value items like "raincoats," "sweaters," and "blouses" to maximize revenue.
2. Offer discounts or promotions on low-performing items to boost sales.
3. Encourage customers to leave reviews after purchases to improve brand reputation.
4. Collect additional customer data (e.g., demographics, seasonal trends) for better predictive modeling in future analyses.
5. Explore advanced machine learning models (e.g., Random Forests or Gradient Boosting) for more accurate predictions of purchase behavior.

## Files Included
1. `Fashion_Retail_Analysis.ipynb`: Jupyter Notebook containing code for data cleaning, EDA, regression modeling, and visualizations.
2. `Fashion_Retail_Sales.csv`: Original dataset used for analysis.
3. `Cleaned_Fashion_Retail_Sales.csv`: Cleaned dataset after preprocessing.



