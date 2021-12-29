---
title: "Part 1: Exploratory Analysis of Population Density & Social Vulnerability"
date: 2021-12-21
published: true
tags: [dataviz, matplotlib, hvplot, altair]
excerpt: "Examining the spatial distribution of population and social vulnerability-related variables in NYC."
altair-loader:
  NYC_population_density_hist: "charts/NYC_population_density_hist.json"
  NYC_boros_total_population_barchart: "charts/NYC_boros_total_population_barchart.json"
  SVI_boxplot_theme1: "charts/SVI_boxplot_theme1.json"
  SVI_boxplot_theme2: "charts/SVI_boxplot_theme2.json"
  SVI_boxplot_theme3: "charts/SVI_boxplot_theme3.json"
  SVI_boxplot_theme4: "charts/SVI_boxplot_theme4.json"
hv-loader:
  NYC_population_density_hvplot: ["charts/NYC_population_density_hvplot.html", "800", "800"]
  SVI_NYC_hvplot_map: ["charts/SVI_NYC_hvplot_map.html", "600"]
toc: false
toc_sticky: false
classes: wide

---

## Total Population & Population Density
To gain a better understanding of where major centers of population are situated throughout the city, I pulled data from the US Census to obtain the total population estimate and land area for each tract. I first grouped population by borough and charted the total population in each. The Bronx has the highest total population.

<div id="NYC_boros_total_population_barchart"></div>

To get a more normalized measure of population, I calculated a new variable for population density:
>Population_Density = Total_Population/AREALAND

<div id="NYC_population_density_hist"></div>

To illustrate population density spatially, the interactive map below shows population density by census tract across NYC.

<div id="NYC_population_density_hvplot"></div>

## Overall SVI
According to the CDC, "social vulnerability refers to the potential negative effects on communities caused by external stresses on
human health. Such stresses include natural or human-caused disasters, or disease outbreaks." The CDC/ATSDR Social Vulnerability Index (CDC/ATSDR SVI) uses 15 US Census variables to assemble an index score for social vulnerability at different geographic levels. 

Since this index is specifically intended for disaster preparation and support for local communities and already incorporates robust census data, 
I downloaded the tract-level index for New York State and filtered to NYC. 
<div id="SVI_NYC_hvplot_map"></div>

### SVI Themes
In addition to an overall SVI score, the dataset also contains the individual scores for four different social vulnerability themes. I mapped the four themes' scores across each census tract, as well as the point layer for hurricane evacuation centers. Below each map is also a box and whiskers plot showing the distribution of scores per theme across all census tracts by each of the five boroughs.

#### Theme 1: Socioeconomic Status
![hec_SVItheme1_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme1_matplotlib.png)
<div id="SVI_boxplot_theme1"></div>

#### Theme 2: Household Composition & Disability
![hec_SVItheme2_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme2_matplotlib.png)
<div id="SVI_boxplot_theme2"></div>

#### Theme 3: Minority Status & Language
![hec_SVItheme3_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme3_matplotlib.png)
<div id="SVI_boxplot_theme3"></div>

#### Theme 4: Housing Type & Transportation
![hec_SVItheme4_matplotlib]({{ site.url }}{{ site.baseurl }}/assets/images/hec_SVItheme4_matplotlib.png)
<div id="SVI_boxplot_theme4"></div>

## Next: [Part 2](https://jennaepstein.github.io/MUSA550-finalproject/part2-accessibility-to-centers/)