---
layout: post
title: "Fire Hydrants and Rats"
subtitle: "Unconventional method of validating 311 calls"
background: "https://cdn.viewing.nyc/assets/media/c1ca9bc8c449a2797606dd45dcb1adbe/elements/56b86fc813c3e1500f281d890bffa401/xl/9d222443-1149-46e1-a4e4-fd06b5f1afb6_1x.jpg"
---

## 311 Calls - Are they reliable?

A problem that arose after some discussions is the reliability of 311 calls. Granted we did take precautions with estimating Rat Populations with the use of buffer periods, but that did not mean anything for the reliability of the calls themselves. One could easily inflate our results with a coordinated effort, or on the flipside make it seem like there are no rats in an area because nobody bothers to report a sighting. So, what was something that was easily spotted, something that OpenData NYC records, and common enough for a group of interns and their mentors to observe. Fire Hydrants.

## The Set-Up and Excursion

The plan was simple, go out on select streets and avenues and record the street violation "Parking Near a Fire Hydrant". [It is illegal in New York City to park within 15 feet on either side of a fire hydrant.](https://www1.nyc.gov/html/dot/html/motorist/parking-regulations.shtml) record all the necessary details of the violation. This included plate number, time, and location. We wait for a week or so and then compare what we found against the [Open Parking and Camera Violations](https://data.cityofnewyork.us/City-Government/Open-Parking-and-Camera-Violations/nc67-uf89) Database from NYC OpenData that were ticketed.

## Findings

#### This map plots the violations that we observed.

![observed](https://raw.githubusercontent.com/marmar897/RatsData/main/Graphs/observed_manhattan.png)

#### This map plots the violations that we observed and were ticketed.

![ticketed](https://raw.githubusercontent.com/marmar897/RatsData/main/Graphs/ticketed_manhattan.png)

It turns out that out of the 123 violations that we as a team observed that day, only 4 appeared in the Open Parking Data and were ticketed. So, this did not show the reliability of 311 calls in a positive light. That said, it was made clear in the beginning that the total reliability of 311 calls was a necessary assumption to estimate NYC's rat population.
