# Time Series Forecasting for Furniture Sales

### **Project Overview**
This project involves time series modeling to forecast sales for the **Furniture** product category for the year 2018. The dataset used is a Tableau dataset containing historical sales data for various product categories. 

### **Dataset Information**
- **Dataset Source**: Tableau dataset
- **Total Entries**: 9,994
- **Columns**: 21

### **Key Features in the Dataset**
- **Order Date**: Date when the order was placed
- **Ship Date**: Date when the order was shipped
- **Category**: Product category (Furniture, Office Supplies, Technology)
- **Sales**: Sales amount for each transaction

We filtered the dataset to focus on the **Furniture** category, which exhibits seasonality.

### **Objective**
To forecast sales for the **Furniture** product category for the year 2018 by leveraging historical sales data and identifying trends, seasonality, and other patterns to support business decisions.


## Project Steps
### 1. Data Preparation
- Filtered the dataset to include only rows where `Category = 'Furniture'`.
- Aggregated sales data by month to create a time series.

### 2. Exploratory Data Analysis
- **Trend Analysis**: Observed an overall seasonal pattern in furniture sales.
- **Seasonality Check**: Identified seasonal peaks during specific months.

### 3. Models Used for Forecasting
#### a. **Exponential Smoothing**
- Captures level, trend, and seasonality components.

#### b. **Holt's Linear Trend Model**
- Accounts for linear trends in data over time.

#### c. **Holt-Winters Model** (Best Performing)
- Incorporates level, trend, and seasonal components.
- Produced the best results with the lowest **AIC** and **RMSE**.

#### d. **ARIMA and SARIMA**
- Applied but did not perform as well as the Holt-Winters model.

### 4. Model Evaluation
- **Performance Metrics**: 
  - **AIC**: Akaike Information Criterion
  - **RMSE**: Root Mean Square Error
  ------------------------------------------------------------------------------------------------------------

## Key Insights
- The **Furniture** category exhibits clear seasonality, with noticeable peaks in sales during certain months.
- The **Holt-Winters Model** effectively captured the seasonal patterns and provided the most accurate forecasts.
- ARIMA and SARIMA models struggled to handle the strong seasonality in the dataset compared to exponential smoothing methods.
  

## **Technologies Used**
**Programming Language:**

Python

**Libraries:**

pandas for data manipulation.

numpy for numerical computations.

matplotlib and seaborn for data visualization.

sklearn for machine learning modeling and evaluation.

statsmodels for statistical analysis.

### **Future Work**

- Expand the analysis to include other product categories such as **Office Supplies** and **Technology**.
- Explore advanced machine learning models like Prophet and LSTM for time series forecasting.
- Develop a dashboard to visualize forecasts and provide actionable insights for stakeholders.
- Investigate external factors (e.g., economic indicators, promotions) to improve forecasting accuracy.

### **Contributing**

Contributions are welcome! Please fork the repository and submit a pull request.

