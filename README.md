![banner](assets/banner.png)
![Python version](https://img.shields.io/badge/Python%20version-3.10.8-B06FCF)
![GitHub last commit (branch)](https://img.shields.io/github/last-commit/Aliya032/flight-price-prediction/main?color=FFDA15)
![GitHub Repo Size](https://img.shields.io/github/repo-size/Aliya032/flight-price-prediction?color=D95353)
![Tyep of ML](https://img.shields.io/badge/Type%20of%20ML-Random%20Forest%20Regression-blue)
[![Static Badge](https://img.shields.io/badge/Open_In_Heroku-o?logo=heroku&logoColor=%23430098&labelColor=%23ffffff)](https://predict-flight-price-a54f89e1be13.herokuapp.com/predict)



## Table of Contents:
- [Problem Statement](#business-problem)
- [Data Source](#data-source)
- [Methods](#methods)
- [Tech Stack](#tech-stack)
- [Quick Glance At The Results](#quick-glance-at-the-results)
- [Limitations & What Can Be Improved](#limitations-and-what-can-be-improved)
- [Explore The Notebook](#explore-the-notebook)
- [Deployment On Heroku](#deployment-on-heroku)
- [App Deployed On Heorku](#app-deployed-on-heroku)


## Problem Statement
This project's objective is to enhance travel planning by forecasting ticket prices for upcoming flights. By leveraging a random forest regression model, it assists travelers in making informed decisions by identifying the most cost-effective flights and optimal travel times. The model is constructed using Kaggle-sourced data.

Predictions about flight prices are generated using a set of key features. These include airline type, arrival and departure times, flight duration, source and destination locations, among others. Through the analysis of these factors, the model provides insights into flight pricing patterns, aiding travelers in planning their journeys effectively. 

## Data Source
- Kaggle Flight Fare Prediction(https://www.kaggle.com/datasets/nikhilmittal/flight-fare-prediction-mh)

## Methods

- Exploratory Data Analysis
- Data Visualization 
- Feature Engineering 
- One Hot Encoding 
- Hyperparameter Tuning
- Pickling
- Model Deployment 


## Tech Stack

- Python *(Refer to requirements.txt for the packages used in this project)*
- Heroku *(for deployment)*

## Quick Glance At The Results

**Information about the dataset:**

![Info](assets/InfoTrainSet.png)

**Price vs Airline:**

![Price Vs Airline](assets/PriceVsAirline.png)
*Inference:* Jet Airways has the most outliers in terms of price.

**Price vs Destination:**

![Price vs Destination](assets/DestinationVsPrice.png)
*Inference:* New Delhi has the most outliers and Kolkata has the least. 

**Months vs Number of flights:**

![Months vs Number of flights](assets/CountOfFlightsMonthsWise.png)
*Inference:* May has the most number of flights

**Type of Airline vs Number of Flights**

![Airline vs Number of Flights](assets/AirlineVsNoOfFlights.png)
*Inference:* Jet Airways has the most flight boarded

**Correlation between all features:**

![Correlation Heatmap](assets/CorrelationHeatmap.png)

**Feature Importance:**

![Feature Importance](assets/FeatureImportance.png)

From the above figure, we can see that the total stops and duration of the flight are the most useful in predicting the target variable, the price. 

When then built the model and obtained the following results before and after the hyperparameter tuning: 

|  | MAE | MSE | RMSE |
|:---:|:---:|:---:|:---:|
| Before Hyperparameter Tuning | 1171.53 | 4357560.02 | 2087.47 |
| After Hyperparameter Tuning | 1163.22 | 4043245.02 | 2010.78 |


## Limitations & What Can Be Improved

1. **Data Timeframe:** This project relies on pre-pandemic data, which might not accurately reflect current market dynamics. Incorporating real-time data spanning more than 7 years could yield more precise predictions. Additionally, including factors like fuel prices and global events (e.g., conflicts, pandemics, economic recessions) could enrich the model's predictive capabilities.

2. **Data Enrichment:** Gathering data through web scraping via tools like Selenium from diverse airline websites can provide a more comprehensive and up-to-date dataset. This could enhance the accuracy of predictions by capturing a broader range of flight prices.

3. **Algorithm Diversification:** Exploring multiple machine learning algorithms beyond the current random forest regression model could lead to more refined predictions. By testing different algorithms, the project's predictive accuracy might be further improved.

4. **Enhanced User Experience:** The front-end design of the application could be enhanced to provide users with a more intuitive and user-friendly interface. A visually appealing and user-centric design can enhance the project's overall usability.

5. **Model Interpretability:** Improving the interpretability of the model's predictions can empower users with insights into how different features influence flight prices. This could help travelers make more informed decisions based on their preferences.


## Explore The Notebook


## App Deployed On Heroku 

![Demo GIF](assets/working-demo.gif)

## Further Readings
🔗 [How Airlines Price Their Flights](https://www.alternativeairlines.com/blog/how-airlines-price-flights)

🔗 [Why are flights so expensive right now?](https://thriftytraveler.com/guides/travel/why-are-flights-so-expensive-right-now/)

🔗 [Google Flights](https://thriftytraveler.com/guides/google-flights/)

🔗 [Airfare Prediction Tools](https://www.wired.com/story/airfare-prediction-tools/)

🔗 [Flight Price Predictor Tools and Apps
](https://techpp.com/2014/05/05/airfare-price-predictor/)





<!-- https://www.vectorlogo.zone/logos/heroku/heroku-icon.svg -->