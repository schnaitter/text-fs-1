(ocr_intro)=

# Einführung
```{admonition} Groblernziel dieses Kapitels
:class: lernziele
Sie können Schritte zur Erstellung eines Forschungskorpus aus Bilddaten  mittels Optical Character Recognition (OCR) aufzählen und die Qualität der Datensammlung anhand eines Samples bewerten.
```

## Zu diesem Kapitel
Nach dem vorherigen [Kapitel](corpus-collection_summary) haben wir also ein Korpus als Sammlung gescannter Bilder. Ein Korpus in dieser Form ist jedoch noch **nicht maschinenlesbar** und kann nicht direkt verarbeitet werden. In diesem Kapitel lernen wir, wie man mit OCR **Bilder in Text umwandelt**.

```{figure} ../book_images/flow-chart_ocr.jpeg
---
height:
name: Flussdiagramm der Fallstudie
---
Flussdiagramm der Fallstudie. Wir befinden uns im dritten Arbeitspaket.
```
Zunächst werden wir lernen, [was OCR ist](ocr), warum wir es brauchen und wie es funktioniert. Außerdem werden wir einen Überblick über einige OCR-Tools geben.

Anschließend werden wir [OCR in Python mit PyTesseract](https://dh-network.github.io/quadriga/data-input/FS_1_MVP_OCR) durchführen, einem kostenlosen und quelloffenen OCR-Tool.

Schließlich werden wir die Metriken kennenlernen, die zur Messung der [OCR-Qualität](ocr-quality) verwendet werden, und [Qualitätsmessungen](https://dh-network.github.io/quadriga/data-input/FS_1_MVP_OCR_Quality) durchführen.
