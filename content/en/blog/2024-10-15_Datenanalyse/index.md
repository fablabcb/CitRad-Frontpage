---
title: Data analysis
date: 2024-10-15
description: >
  How to count cars with a radar sensor?
author: Nanu
weight: 20
resources:
  - src: "featured-data_analysis.png"
    title: "Data analysis on the computer. The algorithm counts cars and measures speeds."
    params:
      byline: "Screenshot: Nanu Frechen / CC-BY-CA"
---

After all our experiments with amplifier circuits and a low-noise power supply, our sensor now seems to be working well. At least you can clearly see different vehicles in the spectral images of the radar data and recognize how fast they are driving. But how can the whole thing be evaluated with an algorithm? In the end, we just want to count vehicles and save the speed of each vehicle.

{{< imgproc data_analysis Fill "1200x600 webp" >}}
Data analysis on the computer. The algorithm counts cars and measures speeds.
{{< /imgproc >}}

The eye can easily distinguish the actual signal from the noise. In data analysis, this requires some smoothing and well-chosen limit values. The noise also changes over time. When the battery discharges. We also had to find a solution for this.

The signal analysis is based on the fact that certain frequencies stand out from the spectrum. This can be seen as lines over time. Each line is a moving object. A moving car, for example. The speed can then be calculated from the frequency.

We use a special trick to recognize when a car passes by: As the car passes, the angle to the Rarsensor changes. This causes the signal to bend downwards (towards 0 km/h). We recognize this bend and know that a car has just driven past the sensor. Whether this bend is to the left or to the right tells us in which direction the car was traveling. Now we just have to determine the detected speed before or after this trigger and save it.

What sounds simple is the result of a lot of fiddling around. And of course we first developed the whole thing on the computer using recorded data. This now has to be programmed and tested on the device itself. Only then will we be ready to give the device to interested parties for their own measurements. But that will be soon!

If you are interested in the technical details, you can take a look at our <a href=https://github.com/fablabcb/CitRad-SensorUnit/blob/main/Software/data%20processing%20method/read_and_display_raw_spectrum.Rmd target="_blank">repository on github</a>.