# About

This is a simple analytics project examining traffic collisions in New York City. It loads data about car crashes from the [NYC Open Data's Crashes dataset](https://dev.socrata.com/foundry/data.cityofnewyork.us/h9gi-nx95) via API and weather data from the [NOAA Climate Data Online API](https://www.ncdc.noaa.gov/cdo-web/webservices/v2).  

For the crashes, we only request data from 2019. For weather data, we get one year of precipitation records from a weather station near LaGuardia Airport - [GHCND:USW00014732](/images/weather_station.jpg?raw=true)  

We ask some simple questions, such as:
* Does precipitation affect traffic safety?  
* Where are crashes happening?  
* When are crashes happening?  
* What factors are associated with increased injury or death?   

# Technical Requirements

This is a Jupyter notebook. You will need common Python libraries, a Jupyter environment, as well as some additional packages:

* [**folium**](https://python-visualization.github.io/folium/)  
* [**pingouin**](https://pingouin-stats.org)  

You'll also need to make this a **trusted notebook** to see the embedded maps. In Jupyter Notebook, you can do this by going to the **File** menu and selecting **Trust Notebook** from the dropdown.

# API Keys

API keys for NYC Open Data and NOAA are read locally from *api_keys/api_key_nyc_open_data.txt* and *api_keys/api_key_noaa.txt*, respectively.  

If you have api_keys.zip, extract it to a folder called api_keys in the same directory as the notebook.   

# Sample Visuals

### Heatmap of Crash Locations

![static heatmap of crash locations, requires folium](/images/static_heatmap.jpg)  

### Animated Heatmap of Crash Locations

![animated heatmap of crash locations at all hours of the day, requires folium](/images/animated_heatmap.jpg)