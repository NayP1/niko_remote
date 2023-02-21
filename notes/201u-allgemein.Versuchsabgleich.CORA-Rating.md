---
id: d6m7rqfokxoi7zf36dxt9wf
title: CORA-Rating
desc: ''
updated: 1676969187303
created: 1676963795876
---
### CORA Rating - CORrelation and Analysis
Die CORA-Methode vereint die folgenden Methoden zu einem Gesamt-Rating-Zahlenwert, um zwei Kurven miteinander zu vergleichen:

1. Korridormethode
2. Kreuzkorrelationsmethode
3. Phasenlage(be)wertung
4. Verlaufsmethode (progression method)
5. Größenwertung (Amplitude)

![](/assets/images/2023-02-21-08-18-19.png)


Rating R &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp &nbsp|		Grade &nbsp &nbsp &nbsp &nbsp &nbsp|		Description 
---------|----------|---------
R > 0.94|		Excellent|	Almost perfect characteristics of the reference signal is captured
0.8 < R ≤ 0.94|		Good|		Reasonably good characteristics of the reference signal is captured, but there are noticeable differences between both signals
0.58 < R ≤ 0.8|		Fair|		Basic characteristics of the reference signal is captured but there are significant differences betweeen the two signals
 R ≤ 0.58|		Poor|		Almost no correlation between the two signals

### ARRK-Path to PPT:
```\\mucfs\project\BMW\EP-620\P58160_Verifikation_Kopfaufprallsimulation\work\50_Reports\Projektdokumentation\ARRK\CORA\230220_CORA_Rating_Kochrezept.pptx```

### Exmaple of animator4 command:
```s[0]:c2d cal isocor([0:3752], [1:1], "auto", 0, 0.014)```