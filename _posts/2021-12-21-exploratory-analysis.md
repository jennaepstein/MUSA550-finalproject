---
title: "Exploratory Analysis: Population Density & Social Vulnerability"
date: 2021-12-21
published: true
tags: [dataviz, matplotlib, hvplot]
excerpt: "Exploration of the spatial distribution of population and social vulnerability-related variables in NYC."
altair-loader:
  NYC_population_density_hist: "charts/NYC_population_density_hist.json"
hv-loader:
  NYC_population_density_hvplot: ["charts/NYC_population_density_hvplot.html", "800", "800"]
  SVI_NYC_hvplot_map: ["charts/SVI_NYC_hvplot_map.html", "800", "800"]
toc: false
toc_sticky: false
classes: wide

---

## Population Density
To gain a better understanding of where major centers of population are situated throughout the city, I pulled data from the US Census using cenpy to obtain the total population estimate and land area for each tract. I then calculated a new variable for population density:
* Population_Density = Total_Population/AREALAND

<div id="NYC_population_density_hist"></div>

To illustrate population density spatially, the interactive map below shows population density by census tract across NYC.

<div id="NYC_population_density_hvplot"></div>

## Overall SVI
According to the CDC, “social vulnerability refers to the potential negative effects on communities caused by external stresses on
human health. Such stresses include natural or human-caused disasters, or disease outbreaks.” The CDC/ATSDR Social Vulnerability Index (CDC/ATSDR SVI) uses 15 U.S. census variables to assemble an index score for social vulnerability at different geographic levels. The following graphic breaks down the different components of the index:
![SVI]({{ site.url }}{{ site.baseurl }}/assets/images/SVI.jpg)

Since this index is specifrically intended for disaster preparation and support for local communities and already incorporates robust census data, 
I downloaded the tract-level index for New York State and filtered to NYC. 
<div id="SVI_NYC_hvplot_map"></div>

### SVI Themes
In addition to an overall SVI score, the dataset also contains the individual scores for four different social vulnerability themes. I mapped the four themes' scores across each census tract, as well as the point layer for hurricane evacuation centers.
#### Theme 1: Socioeconomic Status
![hec_SVItheme1_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme1_matplotlib.png)
#### Theme 2: Household Composition & Disability
![hec_SVItheme2_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme2_matplotlib.png)
#### Theme 3: Minority Status & Language
![hec_SVItheme3_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme3_matplotlib.png)
#### Theme 4: Housing Type & Transportation
![hec_SVItheme4_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme4_matplotlib.png)
