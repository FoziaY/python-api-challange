# Python API Challenge: WeatherPy and VacationPy

<img src="https://sinay.ai/wp-content/uploads/2022/09/api-e1649279794668-scaled.webp" alt="WeatherPy and VacationPy" style="width: 100%; height: auto;">

***
## Background
This project explores the relationship between weather conditions and geographical location, particularly the latitude. It utilizes various APIs and Python libraries to gather, analyze, and visualize weather data from over 500 cities. The project is divided into two main parts: WeatherPy and VacationPy.

***

## Instructions
### Part 1: WeatherPy
In this part, we visualize the weather of over 500 cities across the world using the OpenWeatherMap API and the citipy Python library.

#### Steps
1. **Generate Cities List**: Use random geographic coordinates to create a list of cities.
2. **Retrieve Weather Data**: Use the OpenWeatherMap API to get the weather data for each city.
3. **Create Scatter Plots**: Generate scatter plots to showcase the following relationships:
   - Latitude vs. Temperature
   - Latitude vs. Humidity
   - Latitude vs. Cloudiness
   - Latitude vs. Wind Speed
4. **Compute Linear Regression**: Compute linear regression for each relationship, separating the plots into the Northern and Southern Hemispheres.

<img src="https://static.bc-edx.com/data/dl-1-2/m6/lms/img/linear-regression-plot.png" alt="inear-regression-plot.png" style="width: 100%; height: auto;">

#### Outputs
- **Latitude vs. Temperature**
- **Latitude vs. Humidity**
- **Latitude vs. Cloudiness**
- **Latitude vs. Wind Speed**

### Part 2: VacationPy
In this part, we use the weather data to plan future vacations, using the Geoapify API and the geoViews Python library to create map visualizations.

#### Steps
1. **Load Weather Data**: Load the weather data from Part 1.
2. **Create Humidity Map**: Display a map with a point for every city, where the size of the point is determined by the humidity.
3. **Narrow Down Ideal Conditions**: Filter cities based on ideal weather conditions.
4. **Find Hotels**: Use the Geoapify API to find the first hotel within 10,000 meters of each city's coordinates.
5. **Create Hotel Map**: Add hotel names and countries as additional information in the hover message for each city on the map.

#### Outputs
- **Humidity Map**
- **Hotel Map**

***

## Requirements
### Part 1: WeatherPy
- **Create Plots to Showcase the Relationship Between Weather Variables and Latitude** (30 points)
  - Use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code (10 points)
  - Create scatter plots to showcase various relationships (20 points)
- **Compute Linear Regression for Each Relationship** (40 points)
  - Create linear regression scatter plots for the Northern and Southern Hemispheres for each variable (40 points)

### Part 2: VacationPy
- **Create a Humidity Map** (5 points)
- **Narrow Down Ideal Conditions** (5 points)
- **Find Hotels Using Geoapify API** (10 points)
- **Create Hotel Map** (10 points)

***

## Results
### WeatherPy
The scatter plots reveal the following trends:
1. **Latitude vs. Temperature**: Temperature increases as one approaches the equator (0° latitude), confirming the general expectation that it gets hotter near the equator.
2. **Latitude vs. Humidity**: Humidity does not show a strong correlation with latitude.
3. **Latitude vs. Cloudiness**: Cloudiness varies widely at all latitudes, showing no significant pattern.
4. **Latitude vs. Wind Speed**: Wind speed does not show a strong correlation with latitude.

<img src="https://static.bc-edx.com/data/dl-1-2/m6/lms/img/humidity_map.png" alt="humidity_map.png" style="width: 100%; height: auto;">

### VacationPy
Using the weather data, ideal vacation cities were selected based on criteria such as moderate temperatures, low wind speeds, and clear skies. Hotels near these ideal cities were located using the Geoapify API, and maps were created to visualize these vacation spots.

***

## Usage
To run the analysis:
1. Clone the repository to your local machine.
2. Ensure you have the required libraries installed: `pandas`, `numpy`, `matplotlib`, `requests`, `scipy`, `geopandas`, `geoViews`, `Geoapify`.
3. Add your API keys to the `api_keys.py` file.
4. Open the Jupyter notebooks (`WeatherPy.ipynb` and `VacationPy.ipynb`) and run the cells sequentially.

***
