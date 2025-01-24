---
title: Zusammmenbau
description: Nachdem du die Elektronik erledigt hast, muss das Gehäuse vorbereitet und alles zusammengebaut werden.
categories: []
tags: []
weight: 6
---

## Das brauchst du

<div class="row">
    <div class="col-md-6">
       <h3>Werkzeug</h3>
       <ul>
       <li><img src="/icons/screwdriver.webp" alt="Schraubenzieher" width="200"/>Schraubenzieher</li>
        <li><img src="/icons/gewinde.webp" alt="Lötkolben" width="200"/>Gewindeschneider Mx</li>
        <li><img src="/icons/cutter.webp" alt="Cuttermesser" width="200"/>Cuttermesser</li>
       </ul>
    </div>
    <div class="col-md-6 col-sm-6 col-xs-12">
    <h3>Teile</h3>

    
  - Gehäuse
  - Akku-Pack
  - Lasercut-Füße
  - Lasercut-Adapterplatte
  - Radarhalterung
  - Radarmodul
  - MicroSD-Karte
  - Alles bisher Zusammengebaute
  - 5x M3x5mm Schrauben
  - 4x M3x14mm Zylinderkopfschrauben



        
      </div>
</div>

## So funktioniert es 

<div class="row">

### Adapterplatte montieren


