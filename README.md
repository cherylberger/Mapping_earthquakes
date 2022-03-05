# Mapping_earthquakes
### Module 13 Data Analytics - Mapping Json data using JavaScript and HTML
### Cheryl Berger

## Project Overview: 
Basil and Sadhana like how you created your earthquake map with two different maps and the earthquake overlay. Now, Basil and Sadhana would like to see the earthquake data in relation to the tectonic plates’ location on the earth, and they would like to see all the earthquakes with a magnitude greater than 4.5 on the map, and they would like to see the data on a third map.

## Results:

### Resources: 

https://github.com/cherylberger/Mapping_earthquakes/blob/main/Earthquake_Challenge/major_eq_starter_logic.js
https://github.com/cherylberger/Mapping_earthquakes/blob/main/Earthquake_Challenge/tectonic_plate_starter_logic.js
https://github.com/cherylberger/Mapping_earthquakes/blob/main/Earthquake_Challenge/static/css/style.css


#### Modify the starter code provided to perform the following actions: 
![image](https://user-images.githubusercontent.com/94234511/155920313-dc5224dd-d412-4435-986a-a59de16a849f.png)

#### Setup the file folders as follows: 

![image](https://user-images.githubusercontent.com/94234511/155920562-f2b38cdc-46fb-41f5-abb9-df8ebf6a053d.png)

![image](https://user-images.githubusercontent.com/94234511/156896864-ee40283f-556e-485b-a85f-8c61a83f310c.png)


#### Add API key to the config.js file and add the config.js file to the .gitignore file in the GitHub repo to protect the security of the API key

1)  Register for a MapBox Acct and create an API key.

2) Create a new file in VS Code and name is config and save as JavaScript.  

3) Add the following code to the config. file.  
// API key
const API_KEY = "";

4) Copy and Paste the API key from MapBox between the "" in the API key variable. 

#### The code for the challenge_logic1.js https://github.com/cherylberger/Mapping_earthquakes/blob/main/Earthquake_Challenge/static/js/challenge_logic1.js is detailed below as edited in Visual Studio Code: 

![image](https://user-images.githubusercontent.com/94234511/155921298-22c53a7f-8ba6-4b40-94f7-6c8eb94a5186.png)

![image](https://user-images.githubusercontent.com/94234511/155921371-29cb828f-9a48-4280-8414-9f7c68a4ce58.png)

![image](https://user-images.githubusercontent.com/94234511/156896791-1c67a1f0-233b-4f07-942a-7bd1ab4fdf8b.png)

![image](https://user-images.githubusercontent.com/94234511/156896808-1c46f1d3-50d8-4c93-8cd2-97c3193d211c.png)

#### The code for the index.html file (https://github.com/cherylberger/Mapping_earthquakes/blob/main/Earthquake_Challenge/index.html) that can be used to open the map in a webbrowser on localhost:8000

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta http-equiv="Access-Control-Allow-Origin" content="*">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mapping_GeoJSON_Data_Tplates</title>
    <!-- Add the code for the Leaflet CSS file to the head section of the document -->
    <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
        integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
        crossorigin="" />
    <!-- d3 JavaScript -->
    <script src="https://d3js.org/d3.v5.min.js"></script>
    <!-- Our CSS -->
    <link rel="stylesheet" type="text/css" href="static/css/style.css">

</head>

<body>
    <!-- The div that holds our map (note the plaement of this code for the location of the map) -->
    <div id="mapid"></div>

    <!-- Leaflet JavaScript code - always add after the Leaflet CSS file-->
    <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
        integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
        crossorigin=""></script>
    <!-- API key -->
    <script type="text/javascript" src="static/js/config.js"></script>
    <!-- Our JavaScript -->
    <script type="text/javascript" src="static/js/challenge_logic.js"></script>
</body>

</html>

![image](https://user-images.githubusercontent.com/94234511/155922879-bcbf2b40-307f-4e54-b121-f1ca723e4b58.png)

### Deliverable 1 Add Tectonic Plate Data
The tectonic plates are added to the map showing all earthquakes.
![Tectonic Plates](https://user-images.githubusercontent.com/94234511/155921052-d3b086bc-51d7-49ed-8e64-8aec90f51e3c.png)


### Deliverable 2:  Add Major Earthquake Data
After calling the data for earthquakes greater than mag 4.5, we add the functions to change the style of the map features to reflect mag >5 as orange and >6 in red. 
![image](https://user-images.githubusercontent.com/94234511/156896660-c1a6dfce-7837-43a7-85d3-c7bf383b870a.png)

If all layers are present the map will look as follows on streetview. 
![Major Earthquakes_streetview](https://user-images.githubusercontent.com/94234511/156896511-a494ba4b-aaf0-48cf-9180-81780d9de49e.png)

### Deliverable 3: Add an Additional Map
A dark map was added to the code with the sattelite view. The data for either all earthquakes or both the all earthquakes or major earthquakes layers can be applied.  The dark map view makes the colors standout for slightly improved visualization over the street or satellite views. 
![Darkmap_all layers](https://user-images.githubusercontent.com/94234511/156896490-15485060-345b-4ee1-99d5-9ef91877d8ed.png)

![Darkmap_Major Earthquakes only](https://user-images.githubusercontent.com/94234511/156896495-2f6fe96e-d9ae-4dde-97bb-3160ed8d7350.png)



