# python-api-challenge

Python API Challenge

Project Overview

The Python API Challenge explores weather patterns as we approach the equator by analyzing over 500 cities across the globe. The project leverages Python, APIs, and JSON traversals to retrieve and visualize weather data, as well as plan ideal vacation destinations based on weather conditions.

This challenge consists of two parts:

WeatherPy: Analyze and visualize the relationship between latitude and various weather parameters.

VacationPy: Use weather data to identify ideal vacation locations and display hotel information.

Tools and Technologies

Python Libraries:

pandas

matplotlib

requests

json

numpy

scipy.stats

geoviews

citipy

APIs:

OpenWeatherMap

Geoapify

Other Tools:

Jupyter Notebook

Git/GitHub

Instructions

Part 1: WeatherPy

Objective

Visualize weather conditions of 500+ cities to analyze their relationships with latitude.

Process

Retrieve Weather Data:

Use the OpenWeatherMap API to collect weather data for randomly selected cities using the citipy library.

Visualizations:

Create scatter plots for:

Latitude vs. Temperature

Latitude vs. Humidity

Latitude vs. Cloudiness

Latitude vs. Wind Speed

Linear Regression:

Compute and display linear regression for:

Northern and Southern Hemispheres:

Temperature vs. Latitude

Humidity vs. Latitude

Cloudiness vs. Latitude

Wind Speed vs. Latitude

Analysis:

Interpret the relationship between latitude and weather variables for each hemisphere.

Part 2: VacationPy

Objective

Plan vacation locations based on ideal weather conditions and display nearby hotels.

Process

Humidity Map:

Visualize city locations with point sizes representing humidity.

Filter Ideal Locations:

Narrow down cities with desired weather conditions:

Temperature: 21°C to 27°C

Wind Speed: < 4.5 m/s

Cloudiness: 0%

Hotel Search:

Use the Geoapify API to find the nearest hotel within 10,000 meters of each city.

Save results to a new DataFrame with city, country, coordinates, humidity, and hotel name.

Vacation Map:

Create an interactive map displaying hotel information in hover messages.

Results and Insights

WeatherPy:

Scatter plots demonstrate clear relationships between latitude and weather variables.

Linear regression highlights patterns specific to each hemisphere.

VacationPy:

Identified ideal vacation locations based on weather preferences.

Visualized hotels and weather conditions on an interactive map.

Repository Structure

python-api-challenge/
|
├── WeatherPy/
│   ├── WeatherPy.ipynb
│   ├── city_data.csv
│   └── api_keys.py (excluded via .gitignore)
│
├── VacationPy/
│   ├── VacationPy.ipynb
│   └── output_data.csv
│
├── .gitignore
├── README.md
└── requirements.txt

How to Run

Clone the repository:

git clone <repository_url>

Install required libraries:

pip install -r requirements.txt

Add your API keys to api_keys.py.

Open Jupyter Notebook:

jupyter notebook

Navigate to WeatherPy.ipynb and VacationPy.ipynb to execute the analysis.

Author

Emeka Michael Osasah

License

This project is licensed under the MIT License. See the LICENSE file for details.

