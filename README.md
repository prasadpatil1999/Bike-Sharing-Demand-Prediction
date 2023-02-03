<h1 align="center"> Seoul Bike Sharing Demand Prediction
 </h1>

<h3 align="center"> AlmaBetter Verfied Project - <a href="https://www.almabetter.com/"> AlmaBetter School </a> </h5>

![image](https://user-images.githubusercontent.com/92014177/163593183-d4b01216-3d3a-492c-ba63-8fc93e6eaf4a.png)


<p> </p>

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h2> :floppy_disk: Table of Content</h2>

  * [Introduction](#Introduction)
  * [Abstract](#Abstract)
  * [Dataset Information](#dataset-information)
  * [Problem Statement](#Problem-Statement)
  * [Conclusion](#Conclusion)


![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)


<h2> :book: Introduction:</h2>

* In this dataset, the bikes are rented to the public every hour. 

* As a result, it is important that the rental bike is ready and available to the public at the correct time, as this decreases wait times. Maintaining a consistent supply of rental bikes for the city eventually becomes a major challenge.

* As a result, our main goal is to predict the number of bikes required at each hour in order to maintain a stable supply of rental bikes.

* To do so, we'll need to build a model that will predict numbers of rental bikes at each hour.

* As a result, the dataset consists of various features, some of which will play a major role in predicting the dependent variable, i.e. the number of rental bikes.
 



![image](https://sophiesu.net/wp-content/uploads/2021/01/Bike-Sharing-Demand-1536x644.jpg)




![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)


<h2> :book: Abstract:</h2>

* The goal of this project is to combine the historical bike usage patterns with the weather data to forecast bike rental demand. The data set consists of hourly rental data spanning two years.

* Exploratory Data Analysis is done on the dataset and compares the target variable with the other variables to find the distribution of the graph.

* This information includes information about the host, lodging prices, and reviews, among other things.

* We look for null values which were not found and outliers.

* We also perform correlation analysis to extract out the important and relevant features from the dataset and later perform a train test split to train the model.

* The main objective is to build a predictive model, which could help to train a model to predict the number of bike rentals per hour given the weather conditions.

* This would in turn help to predict quickly and efficiently.



![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)


<h2> :book: Dataset information:</h2>


* Date: year-month-day


* Rented Bike count - Count of bikes rented at each hour


* Hour - Hour of the day


* Temperature-Temperature in Celsius


* Humidity - %


* Wind Speed - m/s


* Visibility - 10m


* Dew point temperature - Celsius


* Solar radiation - MJ/m2


* Rainfall - mm


* Snowfall - cm


* Seasons - Winter, Spring, Summer, Autumn


* Holiday - Holiday/No holiday


* Functional Day - (Non-Functional Day), Fun (Functional Day)



![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h2> :book: Problem Statement:</h2>

With the growing demand and user base for bike-sharing system, providing the city with a stable supply of rental bikes could eventually become a challenging task. The success of bike-sharing system relies in ensuring that the quality of facilities provided, meets the needs and expectations of the users. Therefore, it is important to ensure that rental bikes are available and accessible to the users at right time ,as it reduces the waiting time. Forecasting the number of bikes required and identifying the key factors that influence the demand for rental bikes can greatly help in managing the bike-sharing system.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)



<h1>Rented Bike count - Count of bikes rented at each hour (target variable)</h1>


<h2>🛠️ Tools and Technologies used</h2>

The programming language used in this project is Python . The following libraries were used for data analysis and data visualization and to build a classifier to predict the price range of mobile phones.

Pandas : For loading the dataset and performing data wrangling

Matplotlib: For data visualization.

Seaborn: For data visualization.

NumPy: For some math operations in predictions.

Statsmodels: For statistical computations

Sklearn: For the purpose of analysis,prediction and evaluation.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)


<h2>📑 Steps involved</h2>

Data Preprocessing : Checked for outliers, incorrect values, missing values, duplicates and performed data type correction.

Feature Extraction : Created new columns such as Day, Month, Year, Days_of_week and Weekend from Date column .

Exploratory Data Analysis : Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.

Feature Selection : Checked the VIF value (measure of multicollinearity) and dropped Dew point Temperature and Year which were highly correlated with other independent features.

Feature encoding : The categorical features present in the dataset Seasons, Holiday, Weekend, Functioning Day were dummified.

Feature Scaling : Brought features to a similar range using MinmaxScaler.

Implementation of Regression models

Hyperparameter tuning

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h1>Comparison of models</h1>


<h2>💻 Algorithms used</h2>

Linear Regression

Polynomial Regression

Decision Tree

Random Forest

XGBoost

Gradient Boosting

Stacking

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h1>Conclusion</h1>

<h2>Findings from EDA:</h2>

Temperature and Hour have a strong correlation with the count of rented bikes.

Dew point temperature is highly positively correlated to the Temperature.

Over the weekend and during holidays, rental bike demand decreases.

There is a significant drop in the number of rented bikes during Winters(Dec-Feb) because it's freezing cold!

The demand for bikes increases during warmer temperatures,which is why there's maximum count of rented bikes during the Summer season.

In all seasons,the peak demands for rental bikes occur on the opening (8-9 AM) and closing times (6-7pm) of offices and institutions.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h1>Conclusion Based on Model Evaluation:</h1>

Stacking was found to be most suitable for making predictions of hourly demand for rental bikes.

An adjusted R2 score of 0.91 was obtained.

Temperature and Hour were found to be most influential variables in predicting the hourly demand for rental bikes.

When compared to other models used, decision tree-based models have performed well.

Linear and Polynomial regression models did not perform well in this case, since there is no significant linear correlation between Rented bike count and the independent features.
