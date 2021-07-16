# Mapping Earthquakes


## Overview of Analysis


### Resources
Software/Languages: Javascript, HTML, CSS

Javascript libraries: Leaflet.js

APIs: 

## Building the App

### Adding Tectonic Plate Data
The first portion of our Javascript code prepares the three base layers that will be used. 

![background_tiles.PNG](Resources/background_tiles.PNG)

Next, I added a second layer group variable for the tectonic plate data before adding a reference to the tectonic plate data to the overlay object.

![layer_group_variable.PNG](Resources/layer_group_variable.PNG)

After this, I used the d3.json() function to call to the tectonic plate data hosted by Github user fraxen [here](https://github.com/fraxen/tectonicplates).
Nested within the d3.json callback, the function styleInfo is used to set the size and color of earthquakes based on their magnitude. 


![styleInfo.PNG](Resources/styleInfo.PNG)

### Adding Major Earthquake Data


### Adding an Additional Map Style




## Summary



-----

### **Contact:**

**Email:** perry.abdulkadir@alumni.harvard.edu

**Linkedin:** https://www.linkedin.com/in/perry-abdulkadir-6a255199/
