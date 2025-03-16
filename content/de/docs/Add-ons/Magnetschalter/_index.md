---
title: Magnetschalter
description: Mit dem Magnetschalter kannst du den Sensor starten/stoppen, ohne jedes Mal das Gehäuse aufschrauben zu müssen.
categories: []
tags: []
weight: 5
---
## Vorbermerkung
Der Magnetschalter ermöglicht dir, den Sensor von außen zu starten bzw. zu stoppen. Wir nutzen dafür einen Reedkontakt (Öffner), den wir von innen an der Gehäusewand befestigen. Wird jetzt von außen ein Magnet an die richtige Stelle gehalten, wird der Stromkreis unterbrochen. Wenn du also nach der Montage den Magnet mitnimmst, fängt der Sensor an zu messen. Kommst du zum Abbau zurück, schiebst du den Magnet wieder auf und stoppst damit die Messung.

Du bist völlig frei, wo du den Reedkontakt in deinen Stromkreis einbaust und wo am Gehäuse er positioniert wird. Hauptsache die Stromzuvor zum Teensy kann durch den Kontakt unterbrochen werden. 


Die unten verlinkten 3D-Druck-Teile sind auf den ebenfalls verlinkten Reedkontakt ausgerichtet und möglichst klein gehalten. Solltest du an den Teilen was verändern wollen, kannst du diese [FreeCad-Projektdatei](https://github.com/fablabcb/CitRad-SensorUnit/raw/refs/heads/develop/Hardware/Addons/magneticOnOFF-CitRad.FCStd) nutzen.
{{% alert color="primary" %}}
Es kommt auf die richtige Ausrichtung des Magnets zum Reedkontakt an. Wenn du andere Kontakte verwendest, kann es je nach Funktionsweise sein, dass du dir eine ganz eigene Magnethalterung konstruieren musst. 
{{% /alert %}}

## Das brauchst du

<div class="row">
    <div class="col-md-6">

### Werkzeug
<ul>
       <li><img src="/icons/lötkolben.webp" alt="Lötkolben" width="200"/>Lötkolben + Lötzinn</li>
       <li><img src="/icons/abiso.webp" alt="Lötkolben" width="200"/>Abisolierzange</li>
       <li>Schrumpfschlauch (5cm, optional)</li>
       <li>Sekundenkleber</li>
       </ul>

</div>
    <div class="col-md-6">

### Teile
- fertiger Sensor
- [Reedkontakt (Öffner)](https://www.amazon.de/dp/B088CQL44X)
- [Kontakthalter innen](/parts/ReedSensorHolder_mOO-Citrad.stl) (3D-Druck-Teil)
- [Magnetaufnahme](/parts/MAgnetMount_mOO-Citrad.stl) (3D-Druck-Teil)
- [Magnethalter](/parts/MagnetSlider_mOO-Citrad.stl) (3D-Druck-Teil)
- etwas extra Kabel (optional)
       </div>
</div>

## So funktioniert es 
<div class="row">

### Vorbereitung

<div class="col-md-6">
       {{< imgproc MagneticSwitch_allparts.png Fit "600x400 webp" >}} Alle benötigten 3D-Druck-Teile {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">


 Diese drei Teile musst du mit einem 3D-Drucker fertigen. Sie sind so konstruiert, dass sowohl Reedkontakt als auch Magnet direkt an der Gehäusewand aufliegen. Falls du eigene Designs verwenden willst, musst du das ebenfalls bedenken, damit der Reedkontakt ausgelöst wird.
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->
<div class="row">

### Ankleben der Halter

<div class="col-md-6">
       {{< imgproc reedHolder.jpg Fill "600x300 webp Top" >}} Alle benötigten 3D-Druck-Teile {{< /imgproc >}}
       {{< imgproc magnetMount.jpg Fill "600x300 webp Top" >}} Alle benötigten 3D-Druck-Teile {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

1. Zuerst klebst du den Reedkontakt-Halter ins Gehäuse. Dabei darauf achten, dass das kleine Dreieck in Richtung Gehäuse zeigt und die Spitze des Dreiecks nicht höher positioniert ist, als als die Vertiefung am Gehäuserand an dem der Deckel später einrastet.
2. auf der Außenseite klebst du jetzt die Magnetaufnahme so an, dass das deren Dreieck genauso ausgerichtet und auf gleicher Höhe (Augenmaß reicht aus) positioniert ist, wie das Dreieck auf des Reedkontakt-Halters auf der Innenseite. Es ist außerdem wichtig, dass der schmale Teil der Schräge in Richtung des Gehäuses zeigt. Sonst ist später ein Aufschieben des Magnets unmöglich. 

 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->
<div class="row">

### Verkabelung des Reedkontakts

<div class="col-md-6">
       {{< imgproc wiringReed.jpeg Fit "600x400 webp" >}} Steckbare Integrationsvariante macht die Nutzung des Magnetschalters optional. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

Du kannst frei wählen, an welche Stelle du den Reedkontakt in den Stromkreis einbaust. Du kannst ihn fest verlöten oder wie hier vorgestellt mit extra Stecker und Buchse als optionales Teil zusteckbar machen. 

Sobald die Verkabelung abgeschlossen ist, muss der Reedkontakt mit der viereckigen Erhebung in richtung Gehäuseinneres in den Halter gesteckt werden. Dabei darauf achten, dass er wirklich ganz an der Gehäusewand anliegt. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Richtige Orientierung des Magneten testen

<div class="col-md-6">
       {{< imgproc magnetMountMagnet.jpg Fill "600x300 webp Top" >}} Magnettestweise eingesteckt um Orientierung zu testen {{< /imgproc >}}
       {{< imgproc magnetHolderMagnet.jpg Fill "600x300 webp Center" >}} Im Magnethalter eingeklebter Magnet. {{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

Der Reedkontakt wird den Stromkreis nur dann zuverlässig unterbrechen, wenn der Magnet in der richtigen Orientierung angelegt wird. Es kommt also darauf an, welche Seite des Magnets nach links zeigt und welche nach rechts. Um die richtige Orientierung herauszufinden steckst du den Magneten ohne seinen Halter (3. 3D-Druck-Teil) in die Aufnahme und verbindest den restlichen Stromkreis. Wenn der Sensor aus bleibt (keine LEDs leuchten/blinken), hast du die richtige Orientierung bereits gefunden. Andernfalls drehe den Magneten um und wiederhole den Test. Wahlweise kannst du natürlich auch mit einem Multimeter auf Durchgang messen. 

Jetzt wo du die richtige Orientierung weißt, kannst du den Magneten in den Halter einkleben. Der Halter ist so konstruiert, dass er nur in einer Richtung aufschiebbar ist (kleine Sperrnasen an einem Ende). Klebe den Magneten also so in den Halter, dass er beim Aufschieben richtig orientiert ist. Den Magneten dabei unbedingt vollständig in die Aufnahme drücken, damit nachher die Abstände stimmen. 
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->

<div class="row">

### Die Finale "Aus"-Position

<div class="col-md-6">
       {{< imgproc offPosition.jpg Fill "600x300 webp Center" >}} So sieht die Off-Position aus.{{< /imgproc >}}
</div>
    <div class="col-md-6" style="display: flex; flex-direction: column; justify-content: center;">

Wenn alles fertig geklebt und Zusammengesteckt ist, kannst du den Stromkreis komplett verbingen. Solange der Magnet an Ort und Stelle ist, wird kein Strom fließen. Erst wenn du den Magnethalter/Magnet entfernst beginnt die Messung.  
    </div>
</div>
<hr class="my-4"> <!-- Trennlinie -->