---
title: Erfolgreicher erster Bauworkshop
date: 2025-01-18
description: >
  Mit Mitgliedern des Fablab Cottbus e.V. haben wir uns am 18. Januar 2025 einen Nachmittag Zeit genommen und vier neue CitRad-Sensoren für das Sammeln von offenen Verkehrsdaten gebaut. Dabei konnten wir unsere Bauanleitung auf Schwächen prüfen und vier neue Sensoren für die datenschutzkonforme Verkehrszählung zum Einsatz bringen.  
author: Bene
resources:
  - src: "featured-bauworkshop.jpg"
    title: "Viel Fingerspitzengefühl beim Löten mussten die Teilnehmer des ersten Bauworkshops mitbringen"
    params:
      byline: "Foto: Benedikt Stahl / CC-BY-CA"
---
Relativ kurzfristig erklärten sich vier Personen aus dem Mitgliederkreis des Fablab Cottbus bereit, uns beim Test der Bauanleitung und der Herstellung neuer CitRad-Sensoren für die Verkehrszählung in Cottbus zu unterstützen. Alle Teilnehmenden hatten unterschiedliche Erfahrungslevel, was uns wertvolles Feedback zur Bauanleitung versprach. Und die Erwartungen wurden voll erfüllt.  

{{< imgproc anleitungscheck Fit "1200x600 webp" >}}
Gewissenhaftes Lesen der Anleitung: Um problemlos zum fertigen Sensor zu kommen, mussten sowohl Anweisungstexte vollständig gelesen als auch Fotos genauer betrachtet werden. 
{{< /imgproc >}}

## Viele Hinweise aus verschiedenen Blickwinkeln

Ohne langes Vorgeplänkel gaben wir als einzigen Hinweis unsere Website bekannt. Den Rest sollten sich alle selbst erarbeiten, ohne von uns Erklärungen zu erhalten. Ganz schnell vielen die ersten Unvollständigkeiten auf, für die man als Autor der Dokumentation schnell den Blick verliert. Viel interessanter war jedoch, wie gut oder schlecht einzelne Anweisungen und Fotos von unterschiedlichen Leuten verstanden wurden. So kamen schnell hilfreiche Hinweise zusammen, die man mit dem Feedback der anderen Teilnehmenden direkt richtig einordnen konnte.

## Knackpunkt Löten
Im Vorfeld am meisten Sorgen bereitete uns die Verbindung des Radarmoduls mit dem Rest der Elektronik. Hier gibt es komplexe Schritte vom richtigen Biegen von Pins bis hin zum Löten auf engstem Raum. Erstaunlicherweise kamen hier sowohl erfahrene Lötspezialisten als auch Leute, die schon etwas aus der Übung waren gut zurecht. Weswegen wir nun zuversichtlich sind, dass das Bauen des CitRad-Sensors für Selbstbauer als auch Workshopteilnehmer in Zukunft kein Frust- sondern ein Erfolgserlebnis sein wird.  

## Fertig für den Einsatz auf der Straße
Nach zwei bis drei Stunden waren alle soweit, dass nur noch die fehlende Software auf das Teensy-Entwicklerboard geflasht werden musste. Da das noch nicht Teil der Anleitung war, übernahmen wir das Flashen und statteten die CitRad-Sensoren mit der neuesten Version unseren Auswertealgorithmus aus. Damit sind die Sensoren jetzt bereit, die Anzahl und Geschwindigkeit der vorbeifahrenden Fahrzeuge in beiden Fahrtrichtungen zu erkennen. Für das Sensor Netzwerk in Cottbus bedeutet es außerdem vier neue CitRad-Module die für offen zugängliche Verkehrsdaten sorgen. Das freut nicht nur uns, sondern auch die teilnehmenden frisch gebackenen Sensorpaten.

<div class="row">
<div class="col-md-6">
{{< imgproc sensor_andres Fit "1200x600 webp" >}}
Andres brachte am meisten Erfahrung mit und nutzte am Ende die Zeit für die Implementierung ein paar im Test befindlicher Zusatzfunktionen. 
{{< /imgproc >}}
</div>
<div class="col-md-6">
{{< imgproc sensor_sarah Fit "1200x600 webp" >}}
Sarah traute sich trotz etwas länger zurückliegender Löterfahrung an den Sensorbau und konnte den Workshop ohne große Mühen mit einem Erfolgserlebnis abschließen. 
{{< /imgproc >}}
</div>
</div>
