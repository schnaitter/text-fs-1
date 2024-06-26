# Korpusanalyse: Einführung in die Methode 

## 1. Forschungsfrage und Operationalisierung
Wir gehen von folgender Forschungsfrage aus: 
`````{admonition} Forschungsfrage
:class: tip
Lassen sich für die Spanische Grippe 1918/1919 mit Fokus auf den Berliner Raum Muster in der öffentlichen Aufmerksamkeit ausmachen, die eine wellenartige Verlaufsform aufweisen? 
`````
Um diese mit quantitativen Methoden zu bearbeiten, wurde die Forschungsfrage zunächstwie folgt **operationalisiert**: 
1. Die **öffentliche Aufmerksamkeit im Berliner Raum** wird durch ein Korpus von zwei Berliner Zeitungen gefasst.
2. Die **Spanische Grippe** wird durch ein manuelle erstelltes semantisches Feld, das sich um das Wort "Grippe" kreist, untersucht. 
3. Der **Verlauf** der öffentliche Aufmerksamkeit wird über die sich entwickelte Häufigkeit des Wortfelds untersucht. Eine erhöhte Häufigkeit deutet auf eine erhöhte Aufmerksamkeit hin und vice versa. 


## 2. Erstellen eines semantische Felds

## 2. Häufigkeit als Analysemethode 

### 2.1 Warum die Häufigkeit analysieren?
Die Analyse von Worthäufigkeiten ist sowohl in der Korouslinugistik als auch in den Digital Humanities [p. 73] weit verbreitet. Für die Analyse von Inhaltswörtern (Nomen, Verben, Adjektive, Adverben) wird angenommen, dass ein hohes Vorkommen mit der Wichtigkeit der Wörter den Text in Frage korreliert. Besonders bei einer vergleichenden Analyse (etwa von zwei Zeitungen oder eine Thema über Zeit) ist die Häufigkeitsnanalyse sinnvoll, da der Vergleich so quantisierbar wird. 

### 2.2 Häufigkeit von Grippe
Um die Wichtigkeit eines Themenfelds wie der Spanischen Grippe zu untersuchen, bietet es sich an, nicht nur das Vorkommen eines einzelnen Wortes wie "Grippe" zu untersuchen, sondern andere, mit Grippe im Zusammenhang stehende Wörter zu sammeln, im Sinne eines semantischen Felds. Die Wörter werden in der Grundform angegeben, sodass sie mit den Lemmata im Text verglichen werden können.
Für jedes Wort wird dann die Häufigkeit errechnet, diese nennt sich **absolute Häufigkeit**. Die absoluten Häufigkeiten werden addiert, sodass sich pro Text eine Zahl ergibt, die die Summe aller Häufigkeiten der Grippenbezogenen Wörter angibt.

`````{admonition} Beispiel
:class: tip
1. **Text**: Die Grippe wütet weiter. Zunahme der schweren Fälle in Berlin. Die Zahl der Grippefälle ist in den letzten Tagen auch in Groß-Berlin noch erheblich gestiegen. Die Warenhäuser und sonstigen großen Geschäfte, die Kriegs- und die privaten Betriebe klagen, daß übermäßig viele Angestellte sich haben krank melden müssen und auch bei der Post und bei der Straßenbahn ist der Prozentsatz der Grippekranken deutlich gestiegen. 
2. **Lemmatisierter Text**: der Grippe wüten weiter -- Zunahme der schwer Fall in Berlin -- der Zahl der Grippefall sein in der letzter Tag auch in Groß-Berlin noch erheblich steigen -- der Warenhaus und sonstig groß Geschäft -- der Krieg und der privat Betrieb klagen -- daß übermäßig vieler angestellter sich haben krank melden müssen und auch bei der Post und bei der Straßenbahn sein der Prozentsatz der Grippekranke deutlich steigen --
3. **Semantisches Feld** "Grippe": Grippe, Grippefall, Grippekranke, krank
4. **Häufigkeitsanalyse**: 

```{table}
:name: Häufigkeitsanalyse
| Wort  | Häufigkeit| 
|--------|-------|
| Grippe    | 1   |
| Grippefall | 1 |
| Grippekranke  | 1 |
| krank | 1 |
```
5. **Summierte Häufigkeit**: 4

`````

