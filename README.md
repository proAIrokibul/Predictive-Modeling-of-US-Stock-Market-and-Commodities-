# Commodity and Stock Market Price Analysis and Prediction

## Project Overview

This project aims to analyze and predict the prices and trading volumes of commodities and stocks using machine learning techniques. By leveraging historical data, we uncover key insights into market trends, trading behaviors, and price dynamics. The analysis includes comprehensive exploratory data analysis (EDA), data preprocessing, and predictive modeling. The goal is to provide actionable insights and accurate predictions to support informed financial decision-making.

## Dataset Description

The dataset includes time-series data for various financial instruments, including commodities like crude oil, natural gas, gold, and silver, alongside stocks of major companies such as Apple, Tesla, and Microsoft. Key features include:

- **Date**: Timestamp of each record.
- **Price Data**: Historical prices for commodities, cryptocurrencies, indices, and stocks.
- **Volume Data**: Trading volumes for the respective assets.

### Example Columns
- **Natural_Gas_Price**, **Natural_Gas_Vol.**
- **Crude_oil_Price**, **Crude_oil_Vol.**
- **Bitcoin_Price**, **Bitcoin_Vol.**
- **Apple_Price**, **Tesla_Price**, and corresponding volumes.

---

## Workflow

### 1. Exploratory Data Analysis (EDA)
We conducted detailed EDA to identify key patterns:
- **Price Trends**: Visualized the price evolution of commodities and stocks over time.
- **Trading Volume Analysis**: Highlighted trading activity levels and their fluctuations.
- **Volatility Analysis**: Examined periods of market stability and instability using rolling standard deviations.
- **Correlation Analysis**: Explored relationships between various assets, providing insights into potential market dependencies.

---

### 2. Data Preprocessing
To ensure data quality and prepare it for modeling, the following steps were performed:
- **Data Cleaning**: Removed invalid characters (e.g., commas) in numerical columns and converted them to the correct format.
- **Missing Value Handling**: Imputed missing data using forward fill and mean imputation.
- **Feature Scaling**: Standardized and scaled the dataset using MinMaxScaler for model compatibility.
- **Feature Engineering**: Created lagged features and rolling averages to enhance predictive capabilities.

---

### 3. Predictive Modeling
Three models were implemented to predict prices and trading volumes:

#### Linear Regression
A baseline model to evaluate linear relationships in the data.  
**Performance Metrics**:
- **MAE**: 0.10  
- **MSE**: 0.02  
- **RMSE**: 0.15  
- **R²**: 0.98  
- **MAPE**: 0.27  

#### Random Forest Regressor
An ensemble model capable of capturing non-linear relationships.  
**Performance Metrics**:
- **MAE**: 0.09  
- **MSE**: 0.02  
- **RMSE**: 0.13  
- **R²**: 0.99  
- **MAPE**: 0.29  

#### XGBoost Regressor
A gradient boosting model optimized for speed and accuracy.  
**Performance Metrics**:
- **MAE**: 0.09  
- **MSE**: 0.02  
- **RMSE**: 0.14  
- **R²**: 0.99  
- **MAPE**: 0.28  

---

### 4. Insights and Findings
- **Linear Regression** provided a reliable baseline with an R² of 0.98, effectively capturing most variance.  
- **Random Forest Regressor** outperformed the other models with the lowest RMSE (0.13), showcasing its ability to model complex relationships.  
- **XGBoost Regressor** delivered a strong balance between performance and computational efficiency, achieving similar accuracy to Random Forest.

---

## Conclusion
This project provides a comprehensive framework for understanding and predicting market behavior for commodities and stocks. The insights generated can guide strategic decision-making, investment planning, and market analysis.
