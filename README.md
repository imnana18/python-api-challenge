# WeatherPy and VacationPy Project

In this project, we visualize weather data for over 500 cities using the OpenWeatherMap API and create map visualizations to plan future vacations. The project is divided into two parts: WeatherPy and VacationPy.

## Part 1: WeatherPy

### Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

In this part, we use the OpenWeatherMap API to retrieve weather data for cities and create scatter plots to showcase the following relationships:

- Latitude vs. Temperature
- Latitude vs. Humidity
- Latitude vs. Cloudiness
- Latitude vs. Wind Speed

### Requirement 2: Compute Linear Regression for Each Relationship

We compute linear regressions for each relationship and separate the plots into Northern and Southern Hemispheres. We create scatter plots with linear regression lines, model formulas, and r-values to visualize the relationships.

#### Sample Scatter Plot with Linear Regression Line
![Sample Scatter Plot](/output_data/northern_lat_vs_temp.png)

Plots Created:
- Northern Hemisphere: Temperature vs. Latitude
- Southern Hemisphere: Temperature vs. Latitude
- Northern Hemisphere: Humidity vs. Latitude
- Southern Hemisphere: Humidity vs. Latitude
- Northern Hemisphere: Cloudiness vs. Latitude
- Southern Hemisphere: Cloudiness vs. Latitude
- Northern Hemisphere: Wind Speed vs. Latitude
- Southern Hemisphere: Wind Speed vs. Latitude

### Part 2: VacationPy

In this part, we use weather data to plan future vacations. We create map visualizations and narrow down the city data to find ideal weather conditions. We also use the Geoapify API to find hotels near selected cities.

### Tasks Completed in VacationPy:

1. Created a map that displays points for every city in the city_data_df DataFrame, with point size representing humidity.

![Humidity Map](/output_data/a.png)

2. Narrowed down city_data_df to find ideal weather conditions, e.g., max temperature, wind speed, and cloudiness criteria.

3. Created a new DataFrame called hotel_df to store city, country, coordinates, humidity, and hotel information.

4. Used the Geoapify API to find the first hotel located within 10,000 meters of each city's coordinates.

5. Added hotel names and country information to the hover message for each city on the map.

## Usage

- Part 1 (WeatherPy) can be executed in the provided WeatherPy.ipynb Jupyter notebook.

- Part 2 (VacationPy) can be executed in the VacationPy.ipynb Jupyter notebook.

## Dependencies

The following dependencies were used in this project:

- Pandas
- Matplotlib
- Requests
- GeoViews
- Geoapify API

## Conclusion

This project provides insights into weather patterns in various cities and helps plan future vacations based on weather conditions. The combination of data visualization and the Geoapify API allows for better decision-making when selecting travel destinations.
