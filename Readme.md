# Open Street Map(OSM) Mapper
OSM Mapper presents a graphical and interactive map application that retrieves and displays OSM data such as streets and intersections of various cities. This application is developed in C++ language in linux environment.

## Main Screen
![Alt text](/screenshots/startingscreen.png?raw=true)
![Alt text](/screenshots/intersection.png?raw=true)
The main screen shows all streets of a chosen city, and displays intersection information when it is clicked by mouse.

## Finding Shortest Path
![Alt text](/screenshots/pathfinding.png?raw=true)

When two intersections are clicked, the application computes and displays the shortest path between those two intersections. The path-finding mechanism is based on A* search algorithm. 


## Finding Pickup Route
![Alt text](/screenshots/walkdrive_visual.png?raw=true)
![Alt text](/screenshots/walkdrive_instruction.png?raw=true)

Analogous to Uber application, the mapper displays both visual route and instruction when two intersections are pressed. The route consists of a walking path of a passenger and driving path of a driver.


## Displaying Weather Data
![Alt text](/screenshots/weatherinfo.png?raw=true)

Weather information is retrieved online from from DarkSky API, and displays it to the user through the terminal. The JSON data was retrieved using libcurl library.

## Finding an Intersection
![Alt text](/screenshots/findintersection1.png?raw=true)
![Alt text](/screenshots/findintersection2.png?raw=true)

An intersection can be found by typing in two intersection, where the possible name of intersections are auto-completed while typing.

## Changing Cities
![Alt text](/screenshots/cityload2.png?raw=true)

This application works not only in Toronto(the default location), but various cities as long as the OSM data is provided!

## Credit
Most API used in this application is developed by the ECE297 team in University of Toronto. The APIs include:
- StreetDataBase: used for retrieving high-level map data(e.g. streets and intersections)
- OSMDatabase: used for retrieving low-level OSM data(e.g. OSM node)
- EZGL: used for creating graphical user interface(GUI)
- and many others
