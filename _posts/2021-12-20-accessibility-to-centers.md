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

## Defining the Urban Street Network

Show OSMnx road network for process?
![G_NYC_roadnetwork]({{ site.url }}{{ site.baseurl }}/assets/images/G_NYC_roadnetwork.png)


## HvPlot of Walking Accessibility to Nearest Evacuation Center

Text describing the map:

<div id="points_hvplot_access_map"></div>
lse