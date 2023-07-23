# python-api-challenge
Module 6 Challenge - Python APIs
- Using Python requests, APIs and JSON traversals to create output in order to analyse weather and geolocation data.

## Table of Contents

- [About](#about)
- [Getting Started](#getting_started)
- [Installing](#installing)
- [Usage](#usage)
- [Contributing](#contributing)

## About
**Part 1: WeatherPy**
Python script to visualise the weather of over 500 cities of varying distances from the equator.  
what was the purpose of each part....

Tools/Libraries Imported:
- matplotlib.pyplot library: used for creating graphs and charts
- pandas library: used for data manipulation and analysis
- numpy library: used for numerical computations
- requests library: for making HTTP requests so can interact with APIs and fetch data from web servers
- time: to provide time related functions
- scipy.stats.lingress: from Scipy library to create linear regression
- pprint: pretty print data structures to make them more readable
- citypy library: to determine the nearest city for a given latitude and longitude so can map coordinates to the corresponding name

Python Script:
- File: WeatherPy.ipynb
- Purpose:
  - Create a list a random coordinates that will create a list of cities using the citypy library.
  - Create Plots to Showcase the Relationship Between Weather Variables and Latitude
    - Use the OpenWeatherMap API to retrieve weather data from the cities list generated in the started code
    - Create the Scatter Plots:
      - Latitude Vs. Temperature
      - Latitude Vs. Humidity
      - Latitude Vs. Cloudiness
      - Latitude vs. Wind Speed Plot
  - Compute Linear Regression for Each Relationship
    - Temperature vs. Latitude Linear Regression Plot
    - Humidity vs. Latitude Linear Regression Plot
    - Cloudiness vs. Latitude Linear Regression Plot
    - Wind Speed vs. Latitude Linear Regression Plot
  
Output Folder:
- File: cities.csv
  - Contains: list of cities with longitude, latitude, max temp, humidity, cloudiness, wind speed, country and date.
- Files: Fig1.png, Fig2.png, Fig3.png, Fig4.png
  - Contains picture files of the 4 scatter plots listed above. 

**Part 2: VacationPy**  
Python script to create map visualisations, to assist in planning future vacations.  

Tools/Libraries Imported:
- hvplot.pandas library: used for creating interactive plots using hvplot function
- pandas library: used for data manipulation and analysis
- requests library: for making HTTP requests so can interact with APIs and fetch data from web servers
- pathlib.Path: from pathlib module, simplifies the process of working with file paths

 Python Script:
- File: VacationPy.ipynb
- Purpose:
  - Import Libraries and Load the Weather and Coordinates Data
  - Create a map that displays a point for every city in the city_data_df DataFrame. The size of the point should be the humidity in each city.
  - Narrow down the city_data_df DataFrame to find your ideal weather condition
  - Create a new DataFrame called hotel_df
  - For each city, use the Geoapify API to find the first hotel located within 10,000 metres of your coordinates
  - Add the hotel name and the country as additional information in the hover message for each city in the map

## Getting Started
1. Request API keys from:  
  - OpenWeatherMap (https://openweathermap.org/api)
  - Geoapify (https://www.geoapify.com/)
  - need to save API keys in py file saved same folder location as VacationPy.ipynb and WeatherPy.ipynb files.

2. Open Anaconda prompt.
  a. Activate dev enviroment, type: 'conda activate dev'
  b. Navigate to folder location of python scripts VacationPy.ipynb and WeatherPy.ipynb
  c. Open Jupyter Notebook, type: 'Jupyter Notebook'

## Installing
Installation instructions.
mention which libraries were installed, not how...
Install following libraries:  
  - citipy
  - geoviews
  - etc etc

## Usage
A step by step series of examples that tell you how to get a development env running.
activate anaconda dev environment before opening Jupyter Notebook
making sure API keys are saved in the correct location

## Contributing
Contributors names
website data sources to find answers for the project eg stackoverflow
or help from tutor

