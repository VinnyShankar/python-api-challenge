# python-api-challenge
### - Overview
- Module 6 Python API Challenge files
- Author: Vinny Shankar
- Acknowledgements:
    - Study Groups: worked together with several students to understand the assignment
    - Classmates: Jed Miller and Hany Dief were instrumental in getting the api url's working properly; Worked with Jesús Jiménez to understand the WeatherPy part of the assignment
    - Starter Code: the challenge gave us starter code which let us fill in the gaps in order to reach the desired outputs
    - Program: University of California Berkeley Data Analytics Bootcamp
### - Contents
- One folder containing:
    * WeatherPy Jupyter Notebook
    * VacationPy Jupyter Notebook
    * output_data folder containing:
        * CSV with list of cities generated by WeatherPy
        * Scatter plot images generated by WeatherPy
- .gitignore file
- This README.md file
### - Description:
- The WeatherPy Jupyter script does the following:
####
    - Randomly generates 1500 pairs of Latitude and Longitude coordinates
    - Uses citipy to get the name of the nearest city for each coordinate pair
    - Uses the OpenWeatherMap API to get weather data for those cities and exports a .csv to the output_data folder
    - Creates scatter plots of Latitude vs. the other weather metrics and exports them as images to the output_data folder
    - Splits the data up by Northern and Southern hemisphere
    - Creates regression scatter plots for latitude vs. each weather metric for each of the two hemispheres
    - Discusses the strength of the linear relationship in each regression scatter plot
- The VacationPy Jupyter script does the following:
####
    - Uses the hvplot module and the .csv generated by WeatherPy to plot each city onto map
    - Filters the city data using ideal vacation weather conditions and generates a list of vacation cities
    - Uses the Geoapify API to find the nearest hotel to each vacation city
    - Drops cities where no hotel was found
    - Uses the hvplot module to plot the remaining cities onto a map
    - Adds the hotel name and country to the hover message for each city on the map

