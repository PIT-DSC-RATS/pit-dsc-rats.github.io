---
layout: post
title: "Fire Hydrants and Rats"
subtitle: "Unconventional method of validating 311 calls"
background: "/img/fire_hydrants/hydrant_bg.jpg"
---

## 311 Calls - Are they reliable?

A problem that arose after some discussions is the reliability of 311 calls. Granted we did take precautions with estimating Rat Populations with the use of buffer periods, but that did not mean anything for the reliability of the calls themselves. One could easily inflate our results with a coordinated effort, or on the flipside, make it seem like there are no rats in an area because nobody bothers to report a sighting. So, what was something that was easily spotted, something that OpenData NYC records, and common enough for a group of interns and their mentors to observe? Fire Hydrants.

## The Set-Up and Excursion

The plan was simple: go out on select streets and avenues and record a specific type of traffic violation: Parking Near a Fire Hydrant. [It is illegal in New York City to park within 15 feet on either side of a fire hydrant.](https://www1.nyc.gov/html/dot/html/motorist/parking-regulations.shtml) We recorded all the necessary details of the violation. This included plate number, time, and location. We waited for a week or so for NYC OpenData to update their databases to then compare what we found against the [Open Parking and Camera Violations](https://data.cityofnewyork.us/City-Government/Open-Parking-and-Camera-Violations/nc67-uf89) Database from NYC OpenData that were ticketed.

## Findings

#### This map plots the violations that we observed.

![observed](\img\fire_hydrants\observed_manhattan.png)

#### This map plots the violations that we observed and were ticketed.

![ticketed](\img\fire_hydrants\ticketed_manhattan.png)

### Get ready for some numbers thrown your way.

##### I.

[We observed 123 Fire Hydrant traffic Violations from 1:00 PM to 4:00 PM of July 11, 2022](https://github.com/marmar897/RatsData/blob/main/july_11_observations.csv)

##### II.

[There were 31 311-Calls that were about Illegal Parking near a Fire Hydrant. Which had zero overlap with the traffic violations we observed](https://github.com/marmar897/RatsData/blob/main/calledin.csv)

##### III.

[There were 1,993 Fire Hydrant related traffic violations in July 11, 2022. Which had zero overlap with our observations](https://github.com/marmar897/RatsData/blob/main/july_11_hydrant_violations.csv)

##### IV.

[Only 4 of the Fire Hydrant related traffic violations that we observed were ticketed](https://github.com/marmar897/RatsData/blob/main/DataSets/result.csv)

<p></p>

### Takeaways from this validation side project

##### I.

It's somewhat reasonable to assume that the NYPD has a ticketing rate of 3.25% when it comes to Fire Hydrant Violations.

##### II.

There being no overlap between the 123 violations that the team observed and the 31 calls made in Manhattan during that day indicates that;

<p>New Yorkers really do mind their own business</p>
<p>OR</p>
<p>The NYPD do not respond fast enough to the 311 report</p>
<p>OR</p>
<p>Some 311 calls might be bogus</p>

This result does not paint too good a picture for the reliability of 311 calls. That said, it was made clear in the beginning that the total reliability of 311 calls was a necessary assumption to estimate NYC's rat population.
