# Python API Challenge

## Overview
In this project, Python requests, APIs, and JSON are leveraged to answer a fundamental question: "What is the weather like as we approach the equator?" While the immediate answer might be "It gets hotter," this project delves deeper into analyzing weather data from over 500 cities to provide more insights.

## Part 1: WeatherPy
WeatherPy involves creating a Python script to visualize the weather of over 500 cities of varying distances from the equator. The following steps are undertaken:
- Generate random geographic coordinates and find the nearest city to each latitude and longitude combination using the citipy Python library.
- Retrieve weather data for each city using the OpenWeatherMap API.
- Create a series of scatter plots to display relationships like Latitude vs. Temperature, Humidity, Cloudiness, and Wind Speed.
- Separate the plots into Northern and Southern hemispheres, calculating linear regression for each to understand weather changes based on proximity to the equator.

## Part 2: VacationPy
VacationPy showcases how weather data can be used to plan future vacations, utilizing the Geoapify API and the geoViews Python library. The following steps are involved:
- Create a map displaying a point for every city in the city_data_df DataFrame, with the size of the point indicating humidity.
- Narrow down the city_data_df DataFrame to find cities meeting specific weather conditions.
- Create a new DataFrame called hotel_df to store city, country, coordinates, and humidity.
- Use the Geoapify API to find the first hotel located within 10,000 meters of coordinates for each city.
- Add hotel name and country as additional information in the hover message for each city on the map.

## User Guide
1. Run `WeatherPy.ipynb` to collect and store weather data from approximately 550-650 cities worldwide using randomly generated coordinates. API keys will be required for Geoapify and OpenWeatherMap.
2. Graphs created by `WeatherPy.ipynb` will be stored in `output_data`.
3. `VacationPy.ipynb` can be run after `WeatherPy.ipynb` as it is dependent on the data collected by the latter.

## References
- [citipy Python library](https://pypi.org/project/citipy/)
- [OpenWeatherMap API](https://openweathermap.org/api)
- [Geoapify API](https://www.geoapify.com/)
- [geoViews Python library](https://geoviews.org/)
