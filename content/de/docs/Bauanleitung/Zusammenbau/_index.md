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
        <figure class="figure">
          <img src="/parts/gehause_ges.png" alt="Gehäuse gesamt" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Gehäuse</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/akku.png" alt="Akku-Pack" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Akku-Pack</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/lasercut_fuesse.png" alt="Lasercut-Füße" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Lasercut-Füße</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/3d_radarhalter.png" alt="3D-Druck-Halterung für Radarmodul" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Radarhalterung</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/radarmodul.jpeg" alt="Radarmodul" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Radarmodul</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/microsd.png" alt="MicroSD-Karte" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">MicroSD-Karte</figcaption>
        </figure>
        <ul><li>Alles bisher Zusammengebaute</li>
        <li>5x M3x5mm Schrauben</li></ul>
      </div>
</div>

## So funktioniert es 

<div class="row">

### Adapterplatte montieren
{{% alert color="primary" %}}
Dieser Teil wird aktuell überarbeitet. Bitte etwas Geduld.{{% /alert %}}
    <div class="col-md-6">
       {{< imgproc gewindeschneiden Fit "600x400 webp" >}}Gewindeschneiden
{{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Für die Montage an Straßenlaternen oder den Rohren von Straßenschildern brauchen wir ein Zwischenstück zwischen Box und Pfahl. 
Gewinde in Befestigungslöcher (Rückseite) schneiden.
    </div>
</div>

<div class="row">
<div class="col-md-6">
       <div style="width: 400px; height: 300px; background-color: #cccccc; text-align: center; line-height: 200px;">
    Platzhalter
</div> </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Adapterplatte mit M5-Schrauben und den Unterlegschrauben (im Lasercut Teil enthalten) an Rückseite anschrauben.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->



### Grundplatte befestigen
<div class="row">
    <div class="col-md-6">
       {{< imgproc grundplatte_eingebaut Fit "600x400 webp" >}}Grundplatte mit Klettband für den Akku{{< /imgproc >}} </div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

<ul><li>Zuerst das Klettband mit der weichen Seite nach oben in die mittlere Öffnung einführen und in Richtung der Aussparung führen.</li>

<li>Dann die Grundplatte mit den losen Klettbandenden nach oben in das Gehäuse legen und festschrauben. Dabei ist die Orientierung der Platte innerhalb des Gehäuses egal.</li>
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
 Das Radarmodul vorsichtig in die Öffnung der 3D-Druck-Halterung einsetzen. 
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
- Danach mit 3 Schrauben das Audioshield an der Halterung befestigen. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Radarmodul-Rahmen mit Adapterplatten verschrauben
<div class="col-md-6">
       {{< imgproc standfuss Fit "600x400 webp" >}} Angeschraubte Standfüße {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Jetzt kannst du die Standfüße (aus dem Lasercutter) an die 3D-Druck-Halterung anschrauben. Schraube sie nicht zu fest an, damit du das Modul noch bewegen kannst. Die V-förmigen Enden sollten in die gleiche Richtung wie das Radarmodul zeigen. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Micro-SD-Karte einsetzen
<div class="col-md-6">
       {{< imgproc 3d Fit "600x400 webp" >}} Platzhalter Micro SD {{< /imgproc >}} </div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Micro-SD in Audioshield   <span style="background-color:yellow">[Brauchts da einen ExtraSchritt mit Bild?]</span>
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
Die Radareinheit neben den Akku in die dafür vorgesehenen Schlitze stecken. Gehalten wird das Ganze später durch den Deckel.
<br>
{{% alert color="primary" %}}
Die Radareinheit muss richtig in den vorgesehenen Schlitzen stecken. Also nicht verkantet. Sonst lässt sich der Deckel nicht schließen. 
{{% /alert %}}
Die Radareinheit wird nicht festgeschraubt, damit man später unkompliziert an die SD-Karte heran kommt.    

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

**Glückwunsch! Der Hardwareteil ist abgeschlossen!**  Bevor du den Deckel aufs Gehäuse schrauben kannst, musst du noch die <a href="/docs/softwareinstallation/">Software auf das Teensy Entwicklerboard flashen</a> 

<hr class="my-4">

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../elektronik/vorbereitung-radaranschluss">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Vorheriger Schritt 
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../../softwareinstallation/">
    Nächster Schritt <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>