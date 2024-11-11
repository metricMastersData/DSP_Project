# Flight Price Prediction

## Team Members
Abhishek Kushary, abhishekkush@iisc.ac.in​
Aju John Thomas, ajuthomas@iisc.ac.in​
Taru Kaushik, tarukaushik@iisc.ac.in​
Yuvasree Pamujula, yuvasreep@iisc.ac.in

## Problem Statement:
The goal of this project is to predict flight ticket prices based on various factors such as departure and arrival locations, time of booking, airline, flight duration and other relevant features. Predicting flight prices will help users make informed decisions about when to book flights to get the best prices.

## Datasets:

### FlightFarePrediction_data.csv
The "Flight Price Prediction" dataset is sourced from Kaggle and contains historical flight pricing data from multiple airlines. The dataset aims to predict the prices of flights based on various features like source and destination airports, airlines, date of travel, and flight duration.

#### Features/Columns in the Dataset
The dataset contains the following features:
- `IATASource`: The departure airport IATA Code (categorical, e.g., 'New York', 'Los Angeles').
- `IATADestination`: The arrival airport IATA Code (categorical, e.g., 'London', 'Paris').
- `airlineName`: The airline company operating the flight (categorical, e.g., 'Delta', 'American Airlines').
- `flightDate`: The date the journey (date).
- `duration`: The duration of the flight in hours (numerical, float).
- `baseFare`: The basic ticket price for the flight (numerical, float).
- `totalFare`: The total ticket price for the flight (numerical, float).
- `isBasicEconomy`: The class of the flight (categorical, e.g., 'Economy', 'Business').
- `noOfStops`: Number of stopovers during the flight (numerical, integer).

### Airports.csv
The "Airport" dataset is sourced from Kaggle and contains the city, state, country, longitude and latitude data of airports.

#### Features/Columns in the Dataset
This dataset contains following feautures:
- `IATA`: The IATA code of the airport (categorical, e.g., 'Denver Inti', 'Adams').
- `AIRPORT`: The name of the airport (categorical, e.g., 'Denver Inti', 'Adams').
- `CITY`: The city of the airport (categorical, e.g., 'Denver', 'Little Rock').
-  `STATE`: The state of the airport (categorical, e.g., 'CO', 'AR').
- `COUNTRY`: The Country of the airport (categorical, e.g., 'USA', 'USA').
- `LATITUDE`: The Latitude of the airport (numerical, float).
- `LONGITUDE`: The Longitude of the airport (numerical, float).


