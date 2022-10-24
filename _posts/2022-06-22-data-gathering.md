---
layout: post
title: "Gathering Data for Rat Populations Estimation"
subtitle: "311 Calls NYC Open Data"
background: "/img/data_gathering/data-gathering-bg.png"
---

## Background

"If we can't measure it, then it doesn't exist" Not in the sense that the unmeasurable simply phases out of existence, but if we can't measure the extent of a problem we have little to no clue on how to start dealing with said problem.

![Rat](\img\data_gathering\ratbox.jpg)
<span class="caption text-muted">Photographer: Gary Hershorn/Corbis News/Getty Images</span>

Estimating the population of the furry New York Natives can either be very easy or very difficult. Is it as simple as "There's a rat for every person in the city" or Do we go on an excursion to find and count every rat? The latter is BIG ask for 4 interns. So, what do we do? We turn to the next best thing, estimations! As previously mentioned we can just say "There's one rat for every person in New York City" and be done with it. But is that really the case? Surely we can do better? And do better we did.

Building on the work our mentor and project owner, [Jonathan L. Auerbach's](https://jauerbach.github.io/), we will be using his framework to try and get more accurate estimations of how many rats in New York City, and maybe even localize those estimations to a Borough or Neighborhood level, over the more conventional myth of the one to one ratio of people to rats.

[![nycopendata](\img\data_gathering\nycopendata.png)](https://opendata.cityofnewyork.us/data)
<span class="caption text-muted">NYC OpenData has a catalog of datasets ranging from Maps of Subway Entrances, Film Permits, to 311 Calls. Visit the site for all you NYC data needs!</span>

## Initial Data Cleaning with R filter()

With all the recorded 311 calls from 2010 to 2021 at the time of this project there were a lot of calls to go through, and by a lot we mean close 30 Million 311 calls to go through. Thankfully we don't have to go through them one by one manually. We cut down the unecessary data through some filters in R. I mean we don't need information noise complaints when looking at rats no? So we filter for Calls that do not have the BBL and Year data points missing. We also refactor some variables from "Incident Zip" to a much simpler "Zip" and separating the "Month_Year" variable into variables "Month" and "Year".

![Code](\img\data_gathering\coderist.png)

## Refactoring Cleaned Data Sets

With the Data now cleaned and refactoring some variables, we separated the data into smaller data sets into 5 boroughs and into 42 distinct neigborhoods. This way we can see the differences and much more easily apply the [Capture-Recapture Method](https://en.wikipedia.org/wiki/Mark_and_recapture) that will be discussed further in the next post. As a little sneak peek, Capture-Recapture Method, more commonly know as Mark-Recapture Method is a method commonly used in ecology to estimate an animal population's size where it is impractical to count every individual.

![Neighborhood](\img\data_gathering\Neighborhooderist.png)
<span class="caption text-muted">snippet of code showing Zip Codes getting grouped into their respective neighborhoods</span>
