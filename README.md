# Lab 2 Assignment - ENGO 651 (Advanced Geospatial Topics W22)

## Objectives

- Gain experience with Leaflet.js and GeoJSON.
- Learn to build a geoweb app by mashing up two APIs.

## Project Summary

The Lab 2 project task was to build a geoweb application using GeoJSON, Leaflet, and the City of Calgary's Open Calgary API to get building permit data that users are able to query by selecting date ranges. The building permit data will then be displayed using map icons and popups. All pertinent project data can be found in the "project" folder.

The main file is application.py which holds the app routes. The templates folder holds two files, index.html, the "Home" page with the map and search function, and layout.html, the foundation for index.html with all the stylesheets and scripts for the functionality of index.html.

### Application
The application.py file consists of an app route that takes users to the home page via index.html. Users will have to set certain environment variables in order for the program to run including:
- set FLASK_APP=application.py
- set FLASK_DEBUG=1
- the DATABASE_URL will have to be set to the provided, commented out, URI that can be found in the application.py file

Once the program is running the user can select two different dates by clicking on the calendar icon on the right of each input box or by manually entering the date with the given format. Once they click "Search", a number of icons will populate the map and as the user zooms in, clusters will turn into single icons that they can click on and read the building permit information from.
