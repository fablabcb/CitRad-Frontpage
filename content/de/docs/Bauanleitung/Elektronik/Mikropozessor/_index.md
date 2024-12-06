---
title: Mikroprozessor
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
       {{< imgproc cut_contact Fit "600x400 webp" >}}Foto 1: Kontaktunterbrechung
{{< /imgproc >}}
{{< imgproc cut_contact_done Fit "600x400 webp" >}}Foto 2: Die Lücke zwischen den beiden rechteckigen Kontakten haben wurde mit dem Messer erzeugt.
{{< /imgproc >}}

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Der Teensy kann direkt über die Platine oder per USB-Kabel mit Strom versorgt werden. Er darf allerdings nicht über beide Wege gleichzeitig angeschlossen werden. Um das auszuschließen, musst du Stromversorgung per USB kappen, sodass die Stromversorgung nur noch über den Akkupack erfolgen kann. Das geht, indem du mit einem Cuttermesser an der richtigen Stelle ein Stück freikratzt (siehe Foto 1). Am Ende muss es so aussehen wie in Foto 2.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Prüfen, ob Kontakt unterbrochen ist
<div class="col-md-6">
      {{% imgproc control Fit "600x400 webp" %}} Das rote Licht darf <strong>NICHT</strong> mehr leuchten.
{{% /imgproc %}} 

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
      {{% imgproc knopfzelleschrumpfschlauch Fit "600x400 webp" %}} Knopfzellenhalter mit Schrumpflauch über den Anschlusskabeln
{{% /imgproc %}} 

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

- Durch eine Knopfzelle versorgst du den Teensy auch dann mit Strom wenn er gerade nicht am Akku hängt. So verliert er seine Uhrzeit- und Datumseinstellungen nicht, während du den Akku lädst. 
- Bevor du den Knopfzellenhalter an den Teensy löten kannst, muss über beide Kabel ein kleines Stück Schrumpfschlauch gezogen (aber noch nicht erwärmt) werden. Das dient später der Zugentlastung.<br>
{{% alert color="primary" %}}
Die Knopfzelle bitte erst ganz am Ende einsetzen. Andernfalls drohen Kurzschlüsse während des Lötens. 
{{% /alert %}}
</div>
</div>
<hr class="my-4"> <!-- Trennlinie -->
<div class="row">

### Knopfzellenhalter anlöten
<div class="col-md-6">
      {{% imgproc teensy_knopf Fit "600x400 webp" %}} Angelöteter Knopfzellenhalter
{{% /imgproc %}} 

</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">
Das rote Kabel muss an Pin 32, das schwarze an Pin 28 gelötet werden. 
</div>
</div>
<hr class="my-4"> <!-- Trennlinie -->
