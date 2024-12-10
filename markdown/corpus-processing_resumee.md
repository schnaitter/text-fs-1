---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---
```{code-cell} ipython3
:tags: [remove-cell]
from jupyterquiz import display_quiz
import sys
sys.path.append("..")
from quadriga_config import colors
```

# Resümee

In diesem Kapitel wurde eine Übersicht über eine [Auswahl an Methoden des Natural Language Processing](corpus-processing-intro-2) gegeben (Tokenisierung, Lemmatisierung) und es wurde gezeigt, wie diese durch die Python-Bibliothek spaCy auf ein Textkorpus angewendet werden können. 
Im nächsten Schritt kann auf Grundlage der Token und Lemma das Korpus an Hand von Worthäufigkeiten analysiert werden. 

## Lernstandskontrolle

Dummy-Quiz:
```{code-cell} ipython3
:tags: [remove-input]
display_quiz("../assessment/ocr_quizzes.json", colors = colors.jupyterquiz)
```