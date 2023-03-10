---
id: aoa8cbnuapqlqtc3jkmo99k
title: AP-Punkte
desc: ''
updated: 1678444940977
created: 1678437857420
---
## AP1
AP1 ist DER Punkt, mit dem alles startet.

Beim Prüfen der Linie muss darauf geachtet werden, dass die stetig sind und kein Sprünge vorweise. 
- Am einfachsten ist es in ANSA Hilfsvernetzung dort zu generieren, wo Kurve über Spalten laufen. (Mesh --> Shell Mess --> Fill --> Manual)

### Plane 1
Er wird durch den hintersten Punkt der Windschutzscheibe definiert, hierbei zählt aber auch die Dichtung dazu.

Beispiel BMW:

![](/assets/images/2023-03-10-09-46-25.png){width: 600px, border: 2px solid gray}

Beispiel carhs:

![](/assets/images/2023-03-10-10-05-16.png){width: 600px, border: 2px solid gray}

### L1 und PT1
Es wird an der Außenfläche des Fahrzeugs eine Linie erstellt, die bis zum äußersten Punkte des Rahmens (ohne Tür, mit Anbauteilen) geht.

Es muss also darauf geachtet werden, dass kein Teil ganz außen fehlt. (Keder muss auch berücksichtigt werden)

Bei Zierleisten am Dach muss man genau hinschauen, siehe BMW-Hinweis (links richtig, rechts falsch)

![](/assets/images/2023-03-10-10-08-58.png){width: 900px, border: 2px solid gray}

125mm vom äußersten Punkte entlang der Linie L1 und man erhält PT1

### PT2
Von PT1 ausgehend, wird wieder eine senkrechte Ebene Plane2 erstellt. Auf der Schnittlinie zum Dach geht man 50mm nach hinten und man erhält PT2.

Sollte in dem Bereich eine Zierleiste sein, muss diese wieder "geschlossen" werden, wie es auch bereits bei L1 gemacht wurde

Von PT2 aus wir ein Normalenvektor erstellt und dort, wo dieser Vektor das Interior berührt befindet sich AP1.

Es ist sehr wichtig, dass von PT2 aus ein sinnvoller Normalenvektor erstellt werden kann.

### Horizontale Schusswinkel
Standardmäßig liegt der legale Bereich für den horizontalen Winkel für die ASV bei 195° - 255°.

Die Positionen der Köpfe (durch SRPs berechnet) und deren kürzeste Abstände zu den Säulenverkleidungen definieren aber die tatsächlichen Grenzwinkel.
