---
title: "Project Overview"
date: 2021-12-23
tags:
  - Overview
excerpt: "An overview of the project and context."

altair-loader:
  zones_centers_map: "charts/zones_centers_map.json"
hv-loader:
  boros_hurricane_evac_centers_plot: ["charts/boros_hurricane_evac_centers_plot.html", "800", "800"] # second argument is the height
classes: wide
---
## Introduction
For my final project, I was interested in exploring access to hurricane evacuation centers and social vulnerability factors in New York City. This analysis considers the following questions:
* What is the relationship between census-tract level demographics and proximity to hurricane
evacuation centers?
* Are centers in/near areas of high social vulnerability? What does walkability look like for these populations?
* What road networks in the event of major storm-related flooding will be impacted?

### Context
For context, the map below shows an overview of hurricane evacuation centers across the five NYC boroughs and hurricane evacuation zones (areas designated by the City as at risk of high inundation from hurricane-related flooding (1 = highest risk, 6 = lowest risk).
<div id="zones_centers_map"></div>

Across the five boroughs, there are 60 evacuation centers (based on the most up-to-date data available through NYC's Open Data portal). The distribution across the boroughs is shown on this bar graph. Brooklyn and Queens currently have the most centers within their boundaries (17 and 16, respectively).
<div id="boros_hurricane_evac_centers_plot"></div>


