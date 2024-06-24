(introduction_intro)=
# Einführung in die Fallstudie: Fragestellung und Operationalisierung
## 1. Heranführung an die Fragestellung
Dass Pandemien ihre je eigenen Verlaufsprofile entwickeln, konnte Zeitgenoss:innen vor wenigen Jahren am Verlauf der COVID19-Pandemie miterleben. Schnell wurde die Rede von den "Wellen" der Corona-Pandemie sprichwörtlich. Auch während der Spanischen Grippe wurde bereits von "Wellen" bzw. von "Waves" gesprochen und diese spezifische Verlaufsform graphisch dokumentiert (siehe Fig. 1). 

```{figure} ../book_images/Plague-versus-Spanish-Flu.jpg
---
height: 500px
name: Vergleichende Grafik zum Verlauf der Pest (1665) und der Spanischen Grippe (1918/19) in London
---
Vergleichende Grafik zum Verlauf der Pest (1665) und der Spanischen Grippe (1918/19) in London. Quelle: {cite:p}`staveley-wadham_british_2021`
```

Aus Perspektive einer medienwissenschaftlich informierten historischen Epidemiologie überlagern sich dabei unterschiedliche Wellen: Während ‘Fallzahlen‘ (z.B. die Anzahl der Infektionen oder die Anzahl der Todesfälle), wie sie in Fig. 1 dargestellt werden, ein in erster Linie medizinisch zu erhebendes Maß sind, sind die unterschiedliche Intensität und Extensität der öffentlichen Wahrnehmung des pandemischen Geschehens ein Untersuchungsgegenstand der (historischen) Medienwissenschaft. Auch hier ist davon auszugehen, dass sich charakteristische "Mediengezeiten" oder eben: "Medienwellen" zeigen: Mal dominiert die Pandemie den öffentlichen Diskurs, mal tritt sie in der öffentlichen Wahrnehmung zurück. 

## 2. Forschungsfrage und Operationalisierung
Diese Fallstudie führt durch eine Digital Humanities-Forschungsprojekt, das aus medienhistorischer Perspektive den Verlauf der "Medienwellen" während der Spanischen Grippe 1918/19 – bekannt auch als "the Mother of All Pandemics" {cite:p}`taubenberger_2006` – in Berlin und Brandenburg untersucht hat. Das Forschungsprojekt wurde von der folgenden Forschungsfrage geleitet: 

`````{admonition} Forschungsfrage
:class: tip
Lassen sich für die Spanische Grippe 1918/1919 mit Fokus auf den Berliner Raum Muster in der öffentlichen Aufmerksamkeit ausmachen, die eine wellenartige Verlaufsform aufweisen? 
`````

Als eine Orientierungsgröße für ein wellenartiges Muster nehmen wir – in Form einer Hypothese – das Verlaufsprofil der medizinischen Welle der Spanischen Grippe, wie es bei {cite:p}`taubenberger_2006` für Großbritannien berechnet und visualisiert wurde (Fig. 2).

```{figure} ../book_images/Drei-Wellen-1918-19-UK.png
---
height: 300px
name: Drei Wellen der Spanischen Grippe im Vereinigten Königreich.
---
Drei Wellen der Spanischen Grippe im Vereinigten Königreich. Quelle: {cite:p}`taubenberger_2006`
```

Die Forschungsfrage zielt darauf, öffentliche Aufmerksamkeit und deren Veränderung über die Zeit zu messen. Um eine solche Messung möglich zu machen, muss zunächst eine Operationalisierung der Forschungsfrage erfolgen. "Operationalisierung bezeichnet den Prozess, ein Erkennungs- oder Messverfahren für ein theoretisches Konzept zu entwickeln." {cite:p}`krautter_operationalisierung_2023`.

Für die Operationalisierung unserer Forschungsfrage müssen insbesondere zwei Fragen adressiert werden:

- Was ist öffentlichen Aufmerksamkeit im Berliner Raum? 
- Wie kann diese gemessen werden? 

Entlang dieser beiden Fragen kommen wir zur folgenden Operationalisierung:

`````{admonition} Operationalisierung
:class: tip
Als öffentliche Aufmerksamkeit im Berliner Raum sollen in unserer Fallstudie die Texte in Berliner Tageszeitungen gelten. Wir messen diese öffentliche Aufmerksamkeit, indem wir die Häufigkeit von Wörtern ermitteln. Eine besonders hohe öffentliche Aufmerksamkeit für die spanische Grippe in einem bestimmten Zeitraum läge demnach dann vor, wenn wir in den Zeitungen für diesen Zeitraum besonders viele Wörter nachweisen können, die direkt oder indirekt auf die spanische Grippe verweisen. 
`````

Diese Operationalisierung ist, wie jede Operationalisierung in den Digital Humanities, diskutabel. Sie folgt dabei einem quantitativen Methodenparadigma. Und sie wählt mit der Worthäufigkeit einen einfachen Indikator für das zu messende Phänomen. Die Operationalisierung wird zudem weitere Einschränkungen erfahren müssen, etwa was das Korpus der Analysen betrifft, das mit der Formulierung "Texte in Berliner Tageszeitungen" derzeit sowohl zu unscharf angegeben ist als auch viel zu groß wäre. 

Die Reflektion der Grenzen und Beschränkungen, die mit der eigenen Operationalisierung einhergehen, ist essentieller Bestandteil von Digital Humanities-Projekten. Wir werden in der abschließenden [Reflexion](reflection_reflection) darauf zurückkommen. 

## 3. Struktur der Fallstudie
Die Fallstudie vollzieht 5 Schritte: 

- Im **1. Schritt** bauen wir ein Korpus aus Textobjekten für die Analyse auf, das zunächst aus PDF-Dateien besteht (siehe Kapitel ["Korpusaufbau"](corpus-collection_intro))
- Im **2. Schritt** machen wir die Textobjekte im Korpus, die zunächst nur als Bilddateien vorliegen, mittels Optical Character Recognition (OCR) maschinenlesbar (siehe Kapitel ["OCR — Vom Bild zum Text"](ocr_intro))
- Im **3. Schritt** evaluieren wir die OCR-Ergebnisse und testen Optionen zur Nachkorrektur (siehe Kapitel ["Nachkorrektur der OCR-Ergebnisse"](post-correcting_intro)).
- Im **4. Schritt** reichern wir mithilfe von Verfahren des Natural Language Processing (NLP) die Textobjekte im Korpus mit linguistischen Informationen an. (siehe Kapitel ["Korpusverarbeitung – Von Strings zu Token"](corpus-processing_intro)).
- Im **5. Schritt** führen wir die quantitativen Analysen auf dem Korpus durch udn visualisieren die Ergebnisse (siehe Kapitel ["Korpusanalyse"](corpus-analysis_intro)).

Die Fallstudie schließt mit einer Reflexion und einem Ausblick (siehe Kapitel ["Reflexion und Resümee"](reflection_reflection)) 


## 4. Bibliographie
```{bibliography}
```

