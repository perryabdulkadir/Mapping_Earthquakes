# Mapping Earthquakes
Interactive map app that displays earthquake data in real-time

## Overview of Analysis
In this project, I used Javascript, HTML, CSS, and Leaflet.js to create a map that displays earthquake data. The map has multiple layers of data that can be toggled on or off by the user: tectonic plate lines, all earthquakes, and major earthquakes. The user can also select a satellite map, street map, or dark mode app. 

### Resources
Software/Languages: Javascript, HTML, CSS, Mapbox Styles API

Javascript libraries: Leaflet.js


## Building the App

### Adding Tectonic Plate Data
The first portion of our Javascript code prepares the three base layers that will be used. 

![background_tiles.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/background_tiles.png)

Next, I added a second layer group variable for the tectonic plate data before adding a reference to the tectonic plate data to the overlay object.

![layer_group_variable.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/layer_group_variable.png)

After this, I used the d3.json() function to call to the tectonic plate data hosted by Github user fraxen [here](https://github.com/fraxen/tectonicplates).
Nested within the d3.json callback, the function styleInfo is used to set the size and color of earthquakes based on their magnitude. 


![styleInfo.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/styleInfo.png)

The functions getColor and getRadius are, in turn, used by styleInfo. 

![get_color_get_radius.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/get_color_get_radius.png)

I then placed the markers on the map.

![markers1.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/markers1.png)

Finally, I created a legend.

![legend1.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/legend1.png)

That yields a map that looks like this.

![map1.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/map1.png)


### Adding Major Earthquake Data

The process of creating a map layer with only severe earthquake data (Richter >4) is a simple matter of refactoring the code above. Almost everything remains the same except the getColor and getRadius functions.

![get_color2.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/get_color2.png)

When only the major earthquakes layer is selected, this is the resulting map.

![map2.PNG](https://github.com/perryabdulkadir/Mapping_Earthquakes/blob/main/Resources/map2.png)



## Summary
This method can be used to quickly create interactive maps with multiple layers that update in real-time.


-----

### **Contact:**

**Email:** perry.abdulkadir@alumni.harvard.edu

**Linkedin:** https://www.linkedin.com/in/perry-abdulkadir-6a255199/
