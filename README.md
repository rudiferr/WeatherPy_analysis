# "WeatherPy_analysis" Week 6 Challenge
### Tools Used
* Jupyter Notebooks
* Pandas Dataframes
* Numpy NaN replacement
* Google Maps API
* Weather API

## Purpose
The purpose of this analysis is to create a vacation itinerary for users from specified weather criteria and identified potential travel destinations. By utilizing Google API's, we are able to provide the user with recommended ideal hotels within the chosen weather qualifications.

## Overview
### Destination Choice Creation
In order to create the destination map, we generated a list of 2,000 random latitudes and longitudes. With these coordinates pairs we then retrieved and compiled a list of the nearest cities using the citipy module, combined with the OpenWeatherMap API to request the current weather data from each unique city on the list. We then used Google Maps Places API to create a NearbySearch request to populate a .csv with hotels in those cities. Using Map Layers we were able to combine all of this information into an interactive map that showed all of the potential destinations the user could travel to.

### Itinerary Creation
Using additional Map Layers we then created an interactive map that previewed the route between the user's choices of cities. We also created an additional map that updated the chosen cities and hotels with the previously obtained weather data so everything is available at a glance.
