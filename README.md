# python-api-challenge

## Challenge Details

This challenge was to investigate different weather factors for 500+ cities around the world. To perform this analysis, the following resources were used:
* [OpenweatherMap API](https://openweathermap.org/api) - used to collect weather data for cities around the world
* [CitiPy](https://pypi.org/project/citipy/) - used to generate list of cities to be analyzed in this challenge

## WeatherPy 

First, a list of 500+ cities was generated using CitiPy. Next, weatherdata was collected using OpenWeatherMap's API. A print log of each city as it's being processed with the city number and city name can be seen in the jupyter notebook output. The list of cities used was exported to a csv and can be found in the output folder under WeatherPy.

### Visualizations

Scatter plots were generated to show the following relationships:
* Temperature (F) vs. Latitude
* Humidity (%) vs. Latitude
* Cloudiness (%) vs. Latitude
* Wind Speed (mph) vs. Latitude

These visualizations were exported and saved in the Output folder under WeatherPy.

From there, linear regression was run on each relationship, separating the data into Northern and Southern Hemispheres:
* Northern Hemisphere - Temperature (F) vs. Latitude
* Southern Hemisphere - Temperature (F) vs. Latitude
* Northern Hemisphere - Humidity (%) vs. Latitude
* Southern Hemisphere - Humidity (%) vs. Latitude
* Northern Hemisphere - Cloudiness (%) vs. Latitude
* Southern Hemisphere - Cloudiness (%) vs. Latitude
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
* Southern Hemisphere - Wind Speed (mph) vs. Latitude

To create these linear regressions more efficiently, a function (linregress_func) was created.

Observations of trends are shown after each plot.

## Files Included

* VacationPy folder - the VacationPy jupyter notebook can be found here, which contains all analysis for VacationPy part of the challenge
* WeatherPy folder - 
    * WeatherPy jupyter notebook, which contains all analysis for WeatherPy part of the challenge
    * Output folder containing cities.csv and scatter plot visualizations
* index.html 
