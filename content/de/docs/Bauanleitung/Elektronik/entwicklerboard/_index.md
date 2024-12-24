---
title: Teensy Entwicklerboard
description: >
  Alle Vorbereitungsschritte für den Teensy Entwicklerboard 
date: 2024-01-09
weight: 1
---
## Das brauchst du

<div class="row">
    <div class="col-md-6">
       <h3>Werkzeug</h3>
       <ul>
       <li><img src="/icons/cutter.webp" alt="Cuttermesser" width="200"/>Cuttermesser</li>
       <li><img src="/icons/lötkolben.webp" alt="Lötkolben" width="200"/>Lötkolben + Lötzinn</li>
       <li>Mikro-USB-Kabel + 5V Netzteil/USB-Port des Laptops</li>
       </ul>
</div>
    <div class="col-md-6">
<h3>Teile</h3>
<ul>
       <li>Teensy Entwicklerboard</li>
        <li>Knopfzellenhalter</li>
        <li>Schrumpfschlauch (1cm)</li>
       </ul> 
       </div>
</div>

## So funktioniert es 



<div class="row">

<div class="row">

### Funktionsprüfung
<div class="col-md-6">
      {{< imgproc control Fit "600x400 webp" >}} Die Rote LED sollte bei Stromversorgung per USB leuchten.
{{< /imgproc >}} 

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

Der Teensy sollte grundsätzlich funktionieren, bevor du mit den Anpassungen beginnst. Schließe das Teensy Entwicklerboard per USB an eine Stromquelle an. Die rote Kontrollleuchte sollte durchgehend leuchten. Ziehe das USB-Kabel jetzt wieder ab.<br>
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

### Kontakt für USB-Stromversorgung unterbrechen
<div class="col-md-6">
       
{{< imgproc cut_contact_done Fit "600x400 webp" >}} Die Verbindung zwischen den beiden rechteckigen Kontakten (rot eingekreist) muss entfernt werden. Kreis 1 und 2 zeigen wie. 
{{< /imgproc >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
<p>Der Teensy Entwicklerboard soll für dieses Projekt per Akkupack mit Strom versorgt werden. Damit er nicht versehentlich per Akkupack und USB mit Strom versorgt wird, müssen wir zuerst die Stromversorgung per USB deaktivieren. </p>

<p>Im Foto sind zwei eckige Kontakte <span style="border: 2px solid #a6113a">rot eingekreist</span>. Die beiden Leiterbahnen werden durch eine kleine Leiterbahn verbunden (<span style="border: 2px solid #00ffffff"> siehe Pfeil in Kreis 1</span>). Diese musst du mit dem Cuttermesser wegkratzen bis es in etwa so aussieht wie <span style="border: 2px solid #00ffffff">in Kreis 2.</span> </p>
<p>Zur Kontrolle schließt du den Teensy jetzt wieder per USB an eine Stromquelle an.
{{% alert color="primary" %}}
Nur wenn die rote Kontrolleuchte des Teensy **nicht mehr** leuchtet, kannst du fortfahren. Andernfalls musst du nochmal nacharbeiten.
{{% /alert %}}</p>
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->



<div class="row">

### Knopfzellenhalter vorbereiten
<div class="col-md-6">
      {{< imgproc knopfzelleschrumpfschlauch Fit "600x400 webp" >}} Knopfzellenhalter mit Schrumpflauch über den Anschlusskabeln
{{< /imgproc >}} 

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Durch eine Knopfzelle versorgst du den Teensy auch dann mit Strom wenn er gerade nicht am Akku hängt. So verliert er seine Uhrzeit- und Datumseinstellungen nicht, während du den Akku lädst. 
- Bevor du den Knopfzellenhalter an den Teensy löten kannst, muss über beide Kabel ein kleines Stück Schrumpfschlauch gezogen (aber noch nicht erwärmt) werden. Das dient später der Zugentlastung.<br>
{{% alert color="primary" %}}
Die Knopfzelle bitte erst einlegen, wenn du in der Anleitung dazu aufgefordert wirst. Andernfalls drohen Kurzschlüsse während des Lötens. 
{{% /alert %}}
</div>
</div>
<hr class="my-4"> <!-- Trennlinie -->
<div class="row">

### Knopfzellenhalter anlöten
<div class="col-md-6">
      {{< imgproc teensy_knopf Fit "600x400 webp" >}} Angelöteter Knopfzellenhalter
{{< /imgproc >}} 

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Das rote Kabel muss an Pin 32, das schwarze an Pin 28 gelötet werden.<br>

{{% alert color="primary" %}}
Wichtig ist, dass die Kabel auf der Platinenunterseite nicht überstehen dürfen. Später wird hier der SD-Karten-Slot vom Audio-Board liegen. Dieser darf keinen Kontakt zu den Lötstellen bekommen.   
{{% /alert %}}
</div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Vorheriger Schritt 
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../audioshield">
    Nächster Schritt <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a>
</div>