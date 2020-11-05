# python-api-challenge
 
 ## WeatherPy
 
 ## Analysis
 1. As indicated by the correlation coefficient and the linear regression model, there is a strong inverse relationship between Max Temperature and Latitude. As the latitude moves north (positive numbers) or south (negative numbers), the temperature goes in the opposite direction. This means that as the latitude goes closer to the north or south poles, the temperature becomes lower.
 2. There 
 ## included:
 1. api_keys.py
 2. WeatherPy.ipynb 
 3. [cities.csv](https://github.com/tratnikc/APIs-challenge/blob/main/starter_code/output_data/cities.csv) in 'output_data' folder
 4. [output_log.txt](https://github.com/tratnikc/APIs-challenge/blob/main/starter_code/output_data/output_log.txt) in the 'output_data' folder
 5. png files in 'images' folder
    * [lat_cloud.png](https://github.com/tratnikc/APIs-challenge/blob/main/starter_code/images/lat_cloud.png)
    * [lat_humid.png](https://github.com/tratnikc/APIs-challenge/blob/main/starter_code/images/lat_humid.png)
    * [lat_temp.png](https://github.com/tratnikc/APIs-challenge/blob/main/starter_code/images/lat_temp.png)
    * [lat_wind.png](https://github.com/tratnikc/APIs-challenge/blob/main/starter_code/images/lat_wind.png)
    
 
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

