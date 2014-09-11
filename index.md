---
title       : The UFOs Application
subtitle    : An Examination of Sightings in the US and Canada
author      : 
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : prettify  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
---
## Introduction

[The National UFO Reporting Center](http://www.nuforc.org/index.html) maintains an online database for reporting UFO sightings in the US and Canada.  Users enter the date of observation, location, shape of the UFO, duration of the sighting, and any additional comments that they may deem relevant.  Reports stretch back to the year 0200, but this app only uses the last ten years of data. 

Users can examine the data grouped by region of the United States or Canada, look for any trends in reported shape, and look at whether or not there is a statistically significant increase in sightings over the past 10 years.

The app can be found [here](https://ezcode123.shinyapps.io/UFOs/).

<img class=center src="assets/fig/twoufos.png" height='200' width='200'/>

--- .class #id 

## Initial Graphs

When entering the app, the user will find two initial graphs:

![plot of chunk graphs](figure/graphs.png) 

The graph to the left can be used to select the region and shape of most interest.  The graph to the right shows that the number of UFO sightings has increased over the past 10 years.  The p-value of 0.0067 indicates that the observed increase is statistically significant.

---

## User Inputs

There are two pulldown menus that will allow downselection of the data:

1. Region: 
     * Northeast, Midwest, South, West, and Canada.  
     * This can also be left to the default of "All".
2. UFO Shape:
     * Sphere, Unknown, Egg, Light, Circle, Chevron, Changing, Cylinder, Disk, Triangle, Rectangle, Diamond, Formation, Oval, Teardrop, Cigar, Other, Flash, Fireball, Cone, Cross
     * This can also be left to the default of "All".

---

## Output

1. If a Region is selected, the first graph will change to a simple barchart of that region's sightings by shape.
2. The scatterplot of reports over time will be updated in either Region or Shape is selected.  The data in the graph is limited to that Region/Shape and a new slope and p-value is reported.  This can be used to look for any increases or decreases in shape reporting over time, or for any regional differences.


