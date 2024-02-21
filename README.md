# Tracking the movement of International Space Station (ISS) with Python  

## Project Overview: 
This project monitors the International Space Station’s (ISS) trajectory in real-time. The primary goal was to develop a reliable method for tracking the ISS’s position across the Earth’s surface and obtain information about the weather along its orbital path. 

## Method: 
- Acquire Data via Web Scraping: 
  - We started this project by using a script that executes every 5 seconds to fetch the current location of the ISS from a designated website. This site provides the ISS’s coordinates in JSON format to ensure we have access to real-time data and its longitude, latitude, and timestamp. 

- Process Data with Pandas: 
  - We used the Pandas library to read and process the information stored in a CSV file. 

- Visualization with GeoPandas: 
  - To map the ISS's trajectory, we used GeoPandas. Using the Natural Earth database, we plotted the ISS's path over a world map. This provided us with a visual representation of the ISS’s journey and its global movement patterns.

