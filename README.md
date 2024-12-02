# data512-final
Author: Ashwin Naresh

## License 
This project falls under the MIT license and is not used for profit. The material here follows all terms of use and is available for others to use.

## Project Details
This project aims to investigate the impact of wildfires on the city of Savannah, GA. We will use publically available wildfire and air quality data. The main notebook contains a breakdown of the various analyses we will conduct.

## File Breakdown

Main Notebook:
- part1-analysis.ipynb (Point of Entry for the Project)

Reference Notebooks for API Code:
- epa_air_quality_history_example.ipynb
- wildfire_geo_proximity_example.ipynb

Input Data File:
- wildfire/USGS_Wildland_Fire_Combined_Dataset.json (not inlcuded due to size. Link can be found in the main notebook)

Output Data Files: (These are files that are used to load data from so we don't have to call the API's over and over again)
- parsed_data.csv (Contains wildfire data)
- parsed_aqi_data.csv (Contains aqi data)

## Project Reflection and Extra Details
The project reflection can be found in the PDF file located in this repository.
