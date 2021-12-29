---
title: "Part 2: Evaluating Accessibility to Hurricane Evacuation Centers"
date: 2021-12-20
published: true
tags: [dataviz, altair, hvplot, osmnx]
excerpt: "Analyzing walking accessibility to hurricane evacuation centers using NYC's street network."
#altair-loader:
#  altair-chart-1: "charts/zones_centers_map.json"
hv-loader:
  points_hvplot_access_map: ["charts/points_hvplot_access_map.html", "800"] # second argument is the height
toc: false
toc_sticky: false
classes: wide
---

## Defining the Urban Street Network
The walkable road network for all of NYC is massive - this image is an export of the output from [OSMnx](https://osmnx.readthedocs.io/en/stable/) showing all walkable paths.

![G_NYC_roadnetwork]({{ site.url }}{{ site.baseurl }}/assets/images/G_NYC_roadnetwork_v2.png)

## Investigating Walking Accessibility to Nearest Evacuation Center
This static map to illustrates the distance of each node to the nearest center the map (shown in red). The maximum distance for this network analysis was set to 2000 meters (every node beyond 2000 meters is color-coded in the same purple hue, indicating relative inaccessibility).

![points_matplotlib_access_map]({{ site.url }}{{ site.baseurl }}/assets/images/points_matplotlib_access_map.png)

The interactive version of this accessibility surface is below (note: it is slow to load). Hurricane evacuation center points are not shown on this version, but they can be inferred based on the patterns of the colors going from darker to lighter.

<div id="points_hvplot_access_map"></div>
