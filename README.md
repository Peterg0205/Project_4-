# Project_4- Taking Flight 

## Table of Contents

- [Installation](#installation)
- [Background](#background)
- [Getting Started](#getting)
- [Cleaning Data and Applying Supervised Machine Learning](#CleaningDataandApplyingSupervisedMachineLearning)
- [Credits](#credits)

## Installation:

To be able to run the jupyter notebook and VS Code you will need the following imports

- BeautifulSoup
- Matplotlib
- Numpy
- Pandas
- Scipy.stats
- Seaborn
- Graphviz

## Background:
 In today's society, more than 671 milllion people travel by air. Flights are essentially the fastest form of transportation. However, the main concern with travelling by air are delayed flights. Delayed flights can be such a pain thats whether arriving to a destination late or missing a connecting flight. In this project, our objective is to use machine learning to see whether we can predict a delay for a flight flying out of Hartsfield International Airport. 

## Getting Started
### Retrieve the data

The data is located in the Resources folder.

* `Resources/Airlines.csv`

Import the data using Pandas.


## Resources, Libraries, & Tools

Sources:

https://www.kaggle.com/datasets/jimschacko/airlines-dataset-to-predict-a-delay

Tools & languages: Jupyter Notebook and SQL


## Cleaning Data and Applying Supervised Machine Learning
1 – Uploading Data:
 The data was saved as csv files then uploaded to SQL. We connected the SQL database to jupyter notebook in order to proceed to our next step.  

2 – Cleaning the Data:
    We filtered our dataset to include only fights from Atlanta because majority of the dataset had flights flying out of Atlanta. Also, Atlanta hosts more than 2500 flights daily which our group thought would be a good source of data for prediciting delayed flights. To ensure no bias in the data, we chose to select a random sample of 500. We also isolated “Flight ID” column since it had no bearing on whether a flight was delayed or not. The largest outliers affecting the delays were "flight length" we also had to to remove it from the data. 

3 - Applying Supervised Machine Learning:
id - Unique row identifier ID.

Airline - Abreviated name of different commericial airlines.

Flight - Tell about the type of aircraft used.

AirportFrom - The airport origin for the flight.

AirportTo - The airport destination for the flight.

DayOfWeek - Day of the week when the flight took place.

Time - Time of flight.

Length - Length of flight.

Delay - Whether or not there was a delay.

For this analysis, we used several different types of supervised machine learning methods in an attempt to make the most accurate prediction for whether there is a flight delay. This is a classification problem where the dependant varaible (Delay) has two states, 0 or 1, where 0 means there was no delay and 1 means there was a delay. This data provides only generic and static flight info. Information that can vary up until flight time, like weather, are not included in this data becauase that kind of information is generally unknown until flight time.

-Model 1: fully connected nueral network containing three hidden layers with 400, 200, and 10 neurons 

-Model 2: triple hidden layer model with 100, 50, and 50 nuerons in each hidden layer 

-Model 3: simple double hidden layer model with 60 and 30 neurons

## Future Considerations

In the future, we would like to improve the accuracy of the model predictions, by expanding our dataset to include more airports to take away potential bias from just using Atlanta- Hartsfield as the departure point. Also, reviewing the data cleaning process to ensure we are eliminating erroneous data and changing the data point to increase the accuracy above 75%. We would also include datasets from other sources with other relevant data points to predict delays (weather, labor interruptions, etc.) Another thing, we could do in the future is run model on individual airlines to see if any weighs on the dataset adversely. Creating a website so travelers can change the search parameters and predict the chance of delay prior to flying would be something we would consider doing in the future. 


## Credits
Team members:

Peter Gunn 

Hana Tafesse

Ewansiha Simmons 

Herman Tucker 