---
title: Vorbereitung Radaranschluss
description: >
  Für die Spannungsversorgung des Radarmoduls musst du einen Spannungswandler einbauen. Außerdem musst du Anschlüsse für den Datenaustausch zwischen den Komponenten vorbereiten. 
date: 2024-01-09
weight: 3
---
## Das brauchst du

<div class="row">
    <div class="col-md-6">
       <h3>Werkzeug</h3>
       <ul>
       <li><img src="/icons/spitzzange.webp" alt="Spitzzange" width="200"/>Spitzzange</li>
       <li><img src="/icons/lötkolben.webp" alt="Lötkolben" width="200"/>Lötkolben + Lötzinn</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Teile</h3>
<ul>
       <li>Teensy Entwicklerboard + Audioshield aus vorherigem Schritt</li>
        <li>Spannungswandler</li>
        <li>Header 6-Pin</li>
        <li>Header 4-Pin</li>
        <li>Kabel (ca. 4 cm)</li>
       </ul> 
       </div>
</div>

## So funktioniert es 

<div class="row">

### Spannungwandler und Teensy verbinden
<div class="col-md-6">
       {{< imgproc spannungswandler1 Fit "600x400 webp" >}} Spannungswandler, angelötet an GND und 3.3V des Teensy {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

<p>Nicht im Foto: Lege den Spannungswandler mit der Beschriftung nach oben und den Füßchen zu dir zeigend vor dich hin. Die beiden linken Füßchen biegst du jetzt so nah wie möglich am Spannungwandler um 90° nach oben.</p>
<p>Siehe Foto: Nun legst legst du den Spannungswandler mit den der Beschriftung nach unten auf den Teensy. Dabei darauf achten, dass die umgebogenen Füßchen jeweils links an den zwei alleinstehenden Pins, die aus 3.3V-Kontakt und GND-Kontakt (rechts daneben) herausragen, anliegen.</p>
<p>Jetzt kannst du beide Kontaktstellen verlöten.</p>  
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->




<div class="row">

### Steckerverbindung vorbereiten (Teil 1: Header 6-Pin)
<div class="col-md-6">

{{< tabpane text=true right=true >}}
  {{% tab header="Biegen:" disabled=true /%}}
  {{% tab header="1." %}}
  
{{< imgproc 6-pin-rem-pin Fit "600x400 webp" >}} Pin 1 herausgezogen {{< /imgproc >}}

  {{% /tab %}}
  {{< tab header="2.">}}
    
{{< imgproc 6-pin_bend1 Fit "600x400 webp" >}} Pin 5 und 6: Erste Biegung um 90° nach hinten {{< /imgproc >}}

  {{< /tab >}}

  {{% tab header="3." %}}

{{< imgproc 6-pin_bend2 Fit "600x400 webp" >}} Zweite Biegung nach unten {{< /imgproc >}}
  {{% /tab %}}

  {{< tab header="4.">}}
    
{{< imgproc shield_line_in Fit "600x400 webp" >}} Beide Pins angelötet am Line-In des Audioshields {{< /imgproc >}}

  {{< /tab >}}
{{< /tabpane >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Klicke dich durch die Biege-Tabs (1.-4.), um detaillierte Fotos zu den einzelnen Schritten zu sehen.
- Pin 1 (ganz links) aus dem Stecker ziehen. Er wird nicht mehr benötigt.
- Pin 5 und 6 (ganz rechts) zuerst um 90° nach hinten biegen. Dann mit etwa 4mm Abstand um ca. 75 grad nach unten biegen. Beide Pins müssen an die Line-In Kontakte des Audioshields heranreichen und dort festgelötet werden. 

</div>
</div>
<div class="row">
<div class="col-md-6">
       {{< imgproc prep_spannung Fit "600x400 webp" >}} Angelöteter Header 6-Pin {{< /imgproc >}}
</div>
<div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

<ul>
<li>Der Header 6-Pin muss am Ende auf das Radarmodul passen. Es kann helfen, wenn du das Radarmodul zum Zurechtbiegen der Pins schonmal am Audioshield befestigst. Die nötigen Schritte werden <a href="/docs/bauanleitung/zusammenbau/#radarmodul-in-rahmen-stecken">ab hier</a> im Kapitel "Zusammenbau" erklärt.
<li style="border: 2px solid #7adef1ff"> Enable (Pin 2) zu Pin 17 des Teensy biegen und zusammenlöten (passt gerade so).</li>
<li style="border: 2px solid #a6113aff"> Gnd (Pin 4) und Vcc (Pin 3) schräg mit dem Output des Spannungswandlers verbinden (siehe Foto). Hier muss man eventuell mit Lötzinn oder einem kurzen Draht überbrücken. Das Foto am Ende der Seite zeigt nochmal eine Draufsicht, die hilfreich sein kann.</li>
</ul>
{{% alert color="primary" %}}
Aufpassen dass keine Querverbindung besteht. Eventuell die Drähte etwas auseinander biegen.
{{% /alert %}}

</div>
</div>
<div class="row">

</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Steckerverbindung vorbereiten (Teil 2: Header 4-Pin)
<div class="col-md-6">
       {{< imgproc radar_stecker Fit "600x400 webp" >}} Vorbereiteter Header 4-Pin. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

 - Das Kabel (5cm) musst du mit einem Ende an einem der inneren Kontakte des Header 4-Pins anlöten.

     </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->
<div class="row">

### Endergebnis
<div class="col-md-6">
       {{< imgproc radar_stecker_prep2_pin Fit "600x400 webp" >}} Endergebnis nach Ausführung aller Schritte {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Das andere Ende des Kabels lötest du vom Header 4-Pin kommend an GND (lineout oder mic) des Audioshields .
- Am Ende sollte alles wie auf dem Foto aussehen. 

    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../vorbereitung-radaranschluss">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Vorheriger Schritt 
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../../zusammenbau/">
    Nächster Schritt <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>