# Flight-Price-Prediction

## Project Overview
This project is about building models to predict flight prices based on various features, using the Flight Price Prediction dataset from Kaggle. The models were trained and evaluated on various features including airlines, flight number, departure time, stops, arrival time, class, duration, and days left for the flight.

The results obtained from the models were as follows:

	Model            	MAE	         MSE	        R2 Score
	Linear Regression	4580.820538	 46480151.13	0.909097
  Random Forest	    1069.553350	 7433253.57	  0.985463
	Linear SVM	      4951.540023	 65052444.78	0.872775
	Gradient Boosting	2910.739788	 24000176.98	0.953062
	XGBoost	          2291.345928	 16060929.54	0.968589


This notebook presents an extensive exploratory data analysis of the "Flight Price Prediction" dataset available on Kaggle (https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction/code?resource=download).
The dataset consists of multiple features related to flight details, including the airline, flight number, source city, departure time, number of stops, arrival time, destination city, class of travel, duration of flight, days left before departure, and ticket price.
Our goal with this analysis is to uncover patterns and insights in the dataset and, ultimately, to understand the factors influencing the flight prices.

## The EDA is structured around five main research questions:

1. Does the price vary across different airlines?
2. How is the price affected when tickets are bought just 1 or 2 days before departure?
3. Does the ticket price change based on the departure and arrival time?
4. How does the price change with different source and destination cities?
5. How does the ticket price vary between Economy and Business class flights?

Through the EDA, we employ various data visualization and data manipulation techniques to delve into these questions. The insights gathered will not only help us understand the dataset better but also enable us to build a more accurate predictive model in the future.
Each research question is addressed in a separate section, allowing for an organized and thorough investigation. We hope this analysis provides valuable insights into flight price variations and aids in the development of effective prediction models.

![image](https://github.com/Thebtiboutheina/Flight-Price-Prediction/assets/58167996/712a5bf2-c627-4989-8ca7-562300ebbf56)
