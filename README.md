
## CAB Fare Prediction ML Project
![image](https://cdn.vox-cdn.com/thumbor/48hcOptdzrPxAk8q7uT5xJyeQRk=/0x0:1024x685/920x613/filters:focal(431x262:593x424):format(webp)/cdn.vox-cdn.com/uploads/chorus_image/image/52783855/manh_cab.0.0.jpg)

This project is focused on predicting taxi fares in New York City using machine learning techniques. The dataset used for this project includes information about various features of taxi rides, such as pickup and dropoff time, passenger count, trip distance, fare amount, and more.
## Dataset
The dataset used for this project contains the following columns:

VendorID: ID of the taxi vendor.

tpep_pickup_datetime: Date and time when the passenger(s) were picked up.

tpep_dropoff_datetime: Date and time when the passenger(s) were dropped off.

passenger_count: Number of passengers in the taxi ride.

trip_distance: Distance covered by the taxi in the trip.

RatecodeID: Rate code for the trip.

store_and_fwd_flag: Flag indicating whether the trip data was held in vehicle memory before sending to the vendor.

PULocationID: TLC Taxi Zone in which the taxi pickup occurred.

DOLocationID: TLC Taxi Zone in which the taxi dropoff occurred.

payment_type: Payment method used for the trip.

fare_amount: The total fare amount for the trip.

extra: Extra charges added to the fare amount.

mta_tax: Tax charged to the passenger by the Metropolitan Transportation Authority.

tip_amount: Tip amount given to the driver by the passenger.

tolls_amount: Bridge and tunnel tolls charged during the trip.

improvement_surcharge: Surcharge assessed by the taxi on improved transportation.

total_amount: Total amount charged to the passenger for the trip, including all surcharges and tips.

congestion_surcharge: Surcharge assessed on trips in the Manhattan congestion zone.

airport_fee: Airport fee assessed for trips to/from JFK and LaGuardia airports.
## Analysis
The analysis of the dataset was done using Jupyter Notebook.
## Feature Engineering 
feature engineering, where we created new features by extracting information from the pickup and dropoff datetimes. We also used the percentile method to treat outliers in the dataset.
![image](https://user-images.githubusercontent.com/111660500/224512890-d6347be6-0c0f-4b94-aa69-6998294cb8c1.png)

## Multicollinearity Check
we checked for multicollinearity among the columns to ensure that the data was suitable for linear regression. After confirming that the data was appropriate for linear regression, we used the linear regression algorithm to predict taxi fares.
![image](https://user-images.githubusercontent.com/111660500/224512911-66c4450b-5081-41c0-9b41-e3d34218d6ef.png)

## Problem We Faced and Solution
 The data was not normally distributed and we were unable to force transform it in normalize form
 ![image](https://user-images.githubusercontent.com/111660500/224512994-3d893ead-bcd8-474b-9fd0-beffb99e7d5d.png)
Knowing that we still run Linear Regression and we also ran the stochastic gradient descent (SGD) regressor to make predictions. The R-squared value for the linear regressor was 0.95, and the score for the SGD regressor was also 0.95.
## Conclusion
In this project, we predicted taxi fares in New York City using machine learning techniques.

![image](https://user-images.githubusercontent.com/111660500/224513085-d7042128-9936-4f2a-8e10-3306ea1b14ff.png)

We used the linear regression algorithm and the stochastic gradient descent (SGD) regressor to make predictions. The R-squared value for the linear regressor was 0.95

![image](https://user-images.githubusercontent.com/111660500/224513155-4b5e0ee8-4904-49d2-b4c0-af2320f17e6b.png)
The score for the SGD regressor was also 0.95

![image](https://user-images.githubusercontent.com/111660500/224513163-e0aeff3a-ed79-4a84-a539-caa23aaeddf9.png)
