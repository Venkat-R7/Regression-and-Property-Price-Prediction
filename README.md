# Regression-and-Property-Price-Prediction


## Introduction

Property price prediction is a very important area of research given the significance of real estate to a nation’s economy and how much people are invested in buying a dream house in terms of money and time. The cost of a property is influenced by a number of factors, for instance the neighbourhood it is situated in, house size, and age of the property. These factors along with range of other factors contribute to the varying trend of housing prices, which has led to numerous research on house price prediction.
This research focuses on the analysis of Ireland's residential property price register data, which includes location-specific information on every residential property sold in the last decade. Traditional and advanced regression techniques were applied to predict the price of a property based of various attributes. This work applied several machine learning techniques like Multiple linear regression, Random Forest, Lasso Regression and Gradient boosting regression methods. Deep learning methods have shown promising results in varies fields in recent year. In this study a deep connected Artificial Neural Network (ANN) was applied. This research focusses on finding the optimal solution from the above-mentioned regression techniques in designing a model which could be used in predicting property prices.
The results show that the Random Forest regression model performed best compared to other regression techniques and predicts Irish property prices with the lowest error rate. The Random Forest model was able to predict the property price with an average absolute error of 0.16 units in a standardised form. Furthermore, by visualising the data using different graphs and plots along with a Geographical Information map yielded many valuable details which will serve to aid in decision making for Irish real estate market consumers.


## Dataset used for study

The Irish Residential Property Price Register dataset was used in this study and was sourced from the Property Service Regulatory Authority (PSRA) of Ireland. The residential property register information is a compilation of details individuals provided to the appropriate revenue commissioners as part of the stamp duty collection for the registration of properties in various counties of Ireland from 2010. The PSRA also has data on the commercial lease registry, however the information is far more limited and only includes the cost and location of the commercial premises. Therefore, only residential property registry data was considered for analysis and price prediction in this study.

The data includes information about property sales for the period from January 2010 to June 2022, totalling more than 540,000 records. There were nine variables in the dataset, including Date of Sale, Price, Address, and County. In addition, the size of the property was also available which is divided into four separate categories in square meter units. The description of the property specifies whether it is a new, second hand or restored house. For the second hand and restored house the time period information of how old the property is, is not available.


## Data cleaning and Pre-processing
1. Data Cleaning
2. Handling of categorical variables 
	One-hot encoding technique
3. Feature extraction of datetime variables
	Details deduced: year, month, day of the week, and whether the sale occurred at the beginning of the year or the quarter
	Cyclic encoding is a methodology
4. Missing values
	Random Forest classifier model was used to handle missing data using available data points
5. Outlier detection and handling
	IQR methodology was used to handle outliers
6. Transforming data for Normality
	Square root transformation was applied on the data to reduce the right skewness

## Regression Methodologies 
1. Multiple Linear Regression 
2. Random Forest Regression
3. Gradient Boosting Regression 
4. Lasso Regression 
5. Artificial Neural Network 


## Evaluation metrics for regression analysis
1. Root Mean Squared Error
2. Mean Absolute Error
3. Mean Absolute Percentage Error


## Data analysis and Insights

## Baseline regression model results

As the initial step in regression model development to predict property price, baseline models were developed. The error metrics for each of the five models are shown in Table. The same results are displayed graphically in Figure. The evaluation metrics RMSE, MAE and MAPE are used to compare the models.

![](Images/results_baseline.jpg)

From the results it can be observed that the Random Forest model performs better than all the other model with the lowest RMSE, MAE and MAPE values of 0.1679, 0.13 and 0.2345 respectively. The RMSE value indicates the overall average distance between the actual values and the predicted values, thus in a normalised dataset, on average a predicted value will
deviate by 0.1679 units from the actual value when using the RF model. The MAPE value indicates the error in terms of percentage, with 0.2345 the average absolute percentage error. Therefore, the predicted value deviate from the actual value by 23.5%. The RF model performance can be classified as good, since a MAPE value less 25% is considered an acceptable regression model for prediction.