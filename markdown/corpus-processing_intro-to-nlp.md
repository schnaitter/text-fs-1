# Einführung - NLP als Methode zur "Semantisierung" von Text

## 1. Was ist NLP und warum benutzen wir es?
Für den Computer ist ein Text eine Liste von Zeichen, die nicht aus semantischen Einheiten wie z.B. Wörtern oder Sätzen besteht. Sobald die Operationalisierung einer Forschungsfrage von diesen semantischen Einheiten ausgeht, z.B. auf der Häufigkeit eines Wortes aufbaut, ist es sinnvoll Methoden des [Natural Language Processing](https://en.wikipedia.org/wiki/Natural_language_processing) (NLP) anzuwenden, um den Text mit zusätzlichen linguistischen Informationen anzureichern.  
NLP ist ein interdisziplinäres Feld, das sich zwischen der Linguistik und der Informatik ansiedelt und verschiedene Methoden (regelbasiert, statistisch, maschinelles Lernen) zur automatischen Verarbeitung natürlicher Sprache umfasst. Diese reichen von der Aufteilung eines Texts in Wörter ([Tokenisierung](https://en.wikipedia.org/wiki/Lexical_analysis#Tokenization)) über die Analyse von Emotionen in Texten ([Emotion / Sentiment Analysis](https://en.wikipedia.org/wiki/Sentiment_analysis)) bis hin zu der Erstellung von Chatbots ([Dialogue Systems](https://en.wikipedia.org/wiki/Dialogue_system)). 

(corpus-processing-intro-2)=
## 2. Verwendete NLP-Methoden
Ein Phänomen, wie die Spanische Grippe, kann in einem Text durch Worthäufigkeiten untersucht werden. Um die Prävalenz eines Phänomens zu untersuchen, kann es zusätzlich hilfreich sein, Worthäufigkeiten in Beziehung zur Häufigkeit aller Inhaltsworte (Nomen, Verben, Adjektive) zu setzen. Um diese Analysen durchzuführen, muss der Text wie folgt angereichert werden:
1. **Tokenisierung**: Aufteilung eines Texts in Worte
  * "Die Grippe, die weiter wütet." → "Die", "Grippe", "," ,"die", "weiter", "wütet", ".")
2. **Lemmatisierung**: Rückführung von Wortformen auf die Grundform 
  * Krankehaus, Krankenhäuser, Krankenhauses → Krankenhaus
3. **Part-of-Speech (PoS)-Tagging**: [Annotation](https://en.wikipedia.org/wiki/Annotation) von Wortarten an jedes Wort.

```{table} Beispiel Part-of-Speech-Tagging
:name: PoS-Tagging
| Wort   | PoS-Tag| 
|--------|-------|
| Die    | ART   |
| Grippe | NOUN  |
| ,      | $,    |
| die    | ART   |
| weiter | ADJ   |
| wuetet | VVFIN |
| .      | $.    |
```


## 3. NLP mit Python 
In Programmiersprachen gibt es Bibliotheken, die Methoden z.B. zur Textverarbeitung, bündeln. Die Bibliotheken können installiert, in den Programmcode geladen und dann angewendet werden.
Für Python gibt es verschiedene Bibliotheken, mit denen die Verarbeitung von Texten mittels NLP möglich ist. Am weitesten vebreitet sind die Bibliotheken [spaCy](https://spacy.io) und [nltk](https://www.nltk.org/), die in Tabelle {ref}`cmp-spacy-nltk` verglichen werden.

```{table} Vergleich von spaCy und nltk
:name: cmp-spacy-nltk
| Bibliothek | Vorteile | Nachteile | 
|------|----------|-----------|
| spaCy| <ul><li>kurze Verarbeitungsdauer</li><li>leichte Benutzbarkeit durch komplette Pipeline</li><li>Visualisierungsmöglichkeiten</li></ul> | <ul><li>Weniger flexibel in der Anpassung an spezielle Anwendungsfälle</li></ul> | 
| nltk | <ul><li>flexibel in der Anpassung an spezielle Anwendungsfälle</li><li>Transparenz einzelner Schritte in einer Pipeline</li></ul> | <ul><li>Lange Verarbeitungsdauer</li><li>Höhere Einstiegshürde</li></ul>|
```
`````{admonition} Zum Begriff der Pipeline
:class: tip, dropdown
Die verschiedenen NLP-Methoden bauen teilweise aufeinander auf. Grundlegend wird ein Text zuerst tokenisiert, dann folgt PoS-Tagging und die Lemmatisierung. Diese Abfolge der einzelnen Prozess wird im NLP häufig mit der Metapher einer Pipeline beschrieben. 
`````


```{note}
Die Vorverarbeitung ist sprachabhängig. Sowohl nltk als auch spaCy unterstützen über 15 Sprachen (die meisten davon aus dem europäischen Sprachraum). Eine Übersicht über die von spaCy unterstützen Sprachen gibt es [hier](https://spacy.io/models)
```

Da die Vorverarbeitung der Texte keinerlei spezialisierter NLP-Methoden bedarf und auf Grund der leichten Benutzbarkeit sowie der Geschwindigkeit benutzen wir spaCy für die Tokenisierung, Lemmatisierung und PoS-Tagging von Texten.

## 4. Zusammenfassung und nächste Schritte
Die NLP-Methoden, die für die Vorverarbeitung von Texten notwendig sind, wurden erklärt. spaCy wurde als Bibliothek festgelegt, mit der die Methoden auf die Textdaten angewendet werden. Im nächsten Schritt werden die Texte, die als txt-Dateien vorliegen, mittels spaCy annotiert und die Annotationen werden in Tabellen (csv-Dateien) gespeichert. 

## Mögliche Fragen fürs Assessment
* Welche der folgenden Methoden wird benutzt, um einen Text in Wörter aufzuteilen (Lemmatisierung, Tokenisierung, PoS-Tagging?
* Ist die Anwendung von NLP-Methoden notwendig, um aus einem Bild einen Text zu extrahieren? 
* Was ist die lemmatisierte Form von "ärmer"? 
