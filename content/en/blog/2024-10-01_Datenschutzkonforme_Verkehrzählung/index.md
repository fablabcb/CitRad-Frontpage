---
title: Data protection compliant traffic counting
date: 2024-10-01
description: >
  Camera-based projects for analyzing traffic data exist as commercial and open source projects. We have deliberately decided not to build on these projects, as they bring with them various problems with data protection. We made a conscious decision to use radar as the basic technology. Radar allows us to collect traffic data without violating personal rights.
author: Bene
weight: 20
resources:
  - src: "anoncars.jpg"
    title: "Blurred cars at intersection"
    params:
      byline: "Photo: Benedikt Stahl / CC-BY-CA"
---
When we realized that we wanted to collect open traffic data and make it available for analysis, we quickly came to the question of how. Existing projects for the automated analysis of camera images were tempting, as they would have saved us a lot of basic development work. However, data protection-compliant traffic counting would not be possible. Because by recording people, license plates, etc., we would be operating in a legal grey area - even if we deleted this data immediately after evaluation. Radar does not have any of these data protection problems, but it does present additional challenges in terms of analysis.   

{{< imgproc anoncars Fill "1200x600 webp" >}}
The radar only recognizes individual objects without capturing details. As if a camera could only record blurred road users.
{{< /imgproc >}}

## Anonymity of the data

Radar technology works by emitting electromagnetic waves that are reflected by vehicles. By analyzing the reflected waves, the system can collect information about the traffic flow without collecting personal data. This ensures the anonymity of road users. In contrast, image-based systems can collect potentially sensitive information about the identity of drivers and passengers, which is not the case with radar technology.

## Legal compliance and own claim

As we are of the fundamental opinion that personal data should be kept out of data sets where not absolutely necessary, Radar was the ideal solution for us. Of course, a pleasant side effect was that we did not have to concern ourselves with GDPR compliance. Because even if the image data had only been analyzed on the microcontroller and no one had seen it, numerous problems would have remained unresolved. For example, how do you ensure that third parties cannot gain access to the devices and access raw data that has not yet been deleted? Will we have problems with acceptance of the system if people have the feeling that they are being recorded on camera just because they are driving along a road in accordance with the rules? We were able to put all these considerations aside with a clear conscience by using radar.

## Technical requirements and advantages

As far as radar technology itself is concerned, there are some advantages but also many challenges. Camera images are easy for people to grasp. This makes it much easier and quicker to check the evaluation mechanisms during development. Radar, on the other hand, provides us with a spectrum for evaluation that is very difficult for inexperienced viewers to decipher. The initial effort and interpretation of the results will therefore tend to take more time. In the long term, however, radar works more reliably than image analysis. Radar does not care what light conditions prevail. The reflected waves look the same in pitch darkness as they do in broad daylight. Different weather conditions are also no problem for radar. Fog, rain and snow should, at least in theory, be manageable as soon as the evaluation algorithm has been properly adjusted. We will describe how successful we are in doing this in the coming blog posts.

## Conclusion

CitRad collects traffic data in compliance with data protection regulations and makes it available for further analysis. Nobody who drives past a CitRad sensor has to fear that data records will be created somewhere that will be associated with them. And there is certainly no need to fear points in Flensburg. Even if we detect speeding violations, we can only record them statistically and cannot draw any conclusions about the exact car or driver. Misuse of data is therefore also ruled out.
As far as the accuracy of the evaluation is concerned, it will certainly take some time before we can include all eventualities in the evaluation. Until then, however, the CitRad sensor already provides good trends and quantitative overviews.