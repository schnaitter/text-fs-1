# Einführung - NLP als Methode zur "Semantisierung" von Text

## 1. Was ist NLP und warum benutzen wir es?
Für den Computer ist ein Text eine Liste von Zeichen, die nicht aus semantischen Einheiten wie z.B. Wörtern oder Sätzen besteht. Sobald die Operationalisierung einer Forschungsfrage von diesen semantischen Einheiten ausgeht, z.B. auf der Häufigkeit eines Wortes aufbaut, ist es sinnvoll Methoden des [Natural Language Processing](https://en.wikipedia.org/wiki/Natural_language_processing) (NLP) anzuwenden, um den Text mit zusätzlichen linguistischen Informationen anzureichern.  
NLP ist ein interdisziplinäres Feld, das sich zwischen der Linguistik und der Informatik ansiedelt und verschiedene Methoden (regelbasiert, statistisch, [maschinelles Lernen](https://en.wikipedia.org/wiki/Machine_learning)) zur automatischen Verarbeitung natürlicher Sprache umfasst. Diese reichen von der Aufteilung eines Texts in Wörter ([Tokenisierung](https://en.wikipedia.org/wiki/Lexical_analysis#Tokenization)) über die Analyse von Emotionen in Texten ([Emotion / Sentiment Analysis](https://en.wikipedia.org/wiki/Sentiment_analysis)) bis hin zu der Erstellung von Chatbots ([Dialogue Systems](https://en.wikipedia.org/wiki/Dialogue_system)). 

(corpus-processing-intro-2)=
## 2. Verwendete NLP-Methoden
Ein Phänomen, wie die Spanische Grippe, kann in einem Textkorpus untersucht werden, indem das Phänomen durch eine Sammlung an Worten im Sinne eines semantischen Felds umrissen wird. Für diese Worte kann dann die Häufigkeit errechnet und über die Zeit analysiert werden. Dafür muss das Korpus zuerst mittels **Tokenisierung** in Worte sogenannte Token aufgeteilt werden. Verschiedene Wortformen (z.B. Krankenhäuser, Krankenghauses) sollen bei der Analyse mittels **Lemmatisierung** auf dasselbe Wort (hier: Krankenhaus) zurückgeführt werden, sodass die errechneten Häufigkeiten besser zu interpretieren sind. 

`````{admonition} Beispiel
:class: tip
Ursprünglicher Satz: "Die Grippe wütet weiter." \
In tokenisierter und lemmatisierter Form:

```{table}
:name: Tokenisierung und Lemmatisierung
| Token   | Lemma| 
|--------|-------|
| Die    | die   |
| Grippe | Grippe|
| wütet  | wüten |
| weiter | weiter  |
| .      | .     |
```
`````

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

Da die Vorverarbeitung der Texte keinerlei spezialisierter NLP-Methoden bedarf und auf Grund der leichten Benutzbarkeit sowie der Geschwindigkeit benutzen wir spaCy für die Tokenisierung, Lemmatisierung des Textkorpus. spaCy unterschiedlicher Methoden für die Vorverarbeitung bereit, die meisten basieren auf maschinellem Lernen. Da die Vorverarbeitun sprachabhängig ist, stellt spaCy für die unterstützen Sprachen (über 20) verschiedene Analyse-Modelle zur Verfügung. Eine Übersicht über die von spaCy unterstützen Sprachen gibt es [hier](https://spacy.io/models).

## 4. Zusammenfassung und nächste Schritte
Die NLP-Methoden, die für die Vorverarbeitung von Texten notwendig sind, wurden erklärt. spaCy wurde als Bibliothek festgelegt, mit der die Methoden auf die Textdaten angewendet werden. Im nächsten Schritt werden die Texte, die als txt-Dateien vorliegen, mittels spaCy annotiert und die Annotationen werden in Tabellen (csv-Dateien) gespeichert. 

## Mögliche Fragen fürs Assessment
* Welche der folgenden Methoden wird benutzt, um einen Text in Wörter aufzuteilen: Lemmatisierung, Tokenisierung, PoS-Tagging?
* Ist die Anwendung von NLP-Methoden notwendig, um aus einem Bild einen Text zu extrahieren? 
* Was ist die lemmatisierte Form von "ärmer"? 
