---
title: Der erste Prototyp
date: 2023-06-01
description: >
  Nach der ersten Sichtung von möglichen Radarsensoren und Microcontrollern konnte auch das restliche Zubehör besorgt werden und mit dem Aufbau eines ersten kabelgebundenen Sensors begonnen werden.
author: Nanu
resources:
  - src: "featured-prototype.jpg"
    title: "PrototypeFund: Kickoff-Sketch Citrad"
    params:
      byline: "Photo: Nanu Frechen / CC-BY-CA"
  - src: "first_data.png"
    title: "Erste Daten vom Prototyp"
    params:
      byline: "Screenshot: Nanu Frechen / CC-BY-CA"
---


Der CitRad Sensor sollte auf einem möglichst günstigen aber trotzdem zuverlässigen Radarsensor aufbauen und mit einfachen Mitteln nachzubauen sein. Nach einigen Tests fiel unsere Wahl auf das 
[IPS-354 Modul von Innosent](https://www.innosent.de/radarsensoren/ips-354/). Ausserdem brauchten wir einen leistungsstarken Mikroprozessor um die Signale des Sensors zu verarbeiten. Hier entschieden wir uns für den [Teensy 4.0](https://www.pjrc.com/store/teensy40.html) in Kombination mit dem dazu erhältlichen [Teensy Audio Board](https://www.pjrc.com/store/teensy3_audio.html). Das Signal des Sensors lässt sich nämlich mit Audio-Tools verarbeiten. Dazu gibt es das [Audio System Design Tool](https://www.pjrc.com/teensy/gui/index.html) und ausführliche [Tutorials](https://www.pjrc.com/store/audio_tutorial_kit.html). Für uns war vor allem von Interesse dass sich damit eine Spektral-Transformation (FFT) umsetzen lässt. Im Gegensatz zu anderen Systemen kann der Teensy weiter Daten aufzeichnen, während er die Datenverarbeitung macht, sodass uns keine Daten verlorgen gehen.



{{< imgproc prototype Fill "600x300 webp" >}}
Der allererste Hardware-Prototyp
{{< /imgproc >}}

## Ein low-noise Verstärker?

Anfangs waren wir noch überzeut, dass wir eine Verstärkerschaltung brauchen, um das Signal des Sensors nutzen zu können. Hier haben wir verschiedene Verstärkerplatinen getestet und sogar eine [komplett eigene Platine](https://community.fablab-cottbus.de/t/citrad-elektronik-entwicklung/454) entworfen. Zum Schluss haben wir aber gemerkt, dass wir gar keine Verstärkung brauchen, wenn wir die [32bit Audio Library](https://github.com/chipaudette/OpenAudio_ArduinoLibrary#openaudio-library-for-teensy) verwenden, die die volle Bandbreite des Digitalwandlers auf der Audio-Platine nutzt.

## Erste Tests

Mit ein paar Jumperkabeln und Steckleisten konnte es jetzt an den Zusammenbau des allerersten Prototypen gehen. Da zu Beginn ohnehin der Laptop-Betrieb vorgesehen war, wurden alle Komponenten per USB-Kabel mit Strom versorgt und gleichzeitig eine Datenverbindung hergestellt um sich die Daten anschauen zu können. Die Ergebnisse sahen vielversprechend aus!

{{< imgproc first_data Fill "600x300 webp" >}}
Erste aufgezeichnete Daten. Die Geschwindigkeitsverläufe mehrerer Autos sind sichtbar.
{{< /imgproc >}}