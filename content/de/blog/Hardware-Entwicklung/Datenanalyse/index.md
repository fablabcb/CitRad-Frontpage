---
title: Datenanalyse
date: 2024-10-15
description: >
  Wie zählt man Autos mit einem Radarsensor?
author: Nanu
resources:
  - src: "data_analysis.png"
    title: "Datenanalyse am Computer. Der Algorithmus zählt Autos und misst Geschwindigkeiten."
    params:
      byline: "Screenshot: Nanu Frechen / CC-BY-CA"
---

Nach all unseren Experimenten mit Verstärkerschaltungen und rauscharmer Stromversorgung scheint unser Sensor jetzt gut zu funktionieren. Zumindest kann man in den Spektralbildern der Radardaten sehr deutlich verschiedene Fahrzeuge sehen und erkennen wie schnell sie fahren. Aber wie lässt sich das Ganze mit einem Algorithmus auswerten? Schließlich wollen wir zum Schluss nur noch Fahrzeuge zählen und die Geschwindigkeit von jedem Fahrzeug abspeichern.

{{< imgproc data_analysis Fill "1200x600 webp" >}}
Datenanalyse am Computer. Der Algorithmus zählt Autos und misst Geschwindigkeiten.
{{< /imgproc >}}

Das Auge kann leicht das eigentliche Signal vom Rauschen unterscheiden. In der Datenauswertung braucht man dafür einiges an Glättung und gut gewählter Grenzwerte. Ausserdem verändert sich das Rauschen auch mit der Zeit. Wenn der Akku sich entlädt. Auch dafür mussten wir eine Lösung finden. 

Die Signalanalyse basiert darauf, dass bestimmte Frequenzen aus dem Spektrum herausstechen. Das kann man als Linien im Zeitverlauf sehen. Jede Linie ist ein sich bewegendes Objekt. Ein fahrendes Auto zum Beispiel. Aus der Frequenz kann man dann die Geschwindigkeit berechnen. 

Mit einem besonderen Trick erkennen wir wann ein Auto vorbei fährt: Im Vorbeifahren ändert sich der Winkel zum Rarsensor. Dadurch knickt das Signal nach unten ab (Richtung 0km/h). Diesen Knick erkennen wir und wissen dass gerade ein Auto am Sensor vorbei gefahren ist. Ob dieser Knick links rum oder rechtsrum passiert sagt uns in welche Richtung das Auto gefahren ist. Nun müssen wir nur noch vor oder nach diesem Trigger die detektierte Geschwindigkeit ermitteln und abspeichern.

Was sich einfach anhört ist das Ergebnis einer Menge Tüftelei. Und natürlich haben wir das Ganze erstmal am Computer mit aufgezeichneten Daten entwickelt. Das muss nun auf das Gerät selbst programmiert und getestet werden. Erst dann sind wir so weit dass wir das Gerät Interessierten für eigene Messungen in die Hand geben können. Das wird aber bald soweit sein!

Wer an den technischen Details interessiert ist kann sich das Ganze in unserem <a href=https://github.com/fablabcb/CitRad-SensorUnit/blob/main/Software/data%20processing%20method/read_and_display_raw_spectrum.Rmd target="_blank">Repository auf github</a> anschauen.