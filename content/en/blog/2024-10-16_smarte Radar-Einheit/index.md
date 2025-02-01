---
title: Smart radar unit
date: 2024-10-16
description: >
  Implementation of data evaluation on the radar unit
author: Nanu
weight: 20
resources:
  - src: "smart-radar-unit.jpg"
    title: "The evaluation should later run completely on our sensor unit."
    params:
      byline: "Photo: Nanu Frechen / CC-BY-CA"
---

After we have developed an algorithm on the computer to analyze the radar data, the whole thing now has to be implemented on the device. Our goal is that all the data is already analyzed in the box and we only need to store the number of cars and their speed.

Compared to the [evaluation on the computer](/blog/2024/10/15/data-analysis/), there are a few things that need to be done differently on the device: On the computer, we worked with recorded data. On the device, we do the analysis live. This means that we have to buffer values in some places. For example, for smoothing the noisy raw signal. In one direction of travel, we have to buffer the speeds until the trigger of a passing car arrives. Only then can we save the data. For cars traveling in the other direction, we receive a trigger and then have to wait for the speed data.

{{< imgproc smarte-Radar-Einheit Fill "600x375 webp" >}}
The evaluation should later run completely on our sensor unit.
{{< /imgproc >}}


In addition, there is still a lot to optimize in order to evaluate the data efficiently on the small computing core.

You can follow our development in the [SensorUnit repository on github](https://github.com/fablabcb/CitRad-SensorUnit).

