# Einführung - OCR als Methode, um Text maschinenlesbar zu machen

**Optical Character Recognition (OCR)** ist eine Technologie, die es ermöglicht, gedruckten oder handgeschriebenen Text in Dokumenten oder Bildern in maschinenlesbaren Text umzuwandeln. OCR-Software analysiert das Layout des Dokuments, erkennt die Formen der Buchstaben und Zahlen und wandelt diese in digitale Texte um, die weiterverarbeitet werden können.

### Warum benutzen wir OCR?

1. **Digitalisierung von Dokumenten**: OCR ermöglicht die Umwandlung von physischen Dokumenten in digitale Formate, wodurch Speicherplatz gespart und der Zugriff auf Informationen erleichtert wird.

2. **Suchbarkeit**: Texte in Bildern oder gescannten Dokumenten können nach der OCR-Verarbeitung durchsucht werden. Dies erleichtert das Auffinden von Informationen in großen Dokumentensammlungen.

3. **Bearbeitbarkeit**: Mit OCR umgewandelte Texte können bearbeitet und weiterverarbeitet werden. Dies ist besonders nützlich für die Aktualisierung oder Korrektur von Dokumenten.

4. **Automatisierung**: OCR ermöglicht die Automatisierung vieler Prozesse, wie z.B. die Verarbeitung von Formularen, Rechnungen oder anderen Dokumenten in Unternehmen. Dies spart Zeit und reduziert menschliche Fehler.

5. **Barrierefreiheit**: OCR kann dabei helfen, gedruckte Texte für sehbehinderte Menschen zugänglich zu machen, indem die Texte in eine digitale Form gebracht und dann mittels Screenreadern vorgelesen werden.

6. **Archivierung und Langzeitlagerung**: Durch die Digitalisierung und OCR können wichtige Dokumente sicher archiviert und langfristig gespeichert werden, ohne dass sie an Qualität verlieren.


### How one performs OCR 

OCR technology is increasingly being integrated into basic software applications, such as PDF viewers. Tools like MacOS 'Preview' or Adobe Acrobat feature built-in OCR. But this is not suitable for **bulk processing of corpora**. Therefore one still needs **specialized OCR software** or programming packages to process **large quantities of images/PDFs** into machine-readable corpora.  

#### What OCR tools there are

The field of making OCR tools is developing rapidly (together with all other fields of text processing), so there are always new tools challenging the old ones. But as of 2024, the well-known products were: 

* FineReader (commercial, has a desktop interface)
* Tesseract (open source, command-line interface, also some third-party desktop interfaces)
* OCR4all (open source, has a (dockerized locally deployable) desktop interface)
* Kraken & e-Scriptorium (open source, e-Scriptorium has a desktop interface)
* EasyOCR (open source, has a desktop interface)

#### Performing OCR with Tesseract

In this tutorial, we'll do OCR with **Tesseract**,  which is open & free. Specifically, we'll use the Python package **PyTesseract**.