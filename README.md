# WeatherPy - Weather and Mapping APIs

## Overview

This project utilized the following APIs for data collection and visualization:
* OpenWeatherMap API
* Google maps and NearbyPlaces APIs
* Google Directions API

New features:

* Weather description to be collected from weather data and displayed with destination information
* Allow the users to filter the list of destinations based on temperature preferences, and present this on a map.
* Build and display a travel itinerary with selected destinations.  Map the itinerary and provide the destination information on the map.

# Retrieve Weather Data
A set of 3000 random Latitude and Longitude combinations was constructed to provide search data which was consumed by cityPy to try to locate nearby cities.  The located cities became the potential destinations for the PlanMyTrip users. Using the identified cities, the OpenWeatherMap API was used to retrieve the city weather data.

The cities and corresponding weather data was used to generate a world map with markers for all the cities.  Selecting a marker displays an info box with the city name, a hotel, and weather details.

![World Map with city markers](Vacation_Search/WeatherPy_vacation_map.png)


# Create a Travel Destinations Map

The users selected four city destinations in Japan.  A map of the selected destinations was created with city markers and an info box to provide details.

![Travel Destinations](Vacation_Itinerary/WeatherPy_travel_map_markers.png)

A driving itinerary was constructed using the Google Maps Directions API, using the preferred sequence for travel between the cities.

![Travel Destinations & Driving Itinerary](Vacation_Itinerary/WeatherPy_travel_map.png)
