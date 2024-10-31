---
title: Aufbau
description: >
  Schritt für Schritt-Anleitung für den Zusammenbau der CitRad Sensoreinheit. 
date: 2024-01-09
weight: 6
---

{{% pageinfo %}}
This is a placeholder page. Replace it with your own content.
{{% /pageinfo %}}


## Aufbau

### Platine vorbereiten

1. Teensy Vusb-Verbindung trennen (mit Messer). Danach einmal an USB anstecken und sicherstellen dass der Teensy nicht mehr von USB versorgt wird.
1. Knopfzellenbatterie an Teensy anlöten. Vor dem Anlöten Schrumpfschlauch über beide Kabel (wird später als Zugentlastung an die Stromversorgungskabel geschrumpft).
1. 14-Pin Pinleiste (zuschneiden aus 40-Pin Leiste) mit kurzer Seite an Audio Board anlöten
1. Teensy auf die langen Stifte aufsetzen (Pins stehen über) und anlöten
1. Batteriestecker an Batteriekabel löten.
1. Von der Teensy Seite: 5V Pin und GND Pin (rechts und links vom USB) nach vorne biegen.
1. Batteriekabel an die überstehenden Pins von Gnd und 5V des Teensy löten. Dabei das eine Kabel durch den Schrumpfschlauch am Kabel der Knopfzellenbatterie fädeln (Zugentlastung).
1. Die restlichen überlangen Pins können optional gekürzt werden. Mindestens aber die drei Pins links vom 3.3V Pin
1. DC-DC mit 3.3V und Gnd des Teensy verbinden (siehe Foto)
1. 6-Pin-Stecker mit langen Beinen anlöten:
    1. Pin 1 (Nummerierung wie am Radar-Modul) aus dem Stecker ziehen (wird nicht benötigt).
    1. Pin 5 und 6 umbiegen sodass sie in die line-in Anschlüsse des Audio Boards passen (siehe Foto).
    1. Enable (Pin 2) umbiegen und mit Pin 17 des Teensy verbinden (passt gerade so).
    1. Gnd (Pin 4) und Vcc (Pin 3) mit dem Output des DC-DC verbinden (siehe Foto). Hier muss man eventuell mit Lötzinn oder einem kurzen Draht überbrücken.
1. 4-Pin Stecker: GND (Pin 9) über kurzes Kabel mit Gnd am linein oder mic in verbinden.

### Radarmodul zusammen stecken

1. Radarmodul in 3D-Druck Halterung stecken (siehe Foto).
1. Teensy an 3D-Druck Halterung anschrauben (siehe Foto). Dabei die Stecker des Radarmoduls aufstecken.
1. 4-Pin Stecker am Radarmodul einstecken.
1. Lasercut Teile seitlich an das Radarmodul anschrauben.
1. SD-Karte in Audioboard einsetzen.

### Gehäuse vorbereiten

1. Grundplatte in Gehäuse schrauben.
1. Gewinde in Befestigungslöcher (Rückseite) schneiden.
1. Mastplatte mit M5-Schrauben und den Unterlegschrauben (im Lasercut Teil enthalten) an Rückseite anschrauben. 
1. Gummidichtung in Deckel einlegen (was zu lang ist abschneiden).

### Zusammenbau

1. Akku mit Kletterverschluss an Grundplatte befestigen.
1. Knopfzelle in Knopzellenhalter einsetzen. Schalter auf "ON" stellen.
1. Radarmodul mit Halterung in Schlitze in der Grundplatte stecken.
1. Teensy mit Batterie verbinden.

## Software installieren
1. Sketch drauf laden
2. Uhrzeit einstellen
3. Mit Processing überprüfen ob der Radarsensor richtig funktioniert