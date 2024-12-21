---
title: Teensy Mikroprozessor
description: >
  Alle Vorbereitungsschritte für den Teensy Mikroprozessor 
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
       <li>Teensy Mikroprozessor</li>
        <li>Knopfzellenhalter</li>
        <li>Schrumpfschlauch</li>
       </ul> 
       </div>
</div>

## So funktioniert es 
<div class="row">

### Kontakt für USB-Stromversorgung unterbrechen
<div class="col-md-6">
       
{{< imgproc cut_contact_done Fit "600x400 webp" >}}Foto 1: Die Verbindung zwischen den beiden rechteckigen Kontakten (rot eingekreist) muss entfernt werden.
{{< /imgproc >}}
{{< imgproc cut_contact Fit "600x400 webp" >}}Foto 2: Wegkratzen der Verbindung zwischen den beiden Kontakten
{{< /imgproc >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
<p>Der Teensy Mikroprozessor soll für dieses Projekt per Akkupack mit Strom versorgt werden. Damit er nicht versehentlich per Akkupack und USB mit Strom versorgt wird, müssen wir zuerst die Stromversorgung per USB deaktivieren. </p>

<p>Zunächst schließt du den Teensy Mikroprozessor per USB an eine Stromquelle an, um zu überprüfen, ob er ordnungsgemäß funktioniert. Die rote Kontrollleuchte sollte durchgehen an sein. Ziehe das USB-Kabel jetzt wieder ab. </p>

<p>In Foto zwei sind zwei eckige Kontakte rot eingekreist. Die beiden Leiterbahnen werden durch eine kleine Leiterbahn verbunden. Diese musst du mit dem Cuttermesser wegkratzen. </p>
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Prüfen, ob Kontakt unterbrochen ist
<div class="col-md-6">
      {{< imgproc control Fit "600x400 webp" >}} Das rote Licht darf <strong>NICHT</strong> mehr leuchten.
{{< /imgproc >}} 

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

Um zu überprüfen, ob der Kontakt vollständig unterbrochen wurde, schließt du den Teensy per USB-Kabel an eine 5V Spannungsquelle (USB-Netzteil oder Laptop) an.<br>
 {{% alert color="primary" %}}
Nur wenn die rote Kontrolleuchte des Teensy **nicht mehr** leuchtet, kannst du fortfahren. Andernfalls musst du nochmal nacharbeiten.
{{% /alert %}}
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
Wichtig ist dass die Kabel auf der Platinenunterseite nicht überstehen dürfen. Später wird hier der SD-Karten-Slot vom Audio-Board liegen. Dieser darf keinen Kontakt zu den Lötstellen bekommen.   
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