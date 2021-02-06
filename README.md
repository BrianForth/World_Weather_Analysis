# World_Weather_Analysis
This project takes random latitude-longitude pairs and used them to offer the user a selection of cities and hotels therein based on daily high temperatures. 

## Weather_Database

The first file takes 2000 pairs of random lat-lon values, and finds the closest city of at least 500 people to that location. If this location is not already on the list, it is added to the list. Through an API to openweather, the weather for these unique locations is sent to a CSV to be used by the next file.

## Vacation Search

This file takes the CSV created by the previous file and takes input from the user to establish a temperature range for the cities. It then finds hotels in the eligible cities. With the new information, it pulls from the google maps API to create a map of all remaining cities that fall within the temperature and hotel criteria. The map and data frame of cities are then saved to the folder.

## Vacation Itinerary

This file takes the CSV from the previous file and takes the four cities on New Zealand's North Island from the original list that also met the necessary criteria. It then pulls from the google maps API to establish driving directions between the four cities to establish an itinerary for a hypothetical vacation in the area.