<div class="col-md-6">
       {{< imgproc gewinde Fit "600x400 webp" >}}Gewindeschneiden
{{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Für die Montage an Straßenlaternen oder den Rohren von Straßenschildern brauchen wir ein Zwischenstück zwischen Box und Pfahl. 
Schneide mit dem M3 Gewindeschneider ein Innengewinde in jedes der vier Löcher der Adapterplatte aus dem Lasercutter 
    </div>
</div>

<div class="row">
<div class="col-md-6">
       <div style="width: 400px; height: 300px; background-color: #cccccc; text-align: center; line-height: 200px;">
    Dieses Foto fehlt noch
</div> </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Nimm jetzt die 4 M3x14mm Zylinderkopfschrauben, führe sie jeweils durch die Aussparungen an den Ecken des Gehäußes (von innen nach außen) und verschraube sie mit der Adapterplatte.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->



### Grundplatte befestigen
<div class="row">
    <div class="col-md-6">
       {{< imgproc grundplatte_eingebaut Fit "600x400 webp" >}}Grundplatte mit Klettband für den Akku{{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

<ul><li>Zuerst das Klettband mit der weichen Seite nach oben in die mittlere Öffnung einführen und in Richtung der Aussparung führen.</li>

<li>Dann die Grundplatte mit den losen Klettbandenden nach oben in das Gehäuse legen und mit M3x5mm Schrauben festschrauben. Dabei ist die Orientierung der Platte innerhalb des Gehäuses egal.</li>
</ul>
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->



<div class="row">

### Akku befestigen
<div class="col-md-6">
       {{< imgproc akku Fit "600x400 webp" >}}Akkupack im Gehäuse{{< /imgproc >}}</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Akku mit Kletterverschluss an Grundplatte befestigen.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->


<div class="row">


### Radarmodul in Rahmen stecken
<div class="col-md-6">
       {{< imgproc 3d Fit "600x400 webp" >}} Vorderseite {{< /imgproc >}}
       {{< imgproc _back Fit "600x400 webp" >}} Rückseite {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
 Das Radarmodul vorsichtig so in die 3D-Druck-Halterung einsetzen, dass die 4 Pins den Spalt der Halterung herausragen und die 6 Pins auf der gegenüberliegenden Seite durch die große Öffnung ragen. Das Modul sollte am Ende fest in dem 3D-Druck-Teil stecken.
    </div>
</div>
<hr class="my-4"> 
<div class="row">

### Teensy/Audioshield aufstecken und verschrauben
<div class="col-md-6">
       {{< imgproc all Fit "600x400 webp" >}} Vorderseite {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Beim Aufsetzen von Teensy&Audoshield auf die Pins des Radarmoduls musst du nur darauf achten, dass die Löcher für die Schrauben im Audioshield auf die der 3D-Druck-Halterung passen.
- Dann kannst du zuerst den 6-Pin-Stecker verbinden und dann
- Den 4-Pin-Stecker so einstecken, dass das Kabel am zweiten Pin (vom Klinkenanschluss aus gesehen) angelötet ist. 
- Danach mit 3 M3x5mm-Schrauben das Audioshield an der Halterung befestigen. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Radarmodul-Rahmen mit Adapterplatten verschrauben
<div class="col-md-6">
       {{< imgproc standfuss Fit "600x400 webp" >}} Angeschraubte Standfüße {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Jetzt kannst du die Standfüße aus dem Lasercutter mit je einer M3x5mm-Schraube an die 3D-Druck-Halterung anschrauben. Schraube sie nicht zu fest an, damit du das Modul noch bewegen kannst. 
- Die längere der beiden langen Kanten zeigt dabei jeweils in Richtung des breiten Endes der 3D-Druck-Halterung.Der Überstand an der kurzen Kante zeigt vom Radarmodul weg.


Die Standfüße stehen hier nur für das Foto in der Grundplatte. Die Grundplatte brauchst du hier nicht, sie kann im Gehäuse verschraubt bleiben.  
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Micro-SD-Karte einsetzen
<div class="col-md-6">
       {{< imgproc microsd Fit "600x400 webp" >}} MicroSD-Karte im Slot des Audioshields {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Der Slot für die MicroSD-Karte befindet sich jetzt zwischen Teensy und Audioshield. Die Micro-SD-Karte muss mit den Kontakten nach unten vorsichtig bis zum Anschlag in den Slot des Audioshield geschoben werden.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

### Knopfzellenhalter
<div class="row">
    <div class="col-md-6">
       {{< imgproc knopfzelle Fit "600x400 webp" >}} Knopfzellenhalter mit Knopfzelle {{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Knopfzelle in Knopzellenhalter einsetzen. Der Pluspol der Knopfzelle muss in Richtung des Deckels zeigen. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->


<div class="row">

### Elektronik ins Gehäuse
<div class="col-md-6">
       {{< imgproc alltogether Fit "600x400 webp" >}} Vorderseite {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Die Radareinheit neben den Akku in die dafür vorgesehenen Schlitze stecken. Dabei Zeigt der Einschub für die MicroSD-Karte vom Akku weg. Gehalten wird das die Radareinheit durch den aufgeschraubten Deckel, So kommst du jederzeit gut an die MicroSD-Karte heran. 
<br>
{{% alert color="primary" %}}
Der Platz ist hier etwas begrenzt. Aber mit etwas Fingerspitzengefühl, kann man die Radareinheit einsetzen, ohne dass sie sich verkantet. Lockere zur Not den Akku etwas, um mehr Spiel zu haben.  
{{% /alert %}}
 </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Gehäusedeckel abdichten
<div class="col-md-6">
       
{{< imgproc dichtung_schneiden Fill "400x300 webp" >}}
Einkürzen der Gummidichtung.
{{< /imgproc >}}

       
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Die Gummidichtung einmal ringsum in die Nut einlegen und den Überstand mit einem Cuttermesser abtrennen. <br>

{{% alert color="primary" %}}
Dieser Schritt ist wichtig, damit keine Feuchtigkeit in das Gehäuse eindringen kann.
{{% /alert %}}


</div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

**Glückwunsch! Der Hardwareteil ist abgeschlossen!**  Bevor du den Deckel aufs Gehäuse schrauben kannst (mitgelieferte oder M4x20mm Sicherheitsschrauben), musst du noch die <a href="/docs/softwareinstallation/">Software auf das Teensy Entwicklerboard flashen</a> 

<hr class="my-4">

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../elektronik/vorbereitung-radaranschluss">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Vorheriger Schritt 
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../../softwareinstallation/">
    Nächster Schritt <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>