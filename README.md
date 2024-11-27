# Flight Price Prediction

## Team Members
Abhishek Kushary, abhishekkush@iisc.ac.in​
Aju John Thomas, ajuthomas@iisc.ac.in​
Taru Kaushik, tarukaushik@iisc.ac.in​
Yuvasree Pamujula, yuvasreep@iisc.ac.in

## Problem Statement
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
- `IATA`: The IATA code of the airport
- `AIRPORT`: The name of the airport
- `CITY`: The city of the airport
-  `STATE`: The state of the airport
- `COUNTRY`: The Country of the airport
- `LATITUDE`: The Latitude of the airport
- `LONGITUDE`: The Longitude of the airport

# 1. Introduction
This project aims to predict flight fares using a comprehensive dataset. The process involves data cleaning, preprocessing, exploratory data analysis (EDA), feature engineering, and model training and evaluation.

# 2. Data Cleaning
It involves specific Column Extraction, Duplicate data Removal and handling Missing numerical Values through median imputation (numerical) and mode imputation (categorical).

# 3. Data Preprocessing
  # . Date and Time Conversion
  - `flightDate` is converted to datetime format.
  - `travelDuration` is transformed from ISO 8601 format to total minutes.
 # . Column Splitting and Transformation
   - `segmentsAirlineName` is split to create `airlineName`
   - Number of stops is calculated.
   - Boolean columns are converted to integers.
   - `flightDate` is split into month, day, and year columns.
 # . Mapping and Extraction
   - Airport codes are mapped to names and cities using a dictionary.
   - First and last segments of arrival and departure times are extracted.
   - Epoch time is converted to datetime for detailed arrival and departure information.
# 4. Exploratory Data Analysis (EDA)
  # . Visualizations
     - Histogram of total fares.
     - Bar chart of total fares by airline.
     - Scatter plot of total fare vs. travel duration.
     - Pie chart of the number of stops.
     - Bar charts of flight frequencies by origin and destination cities.
# 5. Feature Engineering
  # . New Features
      - Time of day classification for arrivals and departures.
      - Season determination based on month.
      - Combined airport and city names.
  # . Optimization:
      - Data types are optimized for memory usage.
      - Relevant columns are selected for prediction.
      - Categorical columns are encoded using one-hot encoding.
      - Additional Visualizations:
      - Pie charts of departure and arrival times by time of day.
      - Heatmap of the correlation matrix for numerical features.
# 6. Model Training & Evaluation
Implemented XGBoost with hyper parameter tuning and cross validation.

      
     
    
 

*Raw csv datasets available in **master** branch.
