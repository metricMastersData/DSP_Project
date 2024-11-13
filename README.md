# Flight Price Prediction

## Team Members
Abhishek Kushary, abhishekkush@iisc.ac.in​
Aju John Thomas, ajuthomas@iisc.ac.in​
Taru Kaushik, tarukaushik@iisc.ac.in​
Yuvasree Pamujula, yuvasreep@iisc.ac.in

## Problem Statement:
The goal of this project is to predict flight ticket prices based on various factors such as departure and arrival locations, time of booking, airline, flight duration and other relevant features. Predicting flight prices will help users in making informed decisions about when to book flights to get the best prices.

## Datasets:

### FlightFarePrediction_data.csv
The "Flight Price Prediction" dataset is sourced from Kaggle and contains historical flight pricing data from multiple airlines. The dataset aims to predict the prices of flights based on various features like source and destination airports, airlines, date of travel, and flight duration.

#### Features/Columns in the Dataset
The dataset contains the following features:

- `searchDate`: Date when the flight search was made.
- `flightDate`: Date of the flight.
- `startingAirport`: The departure airport
- `destinationAirport`: The arrival airport
- `fareBasisCode`: Code indicating fare rules.
- `travelDuration`:  Total time of the flight.
- `elapsedDays`: Days since flight search.
- `isBasicEconomy`: Indicates if it's a basic economy ticket.
- `isRefundable`: Indicates if the ticket is refundable.
- `isNonStop`: Indicates if the flight is nonstop.
- `baseFare`: The base price of the ticket.
- `totalFare`: Total price including taxes and fees.
- `seatsRemaining`: Number of available seats.
- `totalTravelDistance`: Total distance of the flight.
- `segmentsDepartureTimeEpochSeconds`: Departure time in epoch seconds.
- `segmentsDepartureTimeRaw`: Raw departure time.
- `segmentsArrivalTimeEpochSeconds`: Arrival time in epoch seconds.
- `segmentsArrivalTimeRaw`: Raw arrival time.
- `segmentsArrivalAirportCode`: Arrival airport code.
- `segmentsDepartureAirportCode`: Departure airport code.
- `segmentsAirlineName`: Airline name for the flight segment.
- `segmentsAirlineCode`: Airline code for the flight segment.
- `segmentsEquipmentDescription`: Aircraft description.
- `segmentsDurationInSeconds`: Duration of the flight segment in seconds.
- `segmentsDistance`: Distance of the flight segment.
- `segmentsCabinCode`: Cabin class code for the flight segment.

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

*Raw csv datasets available in **master** branch.
