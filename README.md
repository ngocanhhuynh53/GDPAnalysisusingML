## Problem Definition
In this notebook, we will create time serie driven forecasting engine based on 3 time series models. The dataset we are using is the 'VIETNAM macroeconomics data'. It is a quarterly dataset starting from 2015 and goes on till April 2024. The target variable is 'Tổng sản phẩm trong nước theo giá so sánh' and there 18 features which can help us forecast. The dataset can be found https://vbma.org.vn/vi/market-data/gdp-industry-group


We will first do exploratory data analysis on the data, we do the following:

1. Load data from CSV
2. Tranform 'quarter' attribute to 'date'
3. Check if any data are missing
4. Create a correlation heatmap
5. Create the time series subplots 

Once the data has been cleaned up, we do:

1. Augmented Dickey-Fuller (ADF) test
2. Differencing to achieve stationarity
3. Exploratory Data Analysis by Autocorrelation Analysis
4. Cluster industry by Kmeans
5. Split dataset to forecast

Finally, we train 3 models:

1. ARIMA (Univariate Time Series)
2. SARIMA (Univariate Time Series)
3. SARIMAX(Multi-variate Time Series)

We make predictions for the 7 quarterly using all the models.
