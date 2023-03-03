---
id: es0tucvmv5cjlku6l932ngi
title: FMH rausschreiben
desc: ''
updated: 1677833644910
created: 1677831295991
---
Anleitung zum Rausschreiben der positionierten FMHs, um sie in Animator visuell auszuwerten.

### ANSA-Skript für Knoten-Transformation
Die in Generator positionierten FMHs werden mit einer Transformationskarte aus Generator mit dem derzeitigen Template rausgeschrieben

Link zu Template: 

`x:\Xke\intern\PedOS\09_Strategy\FMVSS201\FMVSS201u\Positioning\Positioning_of_FMHs\Generator\FMVSS201u_v05.tpl`

Nach dem Rausschreiben muss die Dateiendung noch angepasst werden: 

".FMVSS201u_v05" --> ".dyn"

Animator kann Parameter nicht mit einlesen, daher ist eine Transformation der Knoten nötigen. Um dies für viele Punkte zu automatisieren wurden ein ANSA-Skript geschrieben, dass beliebig viele Köpfe einlad und sie anschließend wieder rausschreibt:

`x:\Xke\intern\PedOS\09_Strategy\FMVSS201\FMVSS201u\Positioning\Positioning_of_FMHs\Generator\write_out_FMHs.py`

- Das Pythonskript in den Ordner verschieben, wo sich die gerade aus Generator herausgeschriebenen FMHs befunden
- Die FILES-Variable des Pythonskripts anpassen 
- Das Skript im ANSA-Skripteditor ausführen.

Nun sollten sich zusätzliche FMH_mod.dyn-files im Ordner befinden und können in Animator eingeladen werden.
