---
title: "Part 3: Mapping the Elements Together"
date: 2021-12-19
published: true
tags: [dataviz, folium, map]
excerpt: "An interactive folium map allowing users to explore the different elements of this analysis and inform resource allocation decisions."
folium-loader:
  folium_map_final: ["charts/folium_map_final.html", "800", "800"]
toc: false
toc_sticky: false
classes: wide
---
This final map allows the user to explore the different facets of this analysis. By default, the map loads with the following layers (which can be toggled on/off using radio buttons in the layer control):
* Highest risk **hurricane evacuation zone** (zone 1), shown as red polygons
  - Road inaccessibility during and after a hurricane will impact evacuations. The additional overlay of hurricane evacuation zone 1 (the highest risk of flooding) shows what pockets of the city will be most impacted from inundation. 
* **Most accessible nodes - 1/2 mile)** refers to nodes within a half mile walk of an evacuation center
  - For the purposes of this analysis, I defined "walkability" as indicative of a reasonable distance to walk when faced with imminent danger from a hurricane. I filtered the accessibility data to include nodes only within a half mile (approximately 804.672 meters) from the nearest evacuation center. Those nodes outside of this range would be more difficult to access, especially when racing against an incoming storm.

The user can also enable overlay layers for the following:
* **Population Density (normalized)** by Census tract
  - To enable the choropleth color scale, I normalized the `population_density` variable to be a scale from 0-1
* **Overall Social Vulnerability Index** by Census tract

<div id="folium_map_final"></div>

The flexibility of layer control allows the user to explore different scenarios to see which areas of the city may be impacted differently when faced with a hurricane evacuation need. For instance, areas with census tracts of higher population density and/or higher social vulnerability that also sit in or near pockets at high hurricane risk *and* limited accessibility to centers may be best suited for city personnel to prioritize opening new centers. This map is thus an effective planning tool for identifying areas at greatest need of support when it comes to allocating resources, especially as climate change continues to exacerbate extreme precipitation events.

## Back to [Project Landing Page](https://jennaepstein.github.io/MUSA550-finalproject/)

