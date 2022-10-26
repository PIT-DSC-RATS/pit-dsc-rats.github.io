---
layout: post
title: "Initial Visualizations"
subtitle: "Line Graphs and Scatterplots of Rat Populations"
background: "/img/initial_vis/data_vis_bg.png"
---

## Heatmaps

Click on the heatmap image preview to access our summer **R-Shiny App** that has our interactive heatmaps and other older data visualizations. There is a heatmap showing the distribution of 311- Rat Sighting calls and 3 more Heatmaps with slight variations on their methods of rat population estimation.

**2021 Rat Sighting Reports by ZIP** - Shows exactly what the title says. It shows the distribution of the calls tagged with "Rat Sighting". Comparing this heatmap to the others that show the estimated rat populations, tells us that calls and estimated rat populations are not one to one. i.e. one call doesn't necessarily mean fifty rats.

**Estimated Rat Population by Year (nyc)** - This version of the heatmap shows the estimations based on the method used in [Jonathan Auerbach's](https://rss.onlinelibrary.wiley.com/doi/full/10.1111/j.1740-9713.2014.00764.x) 2014 Study.

**Estimated Rat Population by Year (zip)** - This version of the heatmap shows estimations that are also at a ZIP level but is more erratic, because of large variances in the amount of calls as was mentioned in the previous post **"Erratic Numbers"**.

**Estimated Rat Population by zip (Dynamic)** - This version of the heatmap shows the Dynamic Method that Icaro came up with, that dynamically changes the scope when there isn't enough data points (Calls) in a ZIP and excalates it to the City-Level and redistributes the population based on the percentage of calls.

<a href="https://angelatan222.shinyapps.io/ratsdata/" target="_blank">
![preview](\img\initial_vis\heatmap_preview.png)</a>
<span class="caption text-muted">https://angelatan222.shinyapps.io/ratsdata/</span>

## Line Graphs

![Non-Stacked](\img\initial_vis\mari_Graph_Non-Stacked_3x5.png)

This graph shows the rat population over the years separated into boroughs. We can see that Staten Island has the least amount of rats and Brooklyn has the most amount of rats, in terms of absolute numbers.

![Stacked](/img/initial_vis/Graph_Stacked_3x5.png)

This line graphs shows a similar story to the line graph above, showing the distribution of the total population as well as showing the cumulative number of rats in NYC. However, these two line graphs don't tell the whole story as density of rats also plays a factor.

## Scatterplot

![Scatterplot](\img\initial_vis\mari_graphNYCRatio20_3x5.png)

New Yorkers tend to affiliate themselves to their boroughs and they're neighborhood. To show a little more granularity, each point on this scatterplot shows New York City's 42 Neighborhoods.

We based our neighborhoods on this [Github Repo](https://github.com/erikgregorywebb/nyc-housing/blob/master/Data/nyc-zip-codes.csv)

The X-Axis shows the Rat to Human Ratio, meaning the higher up your neighborhood's point is on the scatterplot, the closer it making the myth of there being one rat per person in New York City, true.

The Y-Axis shows the Rat per Square Meter. So, on average if all the rats were equally spaced out. You would find one rat every 45 ~ 50 square meters or 500 square feet in Bushwick & Williamsburg. On the other hand, You would need to cover double the area to find one if you were in Northwest Brooklyn.

The Dashed Lines represent the mean and increaseing standard deviations. Points that are under the **GREEN-LINE** are below the mean. Points above the **RED-LINE** are in the 95th percentile, i.e a **PROBLEM**.

##### Central Brooklyn is the RATTIEST Neighborhood of 2020
