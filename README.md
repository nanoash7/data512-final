# data512-final
Author: Ashwin Naresh

## License 
This project falls under the MIT license and is not used for profit. The material here follows all terms of use and is available for others to use.

## Project Details
This project aims to investigate the impact of wildfires on the city of Savannah, GA. We will use publically available wildfire and air quality data. The main notebook contains a breakdown of the various analyses we will conduct.

## Classmate Collaboration
The majority of this project was done individually. I collaborated with some classmates on Part 1 when we needed to design a smoke estimate metric.

## Custom Smoke Estimate Metric
In this project, I use a custom smoke estimate metric that I created along with some class mates. To estimate the smoke of a fire, we use 2 variables: size (acres of wildfire) and distance (distance from the city). Smoke disperses as a function of the square of distance and the amount of smoke scales as a function of surface area. Putting this together we get our naive smoke estimate: Smoke Estimate = Size / (Distance^2).

## File Breakdown

### Main Notebook:
- part1-analysis.ipynb (Point of Entry for the Project Part 1)
- part2-analysis.ipynb (Point of Entry for the Project Part 2)

### Reference Notebooks for API Code:
- epa_air_quality_history_example.ipynb
- wildfire_geo_proximity_example.ipynb

### Input Files
- wildfire/USGS_Wildland_Fire_Combined_Dataset.json (not inlcuded due to size. Link can be found in the main notebook). The format of this file is extremely complicated, it is a series of nested json objects.
- tourist_data.csv (Used for part 2 analysis). Columns: year (int), tourists (int, sum of overnight-visit and day-visit), overnight-visit (int, number of single day visitors), day-visit (int, number of multiday visitors). 

### Output Data Files: (These are files that are used to load data from so we don't have to call the API's over and over again)
- parsed_data.csv (Contains wildfire data). Columns: id (int), year (int), size (int, acres of fire), distance(int, distance from Savannah, GA).
- parsed_aqi_data.csv (Contains aqi data). Columns: year (int), aqi (int, air quality estimate).

## Project Reflection and Extra Details
The project reflection, project slide deck, and final project report can be found in the PDF file located in the Presentation and Summary folder!
