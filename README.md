# city_weather_data

I've created a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, I utilized a simple Python library [citipy](https://pypi.python.org/pypi/citipy) and the [OpenWeatherMap API](https://openweathermap.org/api) to create a representative model of weather across world cities.

## Selecting the cities
To generate a random list of cities, we first generate 1000 random lattitude-longitude combinations and use the .nearest_city() function of the citipy library to find the nearest city and creating a list from the unique city names.

## Collecting the weather data
We use the OpenWeatherMap API to collect data about today's weather for each city: `lattitude`, `longitude`, `temperature`, `cloudiness`, `humidity`, and `wind speed`.  A dataframe was then created and exported it to `cityWeather.csv`.


## Scatter Plots
* Temperature (F) vs. Latitude

