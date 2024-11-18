# Practical Application 2 - Used Car Prices

- The goal of the application is to analyze the used car dataset and derive factors taht affect the used car prices. This analysis is presented in a report for car dealerships to understand the factors when determining the price of used cars.

- The source of the dats is vehicles.csv that is obtained from kaggle

- The analysis is captured in a jupyter notebook used_car_prices.ipnyb. Following key oobservations and data from the notebook

  - The data contained historical data on used car prices with various factors listed like year, odometer reading, type, condition etc.

  - Price is the dependent variable. The first goal was to understand the key independent variables. The total numnber of variables was large, so using all for data analysis would involve a lot of compute. Also many variables are highly correlated among themselves or are not correlated with the priced variable.

  - The data was first sanitized to focus on the key parameters for model analysis. To perform this, we fist removed non-relevant information like ID and VIN. We also converted other categorical non-numerical data into numerical data using One-Hot Encoding.

  - We fetched the correlation matrix of each parameter with the price column. We also performed RFE regression to determine the top few columns that need to be kept in the dataset.

  - The dataset was split into a training and test dataset and various different regression models were run on it and the mean squared error was determined
    - Lasso Regression
    - Linear regression with Sequential Selector
    - Ridge Regression
    - Linear Regression with Lasso Selector

- The results were captured in a report. The analysis was performed using the CRISP-DM framework


