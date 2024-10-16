---
title: smarte Radar-Einheit
date: 2024-10-16
description: >
  Implementierung der Datenauswertung auf der Radar-Einheit
author: Nanu

resources:
  - src: "smarte-Radar-Einheit.jpg"
    title: "Die Auswertung soll später vollständig auf unserer Sensor-Einheit laufen."
    params:
      byline: "Photo: Nanu Frechen / CC-BY-CA"
---

Nachdem wir am Computer einen Algorithmus zur Auswertung der Radar-Daten entwickelt haben muss das Ganze nun auf dem Gerät implementiert werden. Unser Ziel ist dass alle Daten schon in der Box ausgewertet werden und wir nur noch die Anzahl der Autos und deren Geschwindigkeit speichern.

Im Vergleich zur [Auswertung am Computer](/blog/2024/10/15/datenanalyse/) gibt es da einiges was auf dem Gerät anders laufen muss: Am Computer haben wir mit aufgezeichneten Daten gearbeitet. Auf dem Gerät machen wir die Auswertung live. Das bedeutet dass wir an einigen Stellen Werte zwischenspeichern müssen. Zum Beispiel für die Glättung des verrauschten Rohsignals. In der einen Fahrtrichtung müssen wir die Geschwindikgeiten zwischenspeichern bis der Trigger eines vorbeifahrenden Autos kommt. Erst dann können wir die Daten speichern. Bei den Autos der anderen Fahrtrichtung bekommen wir einen Trigger und müssen dann auf die Geschwindigkeitsdaten warten.

{{< imgproc smarte-Radar-Einheit Fill "600x375 webp" >}}
Die Auswertung soll später vollständig auf unserer Sensor-Einheit laufen.
{{< /imgproc >}}


Ausserdem gibt es noch einiges zu optimieren um die Daten effizient auf dem kleinen Rechenkern auszuwerten.

Unsere Entwicklung könnt ihr im [SensorUnit  repository auf github](https://github.com/fablabcb/CitRad-SensorUnit) nachverfolgen.