### 2.3 Vergleichbarkeit von Häufigkeiten
Für die Vergleichbarkeit von Worthäufigkeiten in Texten ist wichtig, dass die Texte auch ansonsten vergleichbar sind. Stammen die Texte z. B. aus unterschiedlichen Zeiträumen müssten ggf. zeitspezifische semantische Felder erstellt werden, um für den Sprachwandel Rechnung zu tragen. Auch sollten die Texte eine ähnliche Länge haben, sodass eine erhöhte Häufigkeit tatsächlich auf eine erhöhte Wichtigkeit zurückgeführt werden kann.
Wenn Texte verschieden lang sind, sollten die Häufigkeiten **normalisiert** werden, das heißt sie werden in Bezug zur Textlänge gesetzt. Dafür wird die absolute Häufigkeit durch die Textlänge dividiert, daraus ergibt sich die **relative Frequenz**. Die relative Frequenz des semantischen Felds "Grippe" kann als Anteil der Grippewörter am Gesamttext gesehen werden. 

`````{admonition} Beispiel
:class: tip
Der Beispieltext besteht aus insgesamt 69 Wörter, davon sind 4 Wörter in dem semantischen Feld "Grippe" vorhanden. Daraus ergibt sich folgende Rechnung:

$ f = {4 \over 69} = {0.05797101449} $$.

Das heißt: Jedes zwangstigste Wort im Text steht im Zusammenhang mit der Spanischen Grippe. 
`````

### 2.4 Analyse des gesamten Korpus 
Um den Verlauf der Aufmerksamkeit nachzuvollziehen, wird für jeden Text im Korpus die relative Frequenz des semantischen Felds "Grippe" berechnet und in einer Tabelle gespeichert. Die Frequenzen werden dann über die Zeit verglichen. Um Trends zu erkennen  

`````{admonition} Beispiel
:class: tip
```{table}
:name: Häufigkeitsanalyse
| Zeitung  | Relative Häufigkeit| Tag | Monat | Jahr | 
|--------|-------|--------------|----|-------|---------|
| Grippe    | 1   | || |
| Grippefall | 1 | || |
| Grippekranke  | 1 | || |
| krank | 1 | || |
```
`````

Um Muster über die Zeit zu erkennen, ist es sinnvoll die erhobenen Häufigkeiten in größere Zeitabschnitte zu unterteilen, wie z.B. Wochen oder Monate. Dafür werden sowohl die absoluten Häufigkeiten als auch die Textlängen in dem ausgewählten Zeitraum addiert, sodass auf dieser Basis die relative Häufigkeit für den Zeitraum berechnet werden kann.


`````{admonition} Durchschnitt von relativen Häufigkeiten
:class: warning
Eine zweite Möglichkeit, die Häufigkeiten über eine Zeitraum zusammenzufassen, bestünde darin, den Durchschnitt der Häufigkeiten zu nehmen. Diese Methode ist davon von schwankenden Textlängen an verschiedenen Tagen abhängig. Eine Folge davon wäre, dass Tage mit kurzen Texten und einer hohen Anzahl an Grippewörtern würden Durchschnitt stark in die Höhe ziehen, obwohl die absolute Anzahl an Wörtern geringer ist als an Tagen, für die längere Texte vorliegen. 

```{table}
:name: Beispiel: Methoden des Zusammenfügens

| Tag  | Absolute Häufigkeit| Textlänge | 
|------|--------------------|-----------|
| 1    | 20    | 500 |
| 2    | 5     | 100 |
| 3    | 15    | 600  | 
```
1. Alle Häufigkeiten addieren und durch die Summe der Textlängen teilen: $ {{20 + 5 + 15} \over {500 + 100 + 600}} = {{40} \over {1200}} = {0.033}$
2. Die relative Häufigkeiten addieren und durch die Anzahl an Tagen teilen: $ {{{20 \over 500} + {5 \over 100} + {15 \over 600}} \over 3} = {{0.04 + 0.05 + 0.025} \over 3} = 0.038$

Mit der zweiten Methode ist die relative Häufigkeit um 0.005 höher.
`````

## 3. Visuelle Darstellung 
Im diesen Schritt werden die extrahierten absoluten oder relativen Häufigkeiten visualisert.

* x-Achse als Zeit 
* Liniendiagramm 
* Andere Möglichkeiten

### 3.2 Akkumulierung von Häufigkeiten über Zeit

## 4. Keyword in Context (KWIC) 
* Darstellungsform von Suchergebenissen 
* Zentrierung des Suchbegriffs (und Hervorhebung) 
* Zweck: schnelles Scannen des Kontext für weiterführende Analysen wie: 



## 5. Zusammenfassung und nächste Schritte 

