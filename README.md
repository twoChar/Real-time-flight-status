# flight-tracker-reactjs
A reactjs website that displays current flying planes on a map, showing details about each flight.

## Features

 Display current fetched flights on a map, ability to filter aircraft on map by call sign, you can hover on an aircraft to view the Call sign (If available), or click on it to view information about the fligh.


 You can click "View flight" to display live flight path on the map, which auto refreshes every 10 seconds. if you want it to refresh more often, go to the file src\pages\Flight\FlightInfo.jsx ,  and at line 318: 


Information about airports.


## Packages used

1- react-router

2- react-leaflet

## Other resources and APIs used

1- The app uses [OpenSky Network API](https://opensky-network.org/) for information about flights to be displayed on the map. OpenSky network API has request limitations of 100 API requests per day for anonymous users or 1000 API requests per day for registered users.

2- The app uses [hexdb.io API](https://hexdb.io/) for information about Aircraft, call signs, and airports.

3- The app uses [Country Flags API](https://countryflagsapi.com) for flag images.

4- The app retreives most recent available image of aircraft from [JetPhotos](http://jetphotos.com/). Link is retreived from [hexdb.io API](https://hexdb.io/).

5-The app uses [LeafletJs](https://leafletjs.com/) with [OpenStreetMap](https://www.openstreetmap.org/) for the map.


## How to run project

1- Clone this repository, and in the terminal, run:
### `npm install`

2- run : python backend/insert_data.py
  then run: python backend/app.py
  
3- Use another terminal and run: cd ./frontend 
and then run:

### `npm start`

Runs the app in the development mode.\



