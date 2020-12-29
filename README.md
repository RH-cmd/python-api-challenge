# Python Api Challenge - What's the Weather Like?

![World Map](https://www.mapsofindia.com/worldmap/world-continent-map.jpg)

Background
Whether financial, political, or social -- data's true power lies in its ability to answer questions definitively. So let's take what you've learned about Python requests, APIs, and JSON traversals to answer a fundamental question: "What's the weather like as we approach the equator?"
Now, we know what you may be thinking: "Duh. It gets hotter..."
But, if pressed, how would you prove it?

Part I - WeatherPy
In this example, you'll be creating a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities.

The first requirement is to create a series of scatter plots to showcase the following relationships:

- Temperature (F) vs. Latitude
- Humidity (%) vs. Latitude
- Cloudiness (%) vs. Latitude
- Wind Speed (mph) vs. Latitude

After each plot, add a sentence or two explaining what the code is analyzing.
The second requirement is to run linear regression on each relationship. This time, separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

- Northern Hemisphere - Temperature (F) vs. Latitude
- Southern Hemisphere - Temperature (F) vs. Latitude
- Northern Hemisphere - Humidity (%) vs. Latitude
- Southern Hemisphere - Humidity (%) vs. Latitude
- Northern Hemisphere - Cloudiness (%) vs. Latitude
- Southern Hemisphere - Cloudiness (%) vs. Latitude
- Northern Hemisphere - Wind Speed (mph) vs. Latitude
- Southern Hemisphere - Wind Speed (mph) vs. Latitude

After each pair of plots, explain what the linear regression is modeling. 

![Northern Hemisphere Linear Regression](https://github.com/RH-cmd/python-api-challenge/blob/main/WeatherPy/output_data/Northern%20Hemisphere%20-%20Max%20Temp%20vs.%20Latitude%20Linear%20Regression.png)

Your final notebook must:

Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
Perform a weather check on each of the cities using a series of successive API calls.
Include a print log of each city as it's being processed with the city number and city name.
Save a CSV of all retrieved data and a PNG image for each scatter plot. These documents will be located in a folder named [Output_Data](https://github.com/RH-cmd/python-api-challenge/tree/main/WeatherPy/output_data). 


Part II - VacationPy
Now let's use your skills in working with weather data to plan future vacations. Use jupyter-gmaps and the Google Places API for this part of the assignment.

To complete this part of the assignment,you will need to do the following:


Create a heat map that displays the humidity for every city from Part I.


Narrow down the DataFrame to find your ideal weather condition using the following conditions:


- A max temperature lower than 80 degrees but higher than 70.

- Wind speed less than 10 mph.

- Zero cloudiness.

- Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.

![Humidity Heatmap](https://github.com/RH-cmd/python-api-challenge/blob/main/VacationPy/output_data_maps/humidity_heatmap.png)


Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.


Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.


![Hotels Heatmap](https://github.com/RH-cmd/python-api-challenge/blob/main/VacationPy/output_data_maps/hotel_heatmap.png)



As final considerations:

You must complete your analysis using a Jupyter notebook.

You must use the Matplotlib or Pandas plotting libraries.

For Part I, you must include a written description of three observable trends based on the data. This will be included at the top of the notebook.

For Part II, you must include a screenshot of the heatmap you create and include it in your submission. These screenshots will be located inside a folder called [Output_Data_Maps](https://github.com/RH-cmd/python-api-challenge/tree/main/VacationPy/output_data_maps). 




