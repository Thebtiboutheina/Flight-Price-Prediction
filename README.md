# Flight-Price-Prediction

## Project Overview
This project is about building models to predict flight prices based on various features, using the Flight Price Prediction dataset from Kaggle. The models were trained and evaluated on various features including airlines, flight number, departure time, stops, arrival time, class, duration, and days left for the flight.
## Results
The results obtained from the models were as follows:

	Model            	MAE	         MSE	        R2 Score
	Linear Regression	4580.820538	 46480151.13	0.909097
        Random Forest	        1069.553350	 7433253.57	  0.985463
	Linear SVM	        4951.540023	 65052444.78	0.872775
	Gradient Boosting	2910.739788	 24000176.98	0.953062
	XGBoost	                2291.345928	 16060929.54	0.968589

The Random Forest (RF) model's results are indeed very good, and among the models you've tried, it's the best. It has a very high R2 score of approximately 0.985, which is very close to the perfect score of 1. This suggests that the RF model can explain approximately 98.5% of the variation in the flight prices, which is quite high.
The Mean Absolute Error (MAE) of the RF model is approximately 1069.55. This indicates that on average, the model's predictions are around $1069.55 off from the actual prices. This might sound like a lot, but in the context of flight prices, which can vary widely and can be quite high, this error could be acceptable depending on the range of flight prices in your dataset.
The Mean Squared Error (MSE) is also relatively low. Remember that MSE tends to penalize larger errors more severely than smaller ones, due to the squaring of the residuals.
![image](https://github.com/Thebtiboutheina/Flight-Price-Prediction/assets/58167996/712a5bf2-c627-4989-8ca7-562300ebbf56)

## Exploratory Data Analysis:
We performed exploratory data analysis to understand the distribution of data, relationship among features, and identify any potential outliers. The "Flight Price Prediction" dataset available on Kaggle (https://www.kaggle.com/datasets/shubhambathwal/flight-price-prediction/code?resource=download). We analyzed the correlation of different features with the flight price, investigated the relationship between the number of stops and flight prices for different classes, and analyzed the impact of the time of departure and arrival on ticket price.
Our goal with this analysis is to uncover patterns and insights in the dataset and, ultimately, to understand the factors influencing the flight prices.
The EDA is structured around five main research questions:

1. Does the price vary across different airlines?
2. How is the price affected when tickets are bought just 1 or 2 days before departure?
3. Does the ticket price change based on the departure and arrival time?
4. How does the price change with different source and destination cities?
5. How does the ticket price vary between Economy and Business class flights?

## Outliers:
Outliers were identified using the IQR method but considering the nature of the dataset and the problem at hand, these outliers were kept in the dataset, considering them as possible normal values.

## Feature Engineering:
We performed Label Encoding on ordinal variables and One-Hot-Encoding on nominal categorical variables to transform them into a form that could be provided to machine learning algorithms.
Model Building and Evaluation
We split our dataset into a training set and a test set. Then, we built and evaluated several machine learning models including Linear Regression, Random Forest, Linear SVM, Gradient Boosting, and XGBoost. The models were evaluated using Mean Absolute Error (MAE), Mean Squared Error (MSE), and R2 Score.

## Conclusion
The Random Forest model provided the best performance among the models we tested, achieving a high R2 score and a relatively low Mean Absolute Error. These results indicate that the model can accurately predict flight prices, as it can explain 98.5% of the variation in flight prices.
