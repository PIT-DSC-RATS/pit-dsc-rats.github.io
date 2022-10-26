---
layout: post
title: "Dynamic Mark-Recapture"
subtitle: "Circumventing the erratic figures"
background: "/img/dynamic_cap_recap/maths_bg.jpg"
---

## What is Dynamic Mark-Recapture Method?

A team member, Icaro presented to the team a slight alteration to the Mark-Recapture Method that drastically lowers the average standard deviation of our estimations, while attempting to be more granular. What does this solve?

A blanket, city-wide application of the Mark-Recapture method that Jonathan initially designed in 2014 provides the stablest of estimations. However, it is somewhat lacking in granularity.

A ZIP-level application of the Mark-Recapture method may be the most granular, but it has the most erratic of fluctuations. Since in some years there might not be that much data points, and not having a large volume of data points opens our estimations to some very weird behavior in the form of estimations quadrupling, halving, becoming infinity, or suddenly becoming zero.

If ZIP Code-level is too granular and City-Level is too broad, what do we do? With the alteration that Icaro made to the Mark-Recapture Method we strike a balance between the two.

The Dynamic Mark-Recapture Method looks at the ZIP's call volume and decides whether to apply Jonathan's City-Wide Mark-Recapture Method or the ZIP-Level Mark-Recapture Method. If there **ISN'T** enough calls, it applies the City-Wide Mark-Recapture and if there **IS** enough calls it applies a ZIP-Level Mark-Recapture.
