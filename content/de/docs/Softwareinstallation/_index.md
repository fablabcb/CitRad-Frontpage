---
title: Softwareinstallation
description: Noch etwas Hirn gefällig? Als letzter Schritt vor dem Aufbau an der Straße muss die Software auf den Teensy
categories: []
tags: []
weight: 3
---

## Das brauchst du

<div class="row">
    <div class="col-md-6">

### Werkzeug
- Laptop/PC mit Linux oder Windows
- Datenkabel (Micro-USB)
- Aktuellste Version der [.hex-Datei](https://github.com/fablabcb/CitRad-SensorUnit/releases) (sensor.ino.hex)
- [Teensy-Loader](https://www.pjrc.com/teensy/loader.html) für dein Betriebssystem.

</div>
    <div class="col-md-6">

### Teile
- fertiger Sensor
       </div>
</div>

## So funktioniert es 

Der Hersteller des Teensy stellt auf seiner Website die Software (Teensy-Loader) zum Flashen für Linux, Windows und Mac bereit (s.o). Aus unserem Repository (ebenfalls oben verlinkt) bekommst du die nötige .hex-Datei. Jetzt kannst du den Sensor per Micro-USB-Kabel an deinen PC/Laptop anschließen, den Teensy-Loader starten und die .hex-Datei flashen. Folge einfach den Anleitungen auf der Hersteller-Website.

Beim Flashen wird außerdem die aktuelle Zeit an den Teensy übermittelt. Das ist wichtig, damit wir später die Daten dem Datum und der Tageszeit zuordnen können. Falls du irgendwann mal die Stromzufuhr über die Knopfzelle unterbrochen sein sollte (Defekt oder Tausch der Batterie), flashe vor der nächsten Messung die .hex-Datei einfach nochmal neu.

{{% alert color="primary" %}}
Der Teensy beginnt direkt nach dem Aufspielen der Software mit seiner Arbeit. Das bedeutet, dass auf der Speicherkarte bereits .csv- und .bin-Datein liegen können. Trenne jetzt am besten die Sensoreinheit vom Akkupack und lösche diese Dateien von der SD-Karte. Denn diese Daten solltest du später <strong>nicht</strong> versehentlich ins Portal laden.
{{% /alert %}}

### Flashen mit Arduino IDE

Falls du mit der Arduino IDE vertraut bist, steht es dir natürlich auch frei, [unser Repository](https://github.com/fablabcb/CitRad-SensorUnit) zu klonen und den Teensy selbst zu flashen.


<div class="d-flex justify-content-between">
  <a class="btn btn-sm btn-primary me-3 mb-4" href="../bauanleitung/zusammenbau">
<i class="fas fa-arrow-alt-circle-left me-2"></i> Vorheriger Schritt 
  </a>
  <a class="btn btn-sm btn-primary mb-4" href="../messanleitung">
    Nächster Schritt <i class="fas fa-arrow-alt-circle-right ms-2"></i>
  </a> 
  </div>