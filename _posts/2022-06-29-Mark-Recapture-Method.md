---
layout: post
title: "Mark-Recapture Method"
subtitle: "How are we using it and how can we improve it?"
background: "/img/mark_recapture/marker.jpg"
---

## What is Mark-Recapture

In the previous post we talked about something called the [Capture-Recapture Method](https://en.wikipedia.org/wiki/Mark_and_recapture), or the [Mark-Recapture](https://en.wikipedia.org/wiki/Mark_and_recapture) method as it is more commonly known as. Take not that we might use this term interchangeably. This method commonly used in ecology to estimate an animal population’s size where it is impractical to count every individual. What is it that we do when we apply this population estimation technique? We capture a portion of the population in the initial phase, and mark them, then release them. After some period of time we recapture an equivalent portion of the first sample, and with estimations we first need to make some assumptions. We ASSUME that the chances of each rat getting captured in either the first or the second sample are the same. So, in the second phase we will recapture a mix of marked and unmarked individuals. Then we use the proportion of the marked members in the second sample to give an estimate of the population size.
![Recapture](\img\mark_recapture\recapture.jpeg)
<span class="caption text-muted">http://www.old-ib.bioninja.com.au/options/option-g-ecology-and-conser/g5-population-ecology.html</span>

## How are we using it?

Did we go out and about to capture rats? Nope, not only would it be disgusting, but it would take much more time than the alloted few weeks we had to finish this project. Not to mention the lack of resources to do something at a city-scale. So, we made another assumption based off of some numbers off of this [article](https://elifesciences.org/articles/54020) and this [exterminator's](https://www.ratrelief.com/many-rats-live-nest/) estimations of how many rats might live in a colony. With other sources mentioning that colonies can range anywhere from a minimum of 12 to 100+. We thought it reasonable to assume there would be 50 rats per colony.

Okay, so what does knowing how many rats in a colony help us estimate how many rats are in the city? Instead of doing the Mark-Recapture method on individual rats, we used the Mark-Recapture method on BBLs. Not Brazilian Butt Lifts, but Borough Block Lots. What's a [Borough Block Lot](https://en.wikipedia.org/wiki/Lot_and_block_survey_system)? Basically a unit of real-estate, a group of buildings, or a block.

Okay, okay, okay. What does all of this have to do with estimating the population of rats as a whole? Assuming that 311 Calls from [NYC OpenData](https://opendata.cityofnewyork.us/data) is dependable. We can "mark" BBLs if they called 311 and complained about a Rat Sighting. This way we don't have to do it at a Rat-Level but on a BBL-level.

Long story short, say a caller BBL 42 calls 311 and the call is tagged by the operator as a "Rat-Sighting" related call, BBL 42 is marked. After a set amount of time that we use for a buffer period, to make sure that the caller BBL 42 isn't calling 10 times a day for a week straight about the same rat, but a different one. We "recapture" that BBL and do the fancy math below. We get our estimations.

![Formula](\img\mark_recapture\formula.png)
<span class="caption text-muted">https://www.deanza.edu/faculty/heyerbruce/b6c_pdf/3b_Estimating%20Population%20Size.pdf</span>
