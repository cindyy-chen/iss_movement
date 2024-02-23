# Tracking the movement of International Space Station (ISS) with Python  



## Project Overview: 
This project monitors the International Space Station’s (ISS) trajectory in real-time. The primary goal was to develop a reliable method for tracking the ISS’s position across the Earth’s surface and obtain information about the weather along its orbital path. 

## Method: 
### How the data was collected:

This script accesses several times (at a given frequency) a website 
to collect the timeseries positions of the ISS. For each position
(with the corresponding time), it determines if it is a land or not (ocean),
the country name (if it is land) of the location, and
the current weather conditions (temperature, windspeed).
This script accesses a website (every 5 seconds).
All the collected timeseries data (date/time, latitude, longitude,
temperature, windspeed, country name) is stored in a CSV file that
will later be analyzed with Pandas, GeoPandas and MovingPandas.

Required modules: Pandas, global_land_mask, reverse_geocode

- Acquire Data via Web Scraping: 
  - We started this project by using a script that executes every 5 seconds to fetch the current location of the ISS from a designated website. This site provides the ISS’s coordinates in JSON format to ensure we have access to real-time data and its longitude, latitude, and timestamp. 

- Process Data with Pandas: 
  - We used the Pandas library to read and process the information stored in a CSV file. 

- Visualization with GeoPandas: 
  - To map the ISS's trajectory, we used GeoPandas. Using the Natural Earth database, we plotted the ISS's path over a world map. This provided us with a visual representation of the ISS’s journey and its global movement patterns.

