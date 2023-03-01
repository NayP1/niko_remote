---
id: duqjxixlol75le3floh1bdx
title: '2023-03-01'
desc: ''
updated: 1677668148503
created: 1677664264173
---
Philipp (krank) und Sven nicht anwesend

## To-Do
Kochrezept prüfen und finalisieren und nächste Woche vorstellen.

## Themen
### Abschlusspräsentation
Übersichtsfolie ergänzen mit Links zu den Kochrezepte. Soll möglichst niederschwellig sein.

Kochrezept für Moldflow in ANSA
- Intern prüfen
- In kommender Runde vorstellen
- In PPT verlinken

Ende 2023 weiterer Abschlussbericht

Langfristig soll alles in Confluence

### Kantenkontakt
Elementgröße ist das Problem. Eigestellt für Kontakt sind 2-4mm, wir haben Elementgrößen von 0.8mm - 1.0mm
Drillstiffness kann noch ein weiteres Problem sein, muss aber noch weiter untersucht werden
- Netzverfeinerung um jeden Preis ist gefährlich.
- Masse des Elements (und dadurch auch die Dichte des Materials) wichtig für die Kontaktsteifigkeit
  - Option 1: Netz nicht zu fein machen
  - Option 2: Eigene Kontaktkarte für sehr feine Elemente
- Empfehlung für zu empfehlenden Materialgrößen im Anschluss mit Herrn Stahlschmidt
  - Eigener Kontakt für kleine Elemente benötigt eigenes Include. Für Detailuntersuchung könnte ein solches Include mit Kontaktmodifikationen erstellt werden.
- Kontaktproblem gilt auch für das normale MAT_24 von BMW
- MAT48 zeigte früher das Problem, da die Verfestigung des Materials weicher war, wie bei MAT24
  - Tendenziell ist MAT48 nicht weniger robust wie MAT24

Kontaktsteifigkeit nimmt Elementmasse in die Berechnung, daher ist bei kleinen Elementen, gerade die eine geringe Dichte haben, die Kontaktsteifigkeit zu gering

Automatische Einstellung der Kontakte, nur für Materialien möglich, die sich in der MATDB befinden
- Drillstiffness nicht immer richtig eingestellt
- Kontaktsteifigkeit nicht immer richtig
- Sobald Material von extern kommt, muss alles händisch eingestellt werden. Daher extrem fehleranfällig.
- --> Unklar ob in dem Modell, was immer gerechnet wurde, die Kontakte richtig definiert worden sind
- Gernot: Elementsteifigkeiten sollen sich nicht in der Regel nicht verändern
- Modifierung der künstilchen Elementsteifigkeit gerade bei BMW sehr groß, durch Solverwechsel von ABAQUS zu DYNA. Materialien haben sich beim Solverwechsel anders verhalten und Modifikation der Kontakte war einfachste Lösung, ohne die komplette MATDB zu erzeugen
- Automatische Kontaktsteifigkeitmodifikation aufgrund von kleiner Elementgröße generell möglich, aber wird bei Dynamore wohl eher nicht entwickelt
- SQMS-Check muss angepasst werden für MATFEM-Materialien
  - Für jedes Include, das MATFEM verwendet, muss eine Flag gesetz werden
  - Idee für eigene MID-Range für MATFEM-Materialien

### ANSYS, LSCT und Dynamore
- ANSYS kaufte LSCT
- LSCT ist Entwickler von LS DYNA
- Dynamore ist Vertriebspartner von Dyna
- Überwiegende Entwicklung in USA. Kontaktentwicklung daher auch wohl in USA
- Dynamore hat auch Entwickler, aber deutlich weniger wie LSCT

### Status Mapping-Schnittstelle in ANSA 
ANSA macht Probleme, vermutlich weil Modelle extrem groß ist

Vorschlag, dass Thema für kleinere Modelle vorgenommen?

Thema eher etwas für Moldflow/Autodesk, da sie mehr Input (Temparatur, Fließeigenschaften, ...) haben

Artefakte kommen daher, dass Schmelzeläufe zusammenlaufen. Nur werden auch sehr kleine, lokale Bindenähte berechnet, die zwar stattfinden, aber keinen Einfluss auf die Materialeigenschaften haben

Einstellung, dass es eine Option gibt, um nur relevante Bindenähte abzubilden
- Sofwaretechnisch wahrscheinlich möglich
- Könnte vielleicht sogar bei PEG stattfinden


