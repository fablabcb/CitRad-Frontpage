---
title: Softwareinstallation
description: Noch etwas Hirn gefällig? Als letzter Schritt vor dem Aufbau an der Straße muss die Software auf den Teensy
categories: []
tags: []
weight: z
---

## Das brauchst du

<div class="row">
    <div class="col-md-6">

### Werkzeug
- Laptop/PC mit Linux oder Windows
- Datenkabel (Micro-USB)
- Aktuellste Version der [.hex-Datei](https://github.com/fablabcb/CitRad-SensorUnit/releases) (sensor.ino.hex)

</div>
    <div class="col-md-6">

### Teile
- fertiger Sensor
       </div>
</div>

## So funktioniert es 

Die einfachste Möglichkeit, die Software auf den Teensy zu bekommen, ist das flashen einer bereits kompilierten Hex-Datei unter Linux. Wenn du kein linux-basiertes Betriebssystem hast, springe zu [Windows](#windows).

{{< tabpane text=true right=false >}}
  {{< tab header="Wähle dein Betriebssystem:" disabled=true />}}
  {{< tab header="Linux" >}}
  
<ol>
<li>Zum Flashen der .hex-Datei benötigst du den <strong>teensy-loader-cli</strong>. Er sollte in den Paketquellen gängiger Distributionen enthalten sein. Falls das auf deine Distro nicht zutrifft, beziehe ihn nach der Anleitung auf der <a href="https://www.pjrc.com/teensy/loader.html">Website des Herstellers</a>.</li>
<li>Sind .hex-Datei und teensy-loader-cli bereit, verbinde den fertigen Sensor per USB-Kabel mit deinem Laptop/PC und setze die Speicherkarte ein, falls sie noch nicht eingesetzt ist.</li>
<li>Auf dem Terminal nun folgendes ausführen:

{{< card code=true header="**bash**" lang=C >}}
teensy_loader_cli -v --mcu=teensy40 -w %Pfad zu der Hex-Datei% 
{{< /card >}}

<br>Folge den Anweisungen auf dem Bildschirm folgen (den Knopf auf dem Teensy drücken). Wenn das Program einen Fehler meldet (<strong>Programming...error writing to Teensy</strong>), den Befehl einfach nochmal ausführen. Wenn das Kommando mit <strong>Booting</strong> endet, hat alles geklappt.</li>
<li>Damit später deine Daten mit der richtigen Uhrzeit verstehen sind, musst du noch folgenden Befehl ausführen, um die Uhrzeit einzustellen. </li>

{{< card code=true header="**bash**" lang="C" >}}
date -u +T%s % /dev/ttyACM0
{{< /card >}}
<br>
Glückwunsch, die Einrichtung ist abgeschlossen! Bitte Beachte die Hinweise am Ende der Seite.
{{< /tab >}}

  
  {{< tab header="Windows" >}}   

<ol>
<li>Lade dir den Teensy Loader für Windows von der <a href="https://www.pjrc.com/teensy/loader_win10.html">Herstellerseite</a> herunter.</li>
<li>Verbinde den fertigen Sensor per USB-Kabel mit deinem Laptop/PC und setze die Speicherkarte ein, falls sie noch nicht eingesetzt ist</li>
<li>Drücke einmal, wie in der Anleitung des Herstellers beschrieben, den Knopf am Teensy, um in den Program Mode zu gelangen</li>
<li>Nun kannst du über den File-Dialog die runtergeladene .hex-Datei (s. "Was brauchst du") auswählen und auf den Teensy flashen.</li>
<li>Zeiteinstellung falls nötig</li>
</ol>

<br>
Glückwunsch, die Einrichtung ist abgeschlossen! Bitte Beachte die Hinweise am Ende der Seite


{{< /tab >}}

{{< /tabpane >}}

{{% alert color="primary" %}}
Der Teensy beginnt direkt nach dem Aufspielen der Software mit seiner Arbeit. Das bedeutet, dass auf der Speicherkarte bereits .csv- und .bin-Datein liegen können. Trenne jetzt am besten die Sensoreinheit vom Akkupack und lösche diese Dateien von der SD-Karte. Denn diese Daten solltest du später <strong>nicht</strong> versehentlich ins Portal hochladen.
{{% /alert %}}


## Alternative zum Setzen der Zeit

Wenn kein Linux-System zur Verfügung steht und die Software vom Hersteller die Zeit nicht setzt, besteht eine Alternative darin, die Zeit über eine App oder ein anderes Programm zu setzen. Im Prinzip muss nur eine Zeichenkette der Art "T1720883807" an den Teensy geschickt werden. Möglich ist das z.B. über [diese App](https://play.google.com/store/apps/details?id=de.kai_morich.serial_usb_terminal&hl=de) oder die Arduino IDE.

Die Zeichenkette setzt sich aus dem Buchstaben "T" und der aktuellen UNIX-Zeit in UTC zusammen. Diese bekommt man von [hier](https://www.unixtimestamp.com/de). Einfach die große Zahl oben rechts kopieren und ein "T" davor schreiben. Die Zeit muss nicht exakt sein und man kann einfach ein paar Sekunden draufrechnen.

### Arduino IDE

- installieren
- Serial Monitor öffnen und mit dem Teensy verbinden
- aktuelle Zeit als Befehl senden, z.B. "T1720883807"

### App "USB Serial Terminal"

Zuerst muss sicher gestellt werden, dass man den Sensor auch mit dem Handy verbinden kann! Für die Verbindung von (wahrscheinlich) USB-C zu Micro-USB am Sensor benötigt man einen entsprechenden USB-Adapter.

Sind Handy und Sensor verbunden, öffnet man die App, geht im Menü auf "USB Devices" und wählt den ersten Eintrag aus (z.B. "Serial device - CDC - Port 1"). In der folgenden Ansicht sollten dann direkt schon Nachrichten vom Teensy auftauchen. Jetzt gibt man unten den passenden Zeit-Befehl ein und drückt auf senden. Der Teensy antwortet mit der eingestellten Zeit ("Time set to: ...").