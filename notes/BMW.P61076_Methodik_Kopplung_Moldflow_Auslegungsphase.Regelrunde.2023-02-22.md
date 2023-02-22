---
id: uc3f76xi0p9pylwbco9mmko
title: '2023-02-22'
desc: ''
updated: 1677064325940
created: 1677058099254
---
### Date:
**22.02.2023** 10:30-12:00

### Participants:
- Nikolai Patrzek (ARRK)
- Philipp Mäser (ARRK)
- [[BMW.EP-620.Alexander_Rager]] ([[BMW.EP-620]])
- [[BMW.EP-404.Gabriele_Fruhmann]] ([[BMW.EP-404]])
- [[BMW.EP-620.Geoffrey_Tanaka-Wissel]] ([[BMW.EP-620]])
- [[PEG.Sebastian_Mönnich]] ([[PEG]])
- [[PEG.Sven_Theissen]] ([[PEG]])
- [[matfem.person.michael_richter]] ([[MATFEM]])


### Topics:
- Beauftragungssituation und Rahmenverträge (`Geoffrey ist dran`)
- Abschlussdoku

### Details:
#### Simulationsphasen
- Sebastian:  Abschluss soweit fertig. Einzig Simulationsphasen-PPT kommt hinzu.
- Wenn CAD da, alles wird abgebildet. IdR sind aber nicht alle Details (Geo) bekannt. Das bedeutet, dass meist nicht alle Einzelheiten berechnet werden können. Extreme Scherbelastungen/Temperaturen werden in Moldflow abgebildet; Wissen ist nötig, damit Ergebnisse interpretiert werden können
- MeltFlipper: 
  - Designoptimierung des Angusssystems, um eine gleichmäßigere Schmelzführung zu erzeugen
  - Sinnvoll bei vielen Umlenkvorgängen der Schmelze, bei sehr schnell/langsamen Fließgeschwindigkeiten. 
  - Kann Bindenähte verschieben. Muss aber erst ausgelegt werden, nicht trivial. Kann für bereits existierende Werkezeuge verwendet werden.
  - Für 201u-Bauteile kein Standard, könnte aber eine Möglichkeit seit, wenn es ein Problem gibt.
#### Kochrezept (CORA-Analyse)
- Sollen im selben Ordner abgelegt werden
- Zusätzliche Notiz einfügen, dass die Reihenfolge beim Einladen eine Rolle spielt. Empfehlung, dass Versuchskurve als Referenz definiert wird und bei Vergleich von Simulationen eine Simulationskurve als Referenz immer verwendet wird
- Zusätzliches Kochrezept aus 1-2 Folien. (Oder Details alles im Backup)
- Reine Kochrezept intern test, ob verständlich.
- Handbuch-Verlinkung einfügen (Animator intern)
- Evtl. etwas stärker auf MATFEM-3-Biege-Versuch eingehen
- Zweitest Kochrezept wird im nächsten Termin vorgestellt
  - Bauteil, das in die Simulation reingeht, wird nicht geändert
  - Dass die Dienstleister das Mapping skalieren, soll nicht passieren
  - was aus Moldflow rauskommt, in Ansa skalieren und das Mapping auf das nicht geänderte FE-Teil hinzufügen. Prozess direkt in ANSA
#### Allegemeines Kochrezept
- Bilaterale Runde erstellen, mit ARRK, MATFEM und PEG, damit die Datei passend ist.
#### Kantenkontakt
- Michael Pfaffinger testet schon länger neue Solverversionen und jetzt gibt es zusätzliches Problem
- Ist jetzt durch MATFEM sauber dokumentiert und wurde unter Aufsicht von Michael Pfaffinger an DYNAmore übergeben.
- War bei BMW auch schon bekannt und andere Kontaktthemen machen scheinbar auch Probleme; nicht nur Kantenkontakt.
- MATFEM konnte auch mit MAT_24 und neuster Version eine Durchdringung erzeugen. Weiteres Tracking erfolgt
#### Mold Injection Tool
[[matfem.person.michael_richter]] zeigte einen Arbeitsstand.

Symbole für isotrope und anisotrope Materialkarte

![](/assets/images/2023-02-22-11-51-59.png)
![](/assets/images/2023-02-22-11-52-25.png)

Moldflowsimulation, die die Faserorientierung durch Herstellungsprozess berechnet, zeigt früheres Versagen, wie die isotrope Materialkarte

![](/assets/images/2023-02-22-11-56-38.png){max-width: 400px}

Michael: ANSA gibt eine grobe Abschätzung der Faserorierung; auch ohne Viskositätsdaten, Temperaturdaten und mehr des Materials

Vergleich Simulation-Versuch nur für die Standart-Versuchsträger

Gabriele: Versuchsträger mit [[BMW.P61076_Methodik_Kopplung_Moldflow_Auslegungsphase.Erlanger_Traeger]] könnte sinnvoll sein.

Erlanger-Träger: Standartgeometrie, kommt durch die Entwicklung von Organoblechen

Konklusio:
- Vergleich auf Bauteilebene (rein isotrop vs. ausführlich modelliert)
- Ziel Wie stark ändert sich das Versagen und die Energieabsorption
- Vergleich mit Erlanger-Träger scheint sinnvoll, um eine bessere Aussage zu treffen 




### Actions (für ARRK):
- [ ] Zusätzliche Notiz einfügen, dass die Reihenfolge beim Einladen eine Rolle spielt. One-Pager ezeugen und restliche Folien ins Backup schieben
- [ ] 