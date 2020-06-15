## Introduction
The **goal of this notebook** is to apply new skills learned from the [Geospatial Analysis course](https://www.kaggle.com/learn/geospatial-analysis) to visualize the air quality in Budapest, Hungary. I live in this city, so I thought it would be interesting to compare its districts in this regard. 

I have compiled the dataset for this project from a [website](https://aqicn.org/city/budapest/) that is measuring air pollution across the world. There are measurements for 5 main parameters over the years 2016-2019: co, no2, o3, pm10, so2 (read further about these pollutants in the "Pollutants" section [here](https://en.wikipedia.org/wiki/Air_pollution)). 

In Budapest there are 12 measuring stations, in my analysis I had to remove one of them (situated in the 5th district) as it is fairly new and doesn't have measurements for the whole period of research. 

The geodata about Budapest districts is taken from OSMNX (a Python package for downloading administrative boundary shapes and street networks from OpenStreetMap) using [geocoding](https://www.kaggle.com/alexisbcook/manipulating-geospatial-data).

During my research I have created the following 4 maps of Budapest districts:
1. A simple map showing district borders and location of 11 measuring stations with the option to choose from a range of map tiles;
2. A choropleth map showing the Air Quality Index (AQI) value for each district (a maximum among median values of the 5 measured parameters);
3. A timeslider choropleth map demonstrating how the AQI value for each district changed over the researched period (2016-2019);
4. A choropleth map displaying 5 parameters of the aggregate AQI using feature group and layer control.

The logbook of this project can be found [here](https://docs.google.com/spreadsheets/d/1N_3xASxg3NRPEUMzZn5oDMCpE0OkMCAhTfPZsqVewjc/edit?usp=sharing). It includes the following tabs:

- Time spent on the project
- Ideas for this project
- Useful information for the project (links and info I found about Geospatial Analysis)
- AQI (data sources)
- Possible future improvements
- Lessons learned from the project

This repo contains the following files:
- Input folder (district boarders data, air quality data, description of AQI levels);
- Output folder (4 maps of this project in the html format);
- Jupyter notebook with my code (the maps might not be displayed if you open this file on github, please download html maps and open them separately).

The project can also be found on this [Kaggle page](https://www.kaggle.com/tatianasnwrt/visualizing-air-quality-in-budapest-folium?scriptVersionId=36417494).
