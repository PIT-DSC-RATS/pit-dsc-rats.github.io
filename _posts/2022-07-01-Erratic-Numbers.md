---
layout: post
title: "Erratic Numbers"
subtitle: "No rats to thousands of rats in a year?"
background: "/img/erratic_numbers/Rats.gif"
---

## Problems with Mark-Recapture

The erraticity of our numbers looks to be far beyond the realm of margin for error. For instance, in the year 2011, in ZIP Code 10022, our math says 4,400 Rats. The subsequent year it says 26,400. Is the our math wrong or is there some hidden problem in our collected data? Or is it something else? It turns out that with four heads it's quite difficult to mess up copying a formula. So, what was the problem?

## A Problem with Proportion

Our erratic results come from a lack of consistent data points. Inconsistent in the sense that the volume of calls reporting "Rat Sightings" can vary wildly year-over-year per ZIP code.

[The Law of Large Numbers](https://en.wikipedia.org/wiki/Law_of_large_numbers). According to the law, the average of the results obtained from a large number of trials should be close to the **expected** value and tends to become closer to the expected value as more trials are performed. So, how does this affect our results?

When a specific ZIP Code has a low volume of calls reporting Rat Sightings in a given year (i.e a smaller sample size). A problem with proportions arise. Going from 100 to 150 is a 50% increase. Whereas, going from 500 to 550 is only an 10% increase, despite the absolute number increase being only 50 in both cases. So, the massive fluctuations of doubling, tripling, and halving of rat populations year-over-year not likely happening.

Below we have a line graph showing the Rat Population in Staten Island separated into neighborhoods over time.

![statenisland](\img\erratic_numbers\staten_3x5.png)
<span class="caption text-muted">Suspiciously massive spike in estimation</span>

The graph below shows a trend line for South Shore with a confidence region of 95%, which is the standard. This means that 95% of all results should be within that region.

![southshore](\img\erratic_numbers\southshore_3x5.png)

This is a similar graph to the one above, but has a confidence region of 99.9%. Meaning that this, in theory, should cover 999 results out of 1000.

![soutshore999](\img\erratic_numbers\southshore999_3x5.png)

As we can see, the year 2016 has such a large increase in rat population that even with a 99.9% confidence region, the estimated rat population of said year is still "out of bounds."

## What happened in South Shore in 2016?

Did all the rats decide to proliferate in an organized effort to take control of Staten Island? As great as a premise that is for a movie, it is unlikely. Possible, but unlikely.

In 2014, South Shore Rat Sighting Calls accounted for 1.708% of all the Rat Sighting Calls that year. In 2015 it was 1.549%.

<p></p>
2016, 1.547%.
<p></p>
2017, 1.362%.
<p></p>

Finally in 2018, it accounted for 1.570%.

Not too much of a difference percentage-wise, but with the method that a Icaro had come up with, a modification that dynamically changes the scope of how the Mark-Recapture method is applied. We are able, to some extent, mitigate the erraticity of our results.

So, why not just do it all at a ZIP level and then add all the numbers together? Applying the Mark-Recapture method at this level makes for some wildly innacurate numbers — ranging from an 8-fold increase in population, to ZIP Codes looking like they've eliminated their rat problem in a year. To cut a long story short, the less data points we have, the more erratic our results will be.
