---
id: ly8xkcr5grgt7i2un4najaf
title: Auswertung Tiefziehen MATFEM
desc: ''
updated: 1677090902974
created: 1677090359929
---
Im Rahmen für eine [[Tiefziehuntersuchung|matfem.Tiefziehsimulation_P64076]] mit der Firma MATFEM wurden wir gebeten, eine Auswertung mit LS-PrePost durchzuführen.

Das command-file wurde uns von [[matfem.person.michael_richter]] zur Verfügung gestellt und wird hier kurz erklärt

`openc d3plot "file"` (Öffnen einer Datei)

`top / bot` (Standard View Top / Bottom)

`ac` (View zentrieren)

`selectpart on` (PID anzeigen)

`range userdef x y` (Grenzen der Funktion bestimmen. Zum Beispiel "0" und "1")

`state` (Definieren des States. Mit +/- könenn auch States nach vorne oder hinten verschoben werden)

`print png "file"` (Rausschreiben des Views als .png-Datei)

---

``` sh
openc d3plot "\\mucfs\project\BMW\EP-620\P58160_Verifikation_Kopfaufprallsimulation\work\00_Temp\Temp_Nikolai\MATFEM_Tiefziehsimulation\005\res\z_G60_9623497_G90A_TAHh_210624_VBBG_PTT_kor_UL1_1_3_AFO15_DRAW_005.d3plot"
featuretree show 0
ttb 0
top
ac
state 15;
zoomhere 0.008465 -0.054627 0.085;
pan -210.731735 647.792725;
selectpart on S700/0
fringe 85
top
ac
range userdef 0 1;
print png "mid_history_variable_5_state_15.png" nogamma enlisted "OGL1x1"
state 14;
print png "mid_history_variable_5_state_14.png" nogamma enlisted "OGL1x1"
state 13;
print png "mid_history_variable_5_state_13.png" nogamma enlisted "OGL1x1"
state 12;
print png "mid_history_variable_5_state_12.png" nogamma enlisted "OGL1x1"
state 11;
print png "mid_history_variable_5_state_11.png" nogamma enlisted "OGL1x1"
fringe 81
pfringe
state 15;
range userdef 0 0.5;
print png "mid_history_variable_1_state_15.png" nogamma enlisted "OGL1x1"
state 14;
print png "mid_history_variable_1_state_14.png" nogamma enlisted "OGL1x1"
selectpart on S600/0 S601/0
fringe 81
pfringe
state 15;
print png "out_top_history_variable_1_state_15.png" nogamma enlisted "OGL1x1"
state 14;
print png "out_top_history_variable_1_state_14.png" nogamma enlisted "OGL1x1"
bottom
ac
state 15;
print png "out_bot_history_variable_1_state_15.png" nogamma enlisted "OGL1x1"
state 14;
print png "out_bot_history_variable_1_state_14.png" nogamma enlisted "OGL1x1"
fringe 9
pfringe
top
ac
range userdef 100 350;
state 15;
print png "out_top_von_Mises_state_15.png" nogamma enlisted "OGL1x1"
state 14;
print png "out_top_von_Mises_state_14.png" nogamma enlisted "OGL1x1"
bottom
ac
state 15;
print png "out_bot_von_Mises_state_15.png" nogamma enlisted "OGL1x1"
state 14;
print png "out_bot_von_Mises_state_14.png" nogamma enlisted "OGL1x1"
```