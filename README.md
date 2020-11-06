# python-api-challenge
 
 ## WeatherPy
 
 ## Analysis
 1. The correlation coeffient and linear regression model shows a strong negative correlation between latitude and maximum temperature in the northern hemisphere. As the latitude decreases, the temperature increases. In the southern hemisphere, the correlation coefficient and linear regression model shows a moderate positive correlation between latitude and maximum temperature. As the latitude increases towards zero, the temperature increases as well.
 2. The correlation coefficent and linear regression model for humidity vs latitude shows a weak positive correlation for both hemispheres. 
 3. Wind speed and latitude have no strong relationship in the northern and southern hemisphere as shown by the correlation and linear regression model.
 
 ## included:
 1. api_keys.py
 2. WeatherPy.ipynb 
 3. [cities.csv](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/output_data/cities.csv) in output_data folder
 4. [output_log.txt](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/output_data/output_log.txt) in output_data folder
 5. png files in images folder
    * Cloudiness vs Latitude - [lat_cloud.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/lat_cloud.png)
    * Humidity vs Latitude - [lat_humid.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/lat_humid.png)
    * Temperature vs Latitude - [lat_temp.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/lat_temp.png)
    * Wind Speed vs Latitude - [lat_wind.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/lat_wind.png)  
    
    * Cloudiness vs Latitude
      * Northern Hemisphere - [north_lat_cloud.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/north_lat_cloud.png)
      * Southern Hemisphere - [south_lat_cloud.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/south_lat_cloud.png)
    * Humidity vs Latitude
      * Northern Hemisphere - [north_lat_humid.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/north_lat_humid.png)
      * Southern Hemisphere - [south_lat_humid.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/south_lat_humid.png)
     * Temperature vs Latitude
       * Northern Hemisphere - [north_lat_temp.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/north_lat_temp.png)
       * Southern Hemisphere - [south_lat_temp.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/south_lat_temp.png)
    * Wind Speed vs Latitude
      * Northern Hemisphere - [north_lat_wind.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/north_lat_wind.png)
      * Southern Hemisphere - [south_lat_wind.png](https://github.com/tratnikc/python-api-challenge/blob/main/starter_code/images/south_lat_wind.png)
    
 
 ## Requirements
 Create a series of scatter plots to showcase the following relationships:  
    * Temperature (F) vs Latitude  
    * Humidity (%) vs Latitude  
    * Cloudiness (%) vs Latitude  
    * Wind Speed (mph) vs Latitude  
 1. Randomly select at least 500 unique cities based on latitude and longitude
 2. Perform a weather check on each of the cities using a series of API calls
 3. Include a print log of cities processed
 4. Save CSV of the cities and png images of each scatter plot  
 5. Create linear regression model on Northern and Southern Hemispheres on the relationships cited above.

 ## Algorithm
 1. Leverage the code citipy to generate a list of random cities using latitude and longitude
 2. OpenWeatherMap free accounts allows 60 calls/minute, send 50 requests in 55sec intervals
 3. Loop through the list of cities, get city weather information, when found, add city to list.
 4. Skip city not found on OpenWeatherMap
 5. Log each city being processed
 5. Save the city information to a csv file
 6. Create a data frame of cities with weather information
 7. Create scatter plots
 8. Calculate correlation coefficient and linear regression model

