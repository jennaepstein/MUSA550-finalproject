---
title: "Accessibility to Nearest Evacuation Center"
date: 2021-12-20
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Exploring the urban street network and walking accessibility to nearest evacuation centers."
#altair-loader:
#  altair-chart-1: "charts/zones_centers_map.json"
hv-loader:
  points_hvplot_access_map: ["charts/points_hvplot_access_map.html", "800"] # second argument is the height
toc: false
toc_sticky: false
classes: wide
---
## Process 
The second part of this project involved creating a network analysis to explore walking access to evacuation centers from each intersection. Main steps included:
* Creating a pandanas network
* Loading data for the walkable street network using OSMnx and adding locations of the hurricane evacuation centers to the network
* Plotting the walking distance to the nearest center

## Defining the Urban Street Network
The walkable road network for all of NYC is massive - this image is an export of the output from OSMnx showing all walkable paths.

![G_NYC_roadnetwork]({{ site.url }}{{ site.baseurl }}/assets/images/G_NYC_roadnetwork_v2.png)
<img src="G_NYC_roadnetwork_v2.png" height="300">


## Investigating Walking Accessibility to Nearest Evacuation Center
This static map to illustrates the distance of each node to the nearest center the map (shown in red). The maximum distance for this network analysis was set to 2000 meters (every node beyond 2000 meters is color-coded in the same purple hue, indicating relative inaccessibility).

![points_matplotlib_access_map]({{ site.url }}{{ site.baseurl }}/assets/images/points_matplotlib_access_map.png)

The interactive version of this accessibility surface is below (note: it is slow to load).
<div id="points_hvplot_access_map"></div>
