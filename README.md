# BoomBikeAssignment
A Linear Regression Model on a Rental Bike organization to increase their demand.

# Linear Regression Model for Prediction of Hiring of Bikes
- A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

- In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19.


## Table of Contents
* [Objective](#Objective)
* [Business Goal](#business-goal)
* [Data Caveats](#data-caveats)
* [Model Buidling](#model-building)
* [Libraries Used](#Libraries-used)
* [Data Dictionary](#data-dictionary)
* [References](#references)
* [Inferences](#inferences)
* [Critical Features](#critical-features)
* [Data Citation](#data-citation)


<!-- You can include any other section that is pertinent to your problem -->
## Objective
- Build a multiple linear regression model for the prediction of demand for shared bikes.

## Business Goal
 - Find variables are significant in predicting the demand for shared bikes and how well those variables describe the bike demands. Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

- Based on the goal mentioned above, model the demand for shared bikes with the available data.

## Data Caveats

* In the dataset that some of the variables like 'weathersit' and 'season' have values as 1, 2, 3, 4 which have specific labels associated with them (as described in the data dictionary). These numeric values associated with the labels may indicate that there is some order to them - which is actually not the case. So, it is advisable to convert such feature values into categorical string values before proceeding with model building.

* The column 'yr' has two values 0 and 1 indicating the years 2018 and 2019 respectively. Since these bike-sharing systems are slowly gaining popularity, the demand for these bikes is increasing every year proving that the column 'yr' might be a good variable for prediction. So think twice before dropping it.

## Model building

 - In the dataset provided,there are three columns named 'casual', 'registered', and 'cnt'. The variable 'casual' indicates the number casual users who have made a rental. The variable 'registered' on the other hand shows the total number of registered users who have made a booking on a given day. Finally, the 'cnt' variable indicates the total number of bike rentals, including both casual and registered. The model should be built taking this 'cnt' as the target variable.

## Libraries Used
- Pandas
- Numpy
- Seaborn
- Matplotlib
- Scikit Learn
- Statsmodels

## Data Dictionary

- instant: record index
- dteday : date
- season : season (1:spring, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2018, 1:2019)
- mnth : month ( 1 to 12)
- holiday : whether day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
- weekday : day of the week
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
- weathersit :
> - 1: Clear, Few clouds, Partly cloudy, Partly cloudy
> - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
> - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
> - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : temperature in Celsius
- atemp: feeling temperature in Celsius
- hum: humidity
- windspeed: wind speed
- casual: count of casual users
- registered: count of registered users
- cnt: count of total rental bikes including both casual and registered


## Critical Features
- 'yr'
- 'mnth'('September','November')
- 'Winter', 
- 'Tues', 
- 'holiday', 
- 'Mist', 
- 'windspeed', 
- 'Spring', 
- 'Light rain'

## Acknowledgements
- This research was supported by IIIT-Bangalore and upgrad online learning platform.

## Contributors
* [Ramanujam Srinivasan](https://github.com/srinirama/)
