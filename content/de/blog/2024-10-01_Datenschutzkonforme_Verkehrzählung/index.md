---
title: Datenschutzkonforme Verkehrszählung
date: 2024-10-01
description: >
  Kameragestützte Projekte zur Auswertung von Verkehrsdaten existieren als kommerzielle und Open Source Projekte. Wir haben uns bewusst dagegen entschieden, auf diesen Projekte aufzubauen, da sie diverse Probleme mit dem Datenschutz mit sich bringen. Wir haben uns bewusst dafür entschieden, Radar als Grundtechnologie zu verwenden. Den Radar erlaubt uns, Verkehrsdaten zu sammeln, ohne dabei Persönlichkeitsrechte zu verletzen. 
author: Bene
weight: 20
resources:
  - src: "featured-anoncars.jpg"
    title: "Geblurte Autos auf Kreuzung"
    params:
      byline: "Foto: Benedikt Stahl / CC-BY-CA"
---
Als uns klar war, dass wir ein offener Verkehrsdaten sammel und zur Analyse bereitstellen woollen, landeten wir schnell bei der Frage nach dem wie. Existierende Projekte zur automatisierten Auswertung von Kamerabildern waren verlockend, da sie uns viel Grundlagenentwicklung erspart hätten. Datenschutzkonforme Verkehrszählung wäre damit allerdings nicht möglich. Denn durch das Aufzeichnen von Personen, Kennzeichen etc. würden wir uns - auch wenn wir diese Daten direkt nach der Auswertung gelöscht hätten - in einer rechtlichen Grauzone bewegen. Radar hat all diese Datenschutzprobleme nicht, bringt aber zusätzliche Herausforderungen bei der Auswertung.   

{{< imgproc anoncars Fill "1200x600 webp" >}}
Das Radar erkennt nur einzelne Objekte, ohne Details zu erfassen. So als könnte eine Kamera nur unscharfe Verkehrsteilnehmer aufzeichnen.
{{< /imgproc >}}

## Anonymität der Daten

Radartechnologie funktioniert, indem sie elektromagnetische Wellen aussendet, die von Fahrzeugen reflektiert werden. Durch die Analyse der reflektierten Wellen kann das System Informationen über den Verkehrsfluss sammeln, ohne personenbezogene Daten zu erfassen. Dadurch wird die Anonymität der Verkehrsteilnehmer gewährleistet. Im Gegensatz dazu können bildbasierte Systeme potenziell sensible Informationen über die Identität von Fahrern und Passagieren erfassen, was bei der Radartechnologie nicht der Fall ist.

## Rechtskonformität und Eigenanspruch 

Da wir grundsätzlich der Meinung sind, dass persönliche Daten, wo nicht unbedingt notwendig, aus Datensätzen herausgehalten werden sollen, stellte Radar die für uns Ideale Lösung dar. Angenehmer Nebeneffekt war natürlich, dass wir uns so nicht näher mit der Einhaltung der DSGVO beschäftigen mussten. Denn auch wenn die Analyse der Bilddaten nur auf dem Mikrocontroller stattgefunden hätte und sie kein Mensch zu Gesicht bekommen hätte, wären zahlreiche Probleme offen geblieben. Wie stellt man zum Beispiel sicher, dass Dritte sich keinen Zugriff zu den Geräten verschaffen und an noch nicht gelöschte Rohdaten herankommen? Kriegen wir Probleme bei der Akzeptanz des Systems, wenn man das Gefühl hat, man wird auf Kamera aufgezeichnet, nur weil man eine Straße regelkonform entlangfährt. All diese Abwägungen konnten wir mit der Verwendung von Radar guten Gewissens beiseitelegen. 

## Technische Anforderungen und Vorteile

Was die Radartechnologie an sich betrifft, bringt sich einige Vorteile aber auch viele Herausforderungen mit sich. Kamerabilder sind für Menschen leicht zu begreifen. Die Kontrolle der Auswertemechanismen während der Entwicklung kann dadurch viel leichter und schneller erfolgen. Radar dagegen liefert uns für die Auswertung ein Spektrum, das für ungeübte Betrachter nur sehr schwer zu entziffern ist. Der initiale Aufwand und die Interpretation der Ergebnisse wird also tendenziell mehr Zeit in Anspruch nehmen. Auf lange Sicht arbeitet Radar allerdings zuverlässiger als die Bildauswertung. Radar kümmert es nicht, welche Lichtverhältnisse herrschen. Die reflektierten Wellen sehen bei stockfinsterer Nacht genauso aus wie am helligen Tag. Auch unterschiedliche Wetterbedingungen sind für Radar prinzipiell kein Problem. Nebel, Regen und Schnee sollten, so zumindest die Theorie, beherrschbar sein, sobald der Auswertungsalgorithmus einmal ordentlich darauf eingestellt ist. Wie erfolgreich uns das gelingt, werden wir in den kommenden Blogbeiträgen beschreiben.

## Fazit

Mit CitRad werden Verkehrsdaten datenschutzkonform erhoben und zur weiteren Analyse bereitgestellt. Niemand, der an einem CitRad-Sensor vorbeifährt, muss befürchten, dass irgendwo Datensätze entstehen, die mit ihm/ihr in Verbindung gebracht werden. Vor Punkten in Flensburg muss man sich erst recht nicht fürchten. Auch wenn wir Geschwindigkeitsverstöße feststellen, können wir diese lediglich statistisch erfassen und keine Rückschlüsse auf das genaue Auto oder den/die Fahrer:in ziehen. Datenmissbrauch ist somit ebenfalls ausgeschlossen.
Was die Genauigkeit der Auswertung angeht, wird es sicherlich noch einige Zeit dauern, bis wir alle Eventualitäten in der Auswertung mit abfangen werden. Bis dahin liefert der CitRad-Sensor aber in jedem Fall schonmal gute Tendenzen und quantitative Übersichten. 