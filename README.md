# Lab 5: Web-scraping Weather Data with Python
### Date Due: 09/27/2019

In this lab, you will work with a script that extracts live weather conditions from the National Weather Service website for a given location in the United States. 

1. Copy the **NWS_CurWeatherConditions.py** file and paste it into the online Python compiler: https://repl.it/languages/python
   
   Make sure you are using Python version 2.7. You can check the Python version in the compiler window on the right. 

2. Read the the description and comments in the script to understand the purpose of the script

3. Run the scipt. You will see some packages being installed in the compiler window when you run it for the first time.

![Library Installation](/images/loadlib.PNG)

The script returns the current weather conditions for Worcester, MA (Lat: 42.2634, Lon: -71.8022) with the latitude and longitude information provided in the script. Using the latitude and longitude values, it generates the following URL through string concatenation: https://forecast.weather.gov/MapClick.php?lat=42.2634&lon=-71.8022 

4. Open this URL in a firefox or chrome web browser. Locate the information that is being outputted in our script. Right click on this and and select the Inspect Element option. 
![Inspect Element](/images/inspectelement.PNG)

This will launch the Inspector window that helps locate different elements on the page. 
![Inspect Element](/images/inspectelement_window.PNG )

5. Locate the current_conditions-summary 'id' tag on the page.
    
## Edit the NWS_CurWeatherConditions.py script to do the following:

- Edit the lat and lon variables with latitude and longitude (in decimal degrees) for a city of your choice. Note that the city must be located in the United States. If latitude/longitude for a city that is outside the U.S. is specified, the page will return an error. You can find the latitude and longitude for a place of interest through this online geocoder: https://www.latlong.net/ 

- In the web-page, find the 'id' element that contains the Humidity, Wind Speed, Barometer, Dewpoint, Visibility and Last Updated information. Edit line #35 in the script to scrape this 'id' element.
   The final output for the script should include the Humidity, Wind Speed, Barometer, Dewpoint, Visibility and Last Updated information for the selected city.

Submit your script via Github. Clicking this link will create a private repository for you with instructions on how to edit the README file and your script: https://classroom.github.com/a/ZAYyyPBH
Remember to update the existing header in the Labcode.py file. Be sure to include comments and documentation in your script to tell me what it’s doing!
