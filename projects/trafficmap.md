---
layout: project
type: project
image: img/trafficmap2.png
title: "Traffic Map"
date: 2020
published: true
labels:
  - Python
summary: "I developed a program that creates a map with markers for all the traffic collisions from the input file."
---

Traffic Map is a program that asks the user for the name of a CSV file, name of the output file, and creates a map with markers for all the traffic collisions from the input file. It uses collision data collected and made publicly by a state, such as New York City Open Data. I worked on this individually as part of a CS class assignment and got to learn how to write programs that map GIS data using Turtles and Folium packages.

<div class="text-center p-4">
  <img width="300px" src="../img/traffic.png" class="img-thumbnail" >
  <img width="300px" src="../img/trafficmap3.png" class="img-thumbnail" >
</div>

Here is a sample of my code:

```cpp
import folium
import pandas as pd

cuny = pd.read_csv('cunyLocations.csv')
print(cuny["Campus"])

mapCUNY = folium.Map(location=[40.768731, -73.964915])
for index,row in cuny.iterrows():
    lat = row["Latitude"]
    lon = row["Longitude"]
    name = row["Campus"]
    newMarker = folium.Marker([lat, lon], popup=name)
    newMarker.add_to(mapCUNY)
mapCUNY.save(outfile='cunyLocations.html')
```

