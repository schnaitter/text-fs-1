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

| Wort   | PoS-Tag| 
|--------|-------|
| Die    | ART   |
| Grippe | NOUN  |
| ,      | $,    |
| die    | ART   |
| weiter | ADJ   |
| wuetet | VVFIN |
| .      | $.    |



## 3. NLP mit Python 
In Programmiersprachen gibt es Bibliotheken, die Methoden, wie z.B. zur Textverarbeitung, bündeln. Die Bibliotheken können installiert, in den Programmcode geladen und dann angewendet werden.
Für Python gibt es verschiedene Bibliotheken, mit denen die Verarbeitung von Texten mittels NLP möglich ist:
* **[spaCy](spacy.io)**: Unterstützt ca. ... Sprachen, leicht benutztbar, anpassbar, weit verbreitet, schnell, eingebaute Visualisierungsmöglichkeiten, weiter trainierbar (aber nicht so flexibel wie nltk?), gut dokumentiert 
* **[nltk](https://www.nltk.org/)**: 
* **[stanford-core-nlp](https://pypi.org/project/stanford-corenlp/)**: nicht mehr maintained, wenig benutzt, wenig dokumentiert 
* SparkNLP

Neben den in {ref}`corpus-processing-intro-2` aufgelisteten Methoden 

  * What tasks can be carried out by the libraries?

`

```{note}
Die Vorverarbeitung ist sprachabhängig.  
```

`````{admonition} Test
:class: tip
My text
`````
