# Weather Py

Evaluation of 500+ random cities around the world utilizing citypy and random latitude and longitude.
   
Utilized OpenWeatherMap API, Jupyter Notebook, Matplotlib and Pandas.

Generated lists of City, Country, Latitude, Longitude, Humidity, Max. Temperature, Wind Speed and Cloudiness for the 500+ cities.

Plotted scatter plots of the following relationships:

[Temperature (F) vs. Latitude](https://github.com/drjulie2105/python-api-challenge/commit/84e56c856367271ff7fa14fc3e393bfb28a0bcfc)

[Humidity (%) vs. Latitude](https://github.com/drjulie2105/python-api-challenge/blob/development/WeatherPy/lat_humid.png)

[Cloudiness (%) vs. Latitude](https://github.com/drjulie2105/python-api-challenge/blob/development/WeatherPy/lat_cloud.png)

[Wind Speed (mph) vs. Latitude](https://github.com/drjulie2105/python-api-challenge/blob/development/WeatherPy/lat_wind.png)

Plotted linear regression plots separating Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude):

- Northern Hemisphere - Temperature (F) vs. Latitude
- Southern Hemisphere - Temperature (F) vs. Latitude
- Northern Hemisphere - Humidity (%) vs. Latitude
- Southern Hemisphere - Humidity (%) vs. Latitude
- Northern Hemisphere - Cloudiness (%) vs. Latitude
- Southern Hemisphere - Cloudiness (%) vs. Latitude
- Northern Hemisphere - Wind Speed (mph) vs. Latitude
- Southern Hemisphere - Wind Speed (mph) vs. Latitude

Summarized what the linear regression charts demonstrated after each chart.

Saved a [CSV](https://github.com/drjulie2105/python-api-challenge/blob/development/WeatherPy/weather_df.csv) of all retrieved data and a PNG image for each scatter plot.
   
   ### Three Observable Trends
   #### 1. There is a strong positive correlation between Latitude and Maximum Temperature in the Southern Hemisphere.
   #### 2. There is a strong negative correlation between Latitude and Maximum Temperature in the Northern Hemisphere.
   #### 3. There is no correlation between Latitude and Humidity, Latitude and Cloudiness, or Latitude and Wind Speed.
     
        


# VacationPy


   Used Gmaps, Matplotlib, Pandas to evaluate destinations with "Perfect" weather to plan future 
   vacations.
 
   Pulled the weather CSV file from WeatherPy and put into DataFrame
   
   Displayed a heat map utilizing Latitude/Longitude as the locations and the humidity as the weight.
   
   ![image](https://github.com/drjulie2105/python-api-challenge/blob/development/heat_map_final.png)
  
   Made a new DataFrame of "Perfect" weather of the following criteria:
   -A max temperature lower than 80 degrees but higher than 70.
   -Wind speed less than 10 mph.
   -Zero cloudiness.

   Dropped any rows that did not contain all three conditions.

   Used Google Places API to find the first hotel for each city located within 5000 meters of your 
   coordinates.

   Ploted the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and 
   Country.
   
   ![image2](https://github.com/drjulie2105/python-api-challenge/blob/development/hotel_heat_map.png)
