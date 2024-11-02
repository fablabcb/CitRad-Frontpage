---
title: Vorbereitung Radaranschluss
description: >
  Um auch das Radarmodul mit der richtigen Spannung zu versorgen, brauchen wir einen Spannungswandler und einige Anschlussvorbereitungen für den Datenaustausch. 
date: 2024-01-09
weight: 3
---
## Das brauchst du

<div class="row">
    <div class="col-md-6">
       <h3>Werkzeug</h3>
       <ul>
       <li>Saitenschneider</li>
       <li>Spitzzange</li>
       <li>Lötkolben + Lötzinn</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Teile</h3>
<ul>
       <li>Teensy Mikroprozessor</li>
        <li>Knopfzellendings</li>
        <li>Schrumpfschlauch</li>
        <li>2-adriges Kabel (5cm)</li>
       </ul> 
       </div>
</div>

## So funktioniert es 

<div class="row">

### Spannungwandler an Teensy
<div class="col-md-6">
       {{< imgproc spannungswandler1 Fit "600x400 webp" >}} Spannungswandler, angelötet an GND und 3.3V des Teensy {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

 Spannungwandler mit 3.3V und Gnd des Teensy verbinden
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->


<div class="row">

### Steckerverbindung vorbereiten (Teil 1: 6-Pin-Stecker)
<div class="col-md-6">
       {{< imgproc prep_spannung Fit "600x400 webp" >}} Teilweise angelöteter 6-Pin-Stecker {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
- Pin 1 (Nummerierung wie am Radar-Modul) aus dem Stecker ziehen (wird nicht benötigt).
- Pin 5 und 6 umbiegen sodass sie in die line-in Anschlüsse des Audio Boards passen (siehe Foto).
- Enable (Pin 2) umbiegen und mit Pin 17 des Teensy verbinden (passt gerade so).
- Gnd (Pin 4) und Vcc (Pin 3) mit dem Output des DC-DC verbinden (siehe Foto). Hier muss man eventuell mit Lötzinn oder einem kurzen Draht überbrücken.</div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Steckerverbindung vorbereiten (Teil 2: 4-Pin-Stecker)
<div class="col-md-6">
       {{< imgproc radar_stecker Fit "600x400 webp" >}} Vorbereiteter 4-Pin-Stecker. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

 GND (Pin 9) über kurzes Kabel mit Gnd am linein oder mic in verbinden.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->
<div class="row">

### Endergebnis
<div class="col-md-6">
       {{< imgproc radar_stecker_prep2_pin Fit "600x400 webp" >}} Nach Ausführung aller Schritte {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
        Am Ende sollte alles so wie auf dem Foto aussehen. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->