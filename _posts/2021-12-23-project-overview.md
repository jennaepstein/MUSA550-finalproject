---
title: "Project Overview"
date: 2021-12-23
excerpt: "An overview of the project motivation and context."
altair-loader:
  zones_centers_map: "charts/zones_centers_map.json"
hv-loader:
  boros_hurricane_evac_centers_plot: ["charts/boros_hurricane_evac_centers_plot.html", "800", "800"] # second argument is the height
classes: wide
---
## Motivation
Over the past decade,  past decade has witnessed hurricanes and tropical storms have brought widespread damage and devastation to New York City. Major storm events and their impacts - particuiary when it comes to storm surge flooding - are only expected to increase in frequency as the planet warms. 

For my final project, I sought to explore hurricane vulnerability in NYC through the lenses of population density, social vulnerability, and hurricane evacuation center accessibility.

This analysis considers the following questions:
* What is the relationship between census-tract level population composition and proximity to hurricane
evacuation centers?
* Are centers in/near areas of high social vulnerability? What does walkability look like for these populations?
* What road networks in the event of major storm-related flooding will be impacted?

## Context
The map below shows an overview of hurricane evacuation centers across the five NYC boroughs and hurricane evacuation zones. There are six hurricane evacuation zones designated by the city and are ranked by the risk of storm surge impact. In the event of a hurricane or tropical storm, residents living in these zones may be told to evacuate ([Source] (https://www1.nyc.gov/assets/em/html/know-your-zone/knowyourzone.html)). Zone 1 is the most likely to flood and therefore at highest risk of storm surge impacts. Zone 6 is the least likely and therefore has the lowest risk of the zones.
<div id="zones_centers_map"></div>

When ordered to evacuate, NYC residents living within an evacuation zone can seek shelter at one of the City's hurricane evacuation centers - facilities across the City designated as shelters where residents temporarily stay and are processed before being transported to a hurricane shelter. These evacuation centers are critical for residents who do not have family or friends outside of the risk areas with which to stay, and for those who lack financial options for short-term stays outside of the high risk areas. 

Across the five boroughs, there are 60 evacuation centers (based on the most up-to-date data available through NYC's Open Data portal). The distribution across the boroughs is shown on this bar graph. Brooklyn and Queens currently have the most centers within their boundaries (17 and 16, respectively).
<div id="boros_hurricane_evac_centers_plot"></div>