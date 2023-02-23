---
id: m0mz8fn63bmjpfa5uks0fs6
title: Kalkulation 201u Version 1
desc: ''
updated: 1677158364853
created: 1676973652824
---
### Annahmen
2 Dächer: Hardtop + Softtop (Mindestens ein Modellaufbau, um zu sehen, wie sehr sich das Hardtop vom regulären Huracan unterscheidet)

Im regulären Fahrzeug wird ein Curtain vorhanden sein. Wenn dieser entfällt sollte das doch auch Einfluss auf die 201u-Entwicklung des Hardtop haben (12-Meiler, Defoweg)

--> Annahme, dass zwei Dächer entwickelt werde müssen

Weniger Versuchsabgleiche als gewohnt (Testing nur mit Proto-Phase. Es wird wohl nur 5 Fahrzeuge und 2 BIWs (Schlittenversuche) geben)

Zusätzliche Kosten durch Lizenzen(Simulationen auf eigenem Cluster)

### Zeitplan
- 2023-06: Start der Aktivitäten
- 2023-05: Start P-Frei
- 2024-04: Proto (Testing)
- 2024-11: B-Freigabe
- 2025-10: PVS (Vorserie)
- 2026-06: SOP

### VW-Erfahrung:
- 1.75 Personen (0,75+1BCC) für 2 Fahrzeuge mit je zwei Dächer
- 3 Personen (1+2BCC) für 3 Fahrzeug mit je zwei Dächer

### Kalkulation mit Zeit * Manpower
Dauer der Entwicklung: grob 2,5 Jahre (30 Monate)
- **213.750€**
- 0.375 Personen HC ( ```0.375 * 80 € * 150 h/Monat * 30 Monate = 135.000€``` )
- 0.5 Personen BC ( ```0.5 * 35 € * 150 h/Monat * 30 Monate = 78.750€``` )

### Kalkulation mit VW Lastenheft
- **181.700€ +**
- Modellaufbauten ( ```3 Phasen * 2 Dächer * 9.000 €/Modell = 54.000€``` )
- Reguläre Varianten ( ```110 Varianten * 6 Modellaufbauten * 180 €/Variante = 118.800€``` )
- Komplexe Varianten ( ```24 Varianten * 300 €/Variante = 7.200€``` )
- Absicherungsvarianten ( ```2 Varianten * 850 €/Variante = 1.700€``` )
- (+ Mögliche zusätzliche Umfänge durch Versuchsabgleiche oder Aufbau Ersatzmodell zum Test ohne Fahrzeuge oder BIWs zu schädigen)


![](\assets\images\2023-02-21-11-37-24.png)

### Kalkulation mit BMW WRV
**129.530€**
- 2 x Prüfbereich bestimmen + 2 x Cabrio ( `2 * 2.750€ + 2 * 1.375€ = 8.250€` )
  - ( In BMW VW gibt es gleiche Anzahl Prüfbereich bestimmen wie für Modellaufbau, mach mMn. wenig Sinn --> Ein Modellaufbau weniger geplant als bei VW? Könnte sein.)
- 3 x Modellaufbau + 2 x Cabrio ( `3 * 11.100€ + 2 * 7.400€ = 48.100€` )
- 3 x Systemanalyse und Simulation zu Zielerreichung + 2 x Carbio ( `3 * 8.250€ + 2 * 3.850€ = 32.540€ ` )
- 2 x Robustheitsanalyse + 1 Cabrio ( `2 * 1.920€ + 1 * 2.560€ = 6400€` )
- 2 x Versuchsanalyse + 1 Carbio ( `2 * 2.560€ + 1 * 1.920€ = 7.040€` )
- 1 x Umsetzung Funktionserfüllung + 1 Cabrio ( `17.000€ + 10.200€ = 27.200€` )

`y:\Privat\FMVSS-201u\BMW\004-20200121_Kostenstruktur_FMVSS201u.xlsx`

`Konstenstruktur des WRVs von BMW teilweise unklar. In obiger Kalkulation mit BMW WRV wurden Annahmen über die Anzahl der Pakete selber getroffen!`

### Sehr grobe Rechnung zu Lizenz und Hardwarekosten
- **46.200€**
- Anzahl Varianten: ```700``` 
- Durchschnittliche Anzahl an Simulationen pro Variante: ```10```
- Rechenzeit pro Variante mit 40 CPU: ```2h``` (keine Erfahrungswerte auf dem ARRK Cluster! Bei VW waren es 1h mit 48 CPUs (?) )
- Lizenz- und Hardwarekosten pro Stunden: ```3,30 €/h```
- Keine Lizenzkosten für FMH erwartet. Annahme, dass wir Audi/VW FMH bekommen. Ist auch in Interesse von Lamborghini, damit ihre OEM-Skripte sofort funktionieren. Muss aber im Angebot erwähnt werden
