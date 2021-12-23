---
title: "Accessibility to Nearest Evacuation Center"
date: 2019-04-13
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Embedding interactive charts on static pages using Jekyll."
altair-loader:
  altair-chart-1: "charts/measlesAltair.json"
hv-loader:
  points_hvplot_access_map: ["charts/points_hvplot_access_map.html", "500"] # second argument is the height
toc: true
toc_sticky: true
---

## Defining the Urban Street Network

Show OSMnx road network for process?

## HvPlot of Walking Accessibility to Nearest Evacuation Center

Text describing the map:

<div id="points_hvplot_access_map"></div>

## Notes

- See the [raw source code](https://raw.githubusercontent.com/MUSA-550-Fall-2020/github-pages-starter/master/_posts/2019-04-13-measles-charts.md) of this post for details on how these charts were embedded.
- See the [lecture 13A slides](https://github.com/MUSA-550-Fall-2020/week-13/blob/master/lecture-13A.ipynb) for the code that produced these plots.

**Important: When embedding charts, you will likely need to adjust the width/height of the charts before embedding them in the page so they fit nicely when embedded.**
