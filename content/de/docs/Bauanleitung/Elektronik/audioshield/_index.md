---
title: Audioshield und Teensy verbinden 
description: >
  Vorbereitung des Audioshields für den Zusammenbau mit dem Entwicklerboard 
date: 2024-01-09
weight: 2
---
## Das brauchst du

<div class="row">
    <div class="col-md-6">
       <h3>Werkzeug</h3>
       <ul>
       <li><img src="/icons/saitenschneider.webp" alt="Seitenschneider" width="200"/>Seitenschneider</li>
       <li><img src="/icons/spitzzange.webp" alt="Spitzzange" width="200"/>Spitzzange</li>
       <li><img src="/icons/lötkolben.webp" alt="Lötkolben" width="200"/>Lötkolben + Lötzinn</li>
       <li><img src="/icons/abiso.webp" alt="Lötkolben" width="200"/>Abisolierzange</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Teile</h3>
<ul>
       <li>Teensy Entwicklerboard</li>
       <li>Audioshield</li>
        <li>2-adriges Kabel (4cm)</li>
        <li>40-Pin-Leiste</li>
        <li>Batteriebuchse</li>
        <li>Akku-Pack (nur zur Kontrolle der korrekten Polung beim Löten)</li>
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


 Die 40-Pin-Leiste ist für das Audioshield zu lang. Steck sie einfach an einer Seite bündig auf die Lochreihe des Audioshields auf und trenne den Überstand mit dem Seitenschneider ab. 

 Das **Gleiche machst du nochmal** für die gegenüberliegende Seite. Du solltest jetzt zwei gleichlange Leisten (14 Pins) und ein kürzeres Reststück haben. 
 
 Das Reststück wird nicht mehr benötigt. Leg es am besten beiseite, damit du es nicht versehentlich verwendest.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Pinleisten anlöten
<div class="col-md-6">
       {{< imgproc soldered Fit "600x400 webp" >}} Die eingekürzten Pinleisten werden mit den kurzen Enden an das Audioshield gelötet. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 Deine beiden gleichlangen Pinleisten steckst du jetzt mit der kurzen Seite von oben (Seite mit Klinkenanschluss und Micor-SD-Karten-Slot) in das Audioshield und lötest die Leisten auf der Rückseite des Audioshields Pin für Pin fest. 
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
  Um später den Spannungswandler gut anlöten zu können, knipst du jetzt mit dem Seitenschneider (<img src="/icons/saitenschneider.webp" alt="Seitenschneider" width="50"/>) die Pins 21, 22, 23 ab.</li>
  <li>Jetzt lötest du alle Pins fest, um die beiden Platinen zu verbinden.
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


 <ul>
 <li>Im Bild siehst du <span style="border: 2px solid #7adef1ff">Cyan eingerahmt das zweiadrige Kabel (4 cm) und die Anschlussbuchse.</span> In der Anschlussbuchse steckt noch ein Stecker (mit Kabel) der im Lieferumfang enthalten war. Das kann eine Hilfe beim Löten sein. Stecker und Kabel brauchst du allerdings in den folgenden Schritten nicht mehr.
 <li> Trenne das zweiadrige Kabel (4 cm) an beiden Seiten ein Stück weit auf und isoliere alle Enden ab. (Im Foto bereits geschechen)</li>
 <li>Löte jetzt das Kabel <strong>so</strong> an die Buchse, dass die <strong>Polung zum Stecker des Akkupacks passt</strong>.
 </li>
 </ul>
 {{% alert color="primary" %}}
Achtung: Manche Buchsen/Stecker-Sets sind genau umgekehrt gepolt. Vergleiche immer ob der Stecker genauso wie der des Akkupacks gepolt ist und löte erst dann die Buchse entsprechend an das Kabel. 
{{% /alert %}}
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Buchse mit Zugentlastung festlöten
  <div class="col-md-6">
       {{< imgproc stecker1 Fit "600x400 webp" >}} Buchsenkabel zusammenlöten {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

 <ul><li>Das Kabel des Knopfzellenhalters (bereits am Teensy angelötet) führst du jetzt in Richtung der USB-Buchse über den Teensy hinweg. Das schwarze Kabel der Akkupackbuchse aus dem vorherigen Schritt führst du dann (von der Knopfzelle aus kommend) mit durch den Schrumpfschlauch. </li>
 <li>Das <span style="background-color:black; color:white">schwarze</span> Kabel lötest du am umgebogenen <span style="background-color:black; color:white">GND-Pin</span> und das <span style="background-color:red; color:white">rote</span> Kabel am ebenfalls umgebogenen <span style="background-color:red; color:white">5V Pin</span> an.</li>
 <li>Um die Lötstellen für die Kabel des Knopfzellenhalters gegen Zug zu entlasten, werden alle Kabel im Schrumpfschlauch durch Erwärmen "fixiert". Schiebe dazu die Kabel des Knopfzellenhalters etwas in Richtung ihrer Lötstellen zurück, sodass keine Spannung mehr an diesen Kabeln anliegt. Erwärme jetzt vorsichtig den Schrumpfschlauch mit einer Heißluftpistole oder einem Feuerzeug.</li>
 </ul>
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../entwicklerboard">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Vorheriger Schritt 
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../vorbereitung-radaranschluss">
    Nächster Schritt <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>