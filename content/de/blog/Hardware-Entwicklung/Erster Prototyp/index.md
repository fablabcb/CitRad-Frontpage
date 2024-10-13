---
title: Der erste Prototyp
date: 2023-06-01
description: >
  Nach der ersten Sichtung von möglichen Radarsensoren und Microcontrollern konnte auch das restliche Zubehör besorgt werden und mit dem Aufbau eines ersten kabelgebundenen Sensors begonnen werden.
author: Bene
resources:
  - src: "featured-prototype.jpg"
    title: "PrototypeFund: Kickoff-Sketch Citrad"
    params:
      byline: "Photo: Nanu Frechen / CC-BY-CA"
---


CitRad sollte auf einem zuverlässigen und dennoch möglichst günstigen Radarsensor aufbauen. Eine gründliche Recherche war notwendig. Hier kamen uns - wie so oft - die vielfältigen Erfahrungen der Mitglieder des Fablab Cottbus e.V. zugute. Einer, zufälligerweise Doktorand im Radarbereich konnte uns schonmal die grobe Richtung vorgeben. Außerdem nutzten wir die Chance, direkt ein paar Sensoren austesten zu können. Ein passender Kandidat war schnell gefunden.

{{< imgproc prototype Fill "600x300 webp" >}}
Der allererste Hardware-Prototyp
{{< /imgproc >}}

## Die Umwandlung der Radardaten: Audio-Shield

In unserem Setup sollten die Radardaten in Audiosignale umgewandelt werden. Ganz konkret in WAVE Dateien. Dafür musste ein Audio-Shield zum Einsatz kommmen, was sowohl mit Radarsensor als auch dem verwendeten Microcontroller kompatibel ist.

## Die Wahl des Microcontrollers: Teensy

Die WAVE-Dateien, in die unsere Daten aus dem Radarsensor umgewandelt werden, haben den Vorteil, unkomprimiert zu sein. Das lässt auf der einen Seite zuverlässigere Auswertungen zu. Auf der anderen Seite bedeutet es aber auch größere Datenmengen, die verarbeitet werden müssen. Auch wenn im Anfangsstadium die Daten zur Auswertung auf den Computer ausgeleitet werden, muss das System in Zukunft fähig sein, die Daten direkt auszuwerten und nur die fertig ausgewerteten Daten abzuspeichern. Für diesen Fall ist also etwas mehr Rechenpower gefragt. Standard Arduinos oder der Raspberry Pi Pico vielen da schnell raus.

 Unsere Wahl viel am Ende auf den Teensy, da er die notwendige Rechenleistung bietet und als beliebter Microcontroller in der Maker-Szene gut dokumentiert und erprobt ist.

## Die Zusammenstellung der Komponenten

Mit ein paar Jumperkabeln und Steckleisten konnte es jetzt an den Zusammenbau des allerersten Prototypen gehen. Da zu Beginn ohnehin der Laptop-Betrieb vorgesehen war, wurden alle Komponenten per USB-Kabel mit Strom versorgt und gleichzeitig eine Datenverbindung hergestellt. 

## Der erste Erfolg: Die Auswertung der Radardaten

[...]
