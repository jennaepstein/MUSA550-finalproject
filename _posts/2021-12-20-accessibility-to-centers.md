---
title: "Accessibility to Nearest Evacuation Center"
date: 2021-12-20
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Embedding interactive charts on static pages using Jekyll."
altair-loader:
  altair-chart-1: "charts/zones_centers_map.json"
hv-loader:
  points_hvplot_access_map: ["charts/points_hvplot_access_map.html", "800", "800"] # second argument is the height
toc: true
toc_sticky: true
---

## Defining the Urban Street Network

Show OSMnx road network for process?
![G_NYC_roadnetwork]({{ site.url }}{{ site.baseurl }}/assets/images/distance_to_abandoned_cars.png)


## HvPlot of Walking Accessibility to Nearest Evacuation Center

Text describing the map:

<div id="points_hvplot_access_map"></div>
