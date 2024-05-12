# Regression - Yes Bank Stock Closing Price Prediction : Machine learning
<img width="568" alt="Screenshot 2024-05-12 171731" src="https://github.com/keerthan-pu/Regression---Yes-Bank-Stock-Closing-Price-Prediction/assets/114256472/374ee5a2-f38f-4ad3-b731-ccf0913eee74"> <img width="210" alt="Screenshot 2024-05-12 171943" src="https://github.com/keerthan-pu/Regression---Yes-Bank-Stock-Closing-Price-Prediction/assets/114256472/93f754ac-7c99-410b-8f3f-346acf9f013d">


# Business Context
Yes Bank is a well-known bank in the Indian financial domain. Since 2018, it has been in the news because of the fraud case involving Rana Kapoor. Owing to this fact, it was interesting to see how that impacted the stock prices of the company and whether Time series models or any other predictive models can do justice to such situations. This dataset has monthly stock prices of the bank since its inception and includes closing, starting, highest, and lowest stock prices of every month. The main objective is to predict the stock’s closing price of the month.
# Data Description
Dataset link : https://drive.google.com/file/d/1qE-lEu9VDFTQ26ivGoBpg4Ztoe1sek7f/view

![image](https://github.com/keerthan-pu/Regression---Yes-Bank-Stock-Closing-Price-Prediction/assets/114256472/ce92d8e5-f961-46c3-b08e-a6b13175afa6)\

Main Libraries to be Used:

1.Pandas for data manipulation, aggregation

2.Matplotlib and Seaborn for visualisation and behaviour with respect to the target variable

3.NumPy for computationally efficient operations

4.Scikit Learn for model training, model optimization, and metrics calculation.
# Project Architecture
![image](https://github.com/keerthan-pu/Regression---Yes-Bank-Stock-Closing-Price-Prediction/assets/114256472/45657b3f-8a61-44a3-a7ab-712cd10e1797)

# Task performed
1) Data Cleaning :- Dealing with null values, duplicate data and outliers present in our data.

2) Exploratory Data Analysis :- Plotting the dependent variable and distributions of dependent and independent variables. Checking and visualizing the correlation between our dependent and independent variables. Visualizing the relationship between each pair of our variables.

3) Data Preprocessing & Feature Engineering :- Checking for and Dealing with multicollinearity present in our dataset. Applying the log transform to deal with positively skewed data. Scaling the data and splitting it into train and test sets.

4) Model Implementation :- Fitting various models on our data and optimizing them via cross-validation. Using these models to make predictions on test and train data. The Models implemented are :-
Linear Regression,
Lasso Regression,
Ridge Regression and 
Elastic Net Regression

5) Data Visualization :- Using several kinds of charts like Line chart, scatter plot, heatmap, pair plot, distplot, boxplot etc to better visualize data and understand correlation and trends.

6) Model performance comparison :- Comparison of all implemented models using various Regression evaluation metrics like Mean absolute error, Mean squared error, RMSE, R-squared and Adjusted R-squared.

7) Conclusion :- Drawing some insights from the data and the predictions made by our various predictive models on unseen (test) data.

# Insights and Conclusion
Using data visualization on our target variable, we can clearly see the impact of 2018 fraud case involving Rana Kapoor as the stock prices decline dramatically during that period.
After loading the dataset, we found that there are no null values in our dataset nor any duplicate data.
There are some outliers in our features however this being a very small dataset, dropping those instances will lead to loss of information.
We found that the distribution of all our variables is positively skewed. so we performed log transformation on them.
There is a high correlation between the dependent and independent variables. This is a signal that our dependent variable is highly dependent on our features and can be predicted accurately from them.
We found that there is a rather high correlation between our independent variables. This multicollinearity is however unavoidable here as the dataset is very small.
We implemented several models on our dataset in order to be able to predict the closing price and found that all our models are performing remarkably well and Elastic Net regressor is the best performing model with Adjusted R2 score value of 0.9932 and scores well on all evaluation metrics.
All of the implemented models performed quite well on our data giving us the Adjusted R-square of over 99%.
We checked for presence of Heterodasceticity in our dataset by plotting the residuals against the Elastic Net model predicted value and found that there is no Heterodasceticity present. Our model is performing well on all data-points.
With our model making predictions with such high accuracy, we can confidently deploy this model for further predictive tasks using future data.

