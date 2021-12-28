---
title: "Part 3: Mapping the Elements Together"
date: 2021-12-19
published: true
tags: [dataviz, folium]
excerpt: "An interactive folium map allowing users to explore the different elements of this analysis and inform resource allocation decisions."
folium-loader:
  folium_map_master: ["charts/folium_map_master.html", "800", "800"]
toc: false
toc_sticky: false
classes: wide
---
This final map allows the user to explore the different facets of this analysis. By default, the map loads with the following layers (which can be toggled on/off using radio buttons in the layer control):
* Highest risk hurricane evacuation zone (zone 1), shown as red polygons
- Road inaccessibility during and after a hurricane will impact evacuations, so the additional overlay of hurricane evacuation zone 1 (the highest risk of flooding) as an additional overlay shows what pockets of the city will be impacted from inundation. 
* Most accessible nodes for reaching an evacuation center, shown as black points
- For the purposes of this analysis, I defined "walkability" as indicative of a reasonable distance to walk when faced with imminent danger from a hurricane. I filtered the accessibility data to include nodes only within a half mile (approximately 804.672 meters) from the nearest evacuation center. Those nodes outside of this range would be more difficult to access, esepcailly when racing against an incoming storm.

The user can also enable overlay layers for population density and social vulnerability scores by census tracts. The overal flexibility of layer control allows the user to explore different scenario to see which areas of the city may be impacted differently when faced wtih a hurricane evacuation need. For instance, areas with census tracts of higher population density and/or higher social vulnerability that also sit in or near pockets at high hurricane risk AND lack accessibility to centers may be best sutied for city personnel to prioritize citing new centers. This map is thys an effective plannign tool for identifing areas at greatest need of support when it comes to allocating resources, especially as climate change continues to exacerbate extreme precipitation events.
<div id="folium_map_master"></div>
