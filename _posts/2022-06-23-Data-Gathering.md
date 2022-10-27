---
layout: post
title: "Gathering the Data"
subtitle: "311 Calls NYC Open Data"
background: "/img/data_gathering/data_bg.gif"
---

## Background

"If we can't measure it, then it doesn't exist" Not in the sense that the unmeasurable simply phases out of existence, but if we can't measure the extent of a problem we have little-to-no-clue on how to start dealing with said problem.

![Rat](\img\data_gathering\ratbox.jpg)
<span class="caption text-muted">Photographer: Gary Hershorn/Corbis News/Getty Images</span>

Estimating the population of the furry New York Natives can either be very easy or very difficult. Is it as simple as saying "It's definitely more than 12 rats", or do we go on massive rat hunt to find and count every rat in the city? So, what do we do? We turn to the next best thing, estimations! The myth goes "There's one rat for every person in New York City" But is that really the case? Surely we can do better? And do better we did.

Building on the work our mentor and project owner, [Jonathan L. Auerbach](https://jauerbach.github.io/) did in 2014, we will be using his framework to try and get more accurate estimations of how many rats are in New York City, and maybe even localize those estimations to a Borough or Neighborhood level.

[![nycopendata](\img\data_gathering\nycopendata.png)](https://opendata.cityofnewyork.us/data)
<span class="caption text-muted">NYC OpenData has a catalog of datasets ranging from Maps of Subway Entrances, Film Permits, to 311 Calls. Click the photo to visit the site!</span>

## Initial Data Cleaning with R filter()

With all the recorded 311 calls from 2010 to 2021, there were a lot of calls to go through. By a lot, we mean close 30 Million 311 calls to go through. Thankfully, we didn’t have to go through them one-by-one manually. We cut down the unecessary data through some filters in R. We don’t need information noise complaints when looking at rats, no? So, we filter for Calls that are **NOT MISSING** the BBL and Year data points. We also refactor some variables from “Incident ZIP” to a much simpler “ZIP” and separating the “Month_Year” variable into variables “Month” and “Year”.

![Code](\img\data_gathering\coderist.png)
<span class="caption text-muted">Snippet of code showing the filtering process and refactorization</span>

## Refactoring Cleaned Data Sets

With the Data now cleaned and with some variables refactored, we separated the data into smaller data sets into 5 boroughs consisting of 42 distinct neigborhoods. This way, we can see the differences and much more easily apply the [Capture-Recapture Method](https://en.wikipedia.org/wiki/Mark_and_recapture) that will be discussed further in a later post. 

As a little sneak peek, Capture-Recapture Method, more commonly known as Mark-Recapture Method is a method commonly used in ecology to estimate an animal population's size when it is impractical to count every individual.

![Neighborhood](\img\data_gathering\Neighborhooderist.png)
<span class="caption text-muted">Snippet of code showing Zip Codes getting grouped into their respective neighborhoods</span>
