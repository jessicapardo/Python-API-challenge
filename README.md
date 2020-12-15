# Python-API-challenge

# What's the Weather Like?

![Equator](Images/equatorsign.png)

## Background

Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"

Now, we know what you may be thinking: _"Duh. It gets hotter..."_

But, if pressed, how would you **prove** it?

## Part I - WeatherPy

For this exercise, a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator was created. It was accomplished by utilizing a [simple Python library](https://pypi.python.org/pypi/citipy) and the [OpenWeatherMap API](https://openweathermap.org/api) to create a representative model of weather across world cities.

The first set of scatter plots showcase the following relationships:

* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

The second set of graphs shows linear regressions on each relationship. This time, separating the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

More details of the analysis and visualization of the graphs can be seen in the WeatherPy Jupyther notebook: [WeatherPy](WeatherPy/WeatherPy.ipynb)


## Part II - VacationPy

For this exercise, a Python scrip was created to work with weather data to plan future vacations. It was accomplished by utilizing jupyter-gmaps and the Google Places API.

First, a heat map that displays the humidity for every city from Part I was creaded

![Heat map all cities](Images/all_cities_humidity_map.png)

Second, the data was narrow down to find the ideal weather condition for a vacation spot using the following parameters:

* A max temperature lower than 80 degrees but higher than 70.
* Wind speed less than 10 mph.
* Zero cloudiness.
* Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

Using Google Places API, amap was created to show the first hotel for each city with the ideal weather condition located within 5000 meters 

![hotel map](Images/hotel_map.png)

More details of the analysis and visualization of the graphs can be seen in the VacationPy Jupyther notebook: [VacationPy](VacationPy/VacationPy.ipynb)

### Copyright

Trilogy Education Services © 2020. All Rights Reserved.
