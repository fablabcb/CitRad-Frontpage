---
title: The first prototype
date: 2023-06-01
description: >
  After the first sighting of possible radar sensors and microcontrollers, the remaining accessories could be procured and the construction of a first wired sensor could be started.
author: Nanu
resources:
  - src: "content/de/blog/Hardware-Entwicklung/Erster Prototyp/featured-prototype.jpg"
    title: "PrototypeFund: Kickoff sketch Citrad"
    params:
      byline: "Photo: Nanu Frechen / CC-BY-CA"
  - src: "first_data.png"
    title: "First data from the prototype"
    params:
      byline: "Screenshot: Nanu Frechen / CC-BY-CA"
---


The CitRad sensor had to be based on a radar sensor that was as inexpensive as possible but still reliable and easy to replicate. After a few tests, we chose the
[IPS-354 module from Innosent](https://www.innosent.de/radarsensoren/ips-354/). We also needed a powerful microprocessor to process the signals from the sensor. Here we opted for the [Teensy 4.0](https://www.pjrc.com/store/teensy40.html) in combination with the [Teensy Audio Board](https://www.pjrc.com/store/teensy3_audio.html), which is also available. The signal from the sensor can be processed with audio tools. The [Audio System Design Tool](https://www.pjrc.com/teensy/gui/index.html) and detailed [Tutorials](https://www.pjrc.com/store/audio_tutorial_kit.html) are available for this purpose. We were particularly interested in the fact that a spectral transformation (FFT) can be implemented. In contrast to other systems, the Teensy can continue to record data while it is doing the data processing so that we do not lose any data.



{{< imgproc prototype Fill "600x300 webp" >}}
The very first hardware prototype
{{< /imgproc >}}

## A low-noise amplifier?

Initially, we were still convinced that we needed an amplifier circuit to be able to use the signal from the sensor. We tested various amplifier boards and even designed a [completely custom board](https://community.fablab-cottbus.de/t/citrad-elektronik-entwicklung/454). In the end, however, we realized that we wouldn't need any amplification at all if we used the [32bit Audio Library](https://github.com/chipaudette/OpenAudio_ArduinoLibrary#openaudio-library-for-teensy), which uses the full bandwidth of the digital converter on the audio board.

## First tests

With a few jumper cables and connectors, we were now ready to assemble the very first prototype. Since laptop operation was planned at the beginning anyway, all components were supplied with power via USB cable and at the same time a data connection was established so that the data could be viewed. The results looked very promising!

{{< imgproc first_data Fill "600x300 webp" >}}
First recorded data. The speed curves of several cars are visible.
{{< /imgproc >}}