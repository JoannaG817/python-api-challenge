## python-api-challenge

Part I - WeatherPy

I created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a Python library and the OpenWeatherMap API.

I built a series of scatter plots to showcase the following relationships:
Latitude vs. Temperature (C) 
Latitude vs. Humidity (%) 
Latitude vs. Cloudiness (%) 
Latitude vs. Wind Speed (m/s) 

I ran linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

Northern Hemisphere - Latitude vs. Temperature (C)
Southern Hemisphere - Latitude vs. Temperature (C)
Northern Hemisphere - Latitude vs. Humidity (%)
Southern Hemisphere - Latitude vs. Humidity (%)
Northern Hemisphere - Latitude vs. Cloudiness (%)
Southern Hemisphere - Latitude vs. Cloudiness (%)
Northern Hemisphere - Latitude vs. Wind Speed (m/s)
Southern Hemisphere - Latitude vs. Wind Speed (m/s)

After each pair of plots, I explained what the linear regression is modeling.

I randomly selected more than 500 unique (non-repeat) cities based on latitude and longitude. Performed a weather check on each of the cities using a series of successive API calls. I included a print log of each city as it's being processed with the city number and city name. Saved a CSV of all retrieved data and a PNG image for each scatter plot.

Part 2: VacationPy

In this section I used Jupyter notebooks, the geoViews Python library, and the Geoapify API. 

I narrowed down the city_data DataFrame to find my ideal weather condition. For example:

A max temperature lower than 25C but higher than 12C.
Wind speed less than 8 mph.
Less than 100 cloudy days per year.
ULess than 51% humidity.

Plotted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.
