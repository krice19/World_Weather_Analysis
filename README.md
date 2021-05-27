# World_Weather_Analysis

The purpose of this project is to gather weather data from coordinates and create maps through google API calls to help customers retrieve infomation regarding traveling.  

## Using Open Weather API
In the first deliverble, I generated a random set of 2000 latitudes and longitudes.  From these coordinates, I found the closest city and perforrrmed an API call with OpenWeatherMap.  I retieved the city, country, coordinates, maximum temperature, humidity, cloudiness, wind speed, and weather description.  I put this new data into a dataframe and exported it into a CSV file.

## Using GMAPS and Google Place API Seach

In the second deliverable, I first  started by pulling my csv file from Deliverable 1 into the notebook.  I promoted the user to enter a min and max temperate and created a new dataframe based off these preferences. After cleaning the data, I created a new empty column in the data frame called "Hotel Name".  I lopped through the coordinates and performed a Google API call to get the closest lodding to that city.  From this, was able to create a map all all the different cities with information stored in info box format.  

## Using GMAPS and Google Directions API Search

In my last deliverable, I used my dataframe created in deliverable 2 temperature preferenced cities.  I choose 4 cities from that map, and created a direction layered map to create a travel interary.  I did this using the gmaps direction layer and adding three different stops are waypoints. After the directions  were completed, I put these four cities in their own dataframe and created another map with info box info regarding weather and closest hotels.