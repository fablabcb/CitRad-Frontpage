---
title: Audioshield und Teensy verbinden 
description: >
  Vorbereitung des Audioshields für den Zusammenbau mit dem Mikroprozessor 
date: 2024-01-09
weight: 2
---
## Das brauchst du

<div class="row">
    <div class="col-md-6">
       <h3>Werkzeug</h3>
       <ul>
       <li><img src="/icons/saitenschneider.webp" alt="Saitenschneider" width="200"/>Saitenschneider</li>
       <li><img src="/icons/spitzzange.webp" alt="Spitzzange" width="200"/>Spitzzange</li>
       <li><img src="/icons/lötkolben.webp" alt="Lötkolben" width="200"/>Lötkolben + Lötzinn</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Teile</h3>
<ul>
       <li>Teensy Mikroprozessor</li>
        <li>2-adriges Kabel (5cm)</li>
        <li>40-Pin-Leiste</li>
       </ul> 
       </div>
</div>

## So funktioniert es 

<div class="row">

### Pinleiste einkürzen
<div class="col-md-6">
       {{< imgproc audio_pinleiste Fit "600x400 webp" >}} Kürzen der Pinleiste auf Länge des Audioshields {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 Die 40-Pin-Leiste ist für das Audioshield zu lang. Steck sie einfach an einer Seite bündig ins Shield und trenne den Überstand mit dem Saitenschneider ab. Das gleiche machst du nochmal für die gegenüberliegende Seite.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Pinleisten anlöten
<div class="col-md-6">
       {{< imgproc soldered Fit "600x400 webp" >}} Kürzen der Pinleiste auf Länge des Audioshields {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 Beide Pinleisten lötest du nun auf der Rückseite des Audioshields fest. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Teensy aufsetzen und Pins anpassen
<div class="col-md-6">
       {{< imgproc modified_pins Fit "600x400 webp" >}} Pins abknipsen (cyan) bzw. zurechtbiegen (rot). {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 <ul><li>Nun setzt du den Teensy auf die langen Pins auf. Dabei zeigt die USB-Buchse nach oben und in die gleiche Richtung wie der Klinkenanschluss des Audioshields.</li> 
 <li style="border: 2px solid #a6113aff"> Die Pins an 5V und GND biegst du mit einer Spitzzange (<img src="/icons/spitzzange.webp" alt="Spitzzange" width="50"/>) wie im Foto schräg nach vorne.</li>
 <li style="border: 2px solid #7adef1ff">
  Um später den Spannungswandler gut anlöten zu können, entfernst du jetzt mit dem Saitenschneider (<img src="/icons/saitenschneider.webp" alt="Saitenschneider" width="50"/>) die Pins 21, 22, 23 (Ja, Pin 21 ist auf dem Foto noch nicht gekürzt).</li>
 </ul>   
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Buchse für die Stromversorgung vorbereiten
<div class="col-md-6">
       {{< imgproc cable_plug Fit "600x400 webp" >}} Buchsenkabel zusammenlöten {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 <ul><li> Zuerst das zweiadrige Kabel auf etwa 4 cm kürzen, an beiden Seiten ein Stück weit auftrennen und alle Enden abisolieren</li>
 <li>Um nichts verkehrt anzulöten, stecke am besten die Buchse auf den Stecker des Akkupacks. Dann so zusammenlöten, dass das schwarze Kabel auf das schwarze Kabel und das rote auf das rote geht.</li>
 </ul>
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Buchse mit Zugentlastung festlöten
  <div class="col-md-6">
       {{< imgproc stecker1 Fit "600x400 webp" >}} Buchsenkabel zusammenlöten {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

 <ul><li>Den Kabel des Knopfzellenhalters (bereits am Teensy angelötet) führst du jetzt in Richtung der USB-Buchse über den Teensy hinweg. Das schwarze Kabel der Akkupackbuchse (<strong>ohne Akku</strong>) führst du dann mit durch den Schrumpfschlauch. </li>
 <li>Das <span style="color:black">schwarze</span> Kabel lötest du am zuvor umgebogenen GND-Pin und das <span style="color:red">rote</span> Kabel am ebenfalls umgebogenen 5V Pin an.</li>
 <li>Als letztes schiebst du die Kabel des Knopfzellenhalters soweit in richtung Lötstellen, dass keine Spannung auf dem Kabel ist und erwärmst vorsichtig den Schrumpfschlauch. So entsteht eine Zugentlastung. </li>
 </ul>
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->